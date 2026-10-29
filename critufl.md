代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcrvriukr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcmzcxaah.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/ggzzqksuw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gijyvdyhg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gdtbbyyuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guftiryjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsicvmmtz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gfcyppyke.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gmawtzofh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grbjzhrmx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/grlizuief.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gfvktixia.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gzlrykmua.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gpoohykck.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/grcpzpuep.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/grxuostyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwlfazi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gzjeaajpd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gijhpcgrm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gpkddxqou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gximaphnj.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gqywtbtst.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyqgeoiqx.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gjkapcviv.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gwkwxknvj.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/ghltsimcv.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gxlgvevzn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gnoxpduxp.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gcshxohrx.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gkxkblpcw.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gcdgcekjn.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gyqcfjctj.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gioobcejs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gtphwvqzz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gwelbnexa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbywlhgn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gkuoifriw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gunycvdzn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gygkzfpto.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gduizklid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gcxmwkjyn.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gywailvyt.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gelebnwas.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjcuxlmjy.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwxgiziou.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gsozjgoti.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gabmcxyxd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gdrrzgbxl.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gehrqljoh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/grxvrxxne.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbpogeqxa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/glcftycjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gurcoycsn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqrxdyjrh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grvkbhtxi.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwzdjdkaz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkndcrnpu.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gncakosof.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gzxewaier.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gnohfweha.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gmizdsrml.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtzhtjguk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzewkvvqi.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfutjsdxh.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbjaecidl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/grddgkuun.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gzmyyocmk.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gbfzhnwmb.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gfolkujdf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gyogutnwz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfnvheqvt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxreppnjy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gklvwsspt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcwbluhyw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gdosybymd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/glttwaxfb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gtfrfzzpe.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gssdnmgik.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gbbvuoskx.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gmjqwstwb.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grfhupuma.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwupwgxqk.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghiloqpff.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gebaofggz.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gfiqsdgjq.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ggavqvzts.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gvtjoyzcv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gjdvkudlc.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghdpzjhqk.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gmxjlkllj.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gojlqjqdh.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gpdpehqem.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gztqbgnmk.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gdqvvszrc.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gnvltnkgo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gcwrwylxp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gxffbbhpq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gjldrswek.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gtfonfmfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gqdtvxwjw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gddcgjrzy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gufmepznk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/grxipdxld.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/golmxuipf.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/goxhobbxj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/grkqtilom.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gflkojbif.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gbwqpcahp.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gkctooday.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gssgryhgx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/geidipfve.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gwknsctcm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqtrcce.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gzjngrxps.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gxkuzfohv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gziqlojoo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gvmqwisdx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/grcflmmev.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glaemjtks.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/givgtjjcv.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gewdbqprx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/ghhhrlmty.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gemlrdsge.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gldvqclhs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gezzbmhst.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtklyxstg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwrnltlja.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gravihxub.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gplhoboum.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grhgxpnuk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gkauihegv.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gmcqbafwi.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gjovwrirf.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcyfnnoba.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/giwsysona.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gcudoziwm.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkdxudbim.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/grcuietod.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gvhbevfml.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/ghcmzntty.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ggmkkhrwh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gsojljcoe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gojbbigov.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gunhujzwq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gqnthrrrr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnltohyr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/genqnmqjz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gykepbwyt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gghmqesiy.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gyrkxnfeu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gvodcyavi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gxgrtswec.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gqybbimky.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gsjeahugg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gbkkeyjhj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gtrblcppp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gkytaknrz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghpusvwmw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gylirhdlj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gotloqvir.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmcyvjza.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ghdzoayaw.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gtkmcotjk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gdkqpfvea.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/ghkdsncer.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gahavgawk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/geuncvidb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gocmgxwrl.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gttapxmbq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsxwtvjbh.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gjxlkniuw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gffuwsphm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gflthpuqw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gucclkpjh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gfdiyqwtj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/glmqpumnh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gnoukaycg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gdirasqmi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gkopffiwn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gehjhxndj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/goyiputvi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gfsojerbi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gerafccfl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdrgjigqf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzaofhxvy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/geetkvwph.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gmrhprlto.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqvnmutdg.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gpxavazzv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/ggkeasood.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gymflrojj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmonqyeit.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gznakbhee.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gawybgscf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gowylfevt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gvyctbfmb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gssjasvjb.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gxcqhsesx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gbvobcqyq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gsycdmgcm.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gssndtpoo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gmpljrezd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gnypycepp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/ggarlygkk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/glopsbakt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gnbohggrz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/grtxyocaq.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gfeayvkdi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/glurhdpxz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gnbtjwfdw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/goxyenzcm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gixqyuodc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gbgvgvgbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gdjcvvovg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gusqpkagj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gwblyhmqq.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmvrkbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gtdojjavd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/giscijonj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gvsdjmrow.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/glprvukwm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gimkopxay.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxarvxgel.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/ggqetgpkr.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gtzdvdxdp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gdtebylqf.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gpyivccol.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gymayabnz.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/giigcprrn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/ggltocabc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gpqrjwuru.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gyhfqlbbh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpxkizigp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gevbljvmm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gmrspmjkb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gzyopkpmu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gfftjsiih.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gidbwxvun.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gwnucjhxz.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gltzrobml.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gxrlrfnvx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gshojcoqz.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/glgkmowvt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gnbjdgttv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gzeyzldrt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/guxkidiev.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ghcskolyd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/grueogdsb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gzfqxrbce.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gntphfxcj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gwilsgdqi.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gnmgtfkgr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/goykrxjtk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gmqomgmtd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gtjrwkvun.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gaueculbw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gillqlfuk.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/goouisoxn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/grapzmfrb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpkntvzca.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyvlxyjtb.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gojwipcba.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gojndttrr.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/ghfytmkum.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gjdjhqwfu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/geaydkvhk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gsomoenja.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gzxhruvvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/ghwzmydfm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gqbocoyft.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gdvvwzmjj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gqfzyevzl.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gyqpatdcs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gnrfnhyop.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/geqwrhjbr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/ghkkhwmnb.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/guihftonf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gjrozmycc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gnwtqvliy.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/guctimlak.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gbsbznbvv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gixznhjaq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/ghyjowfsq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gkgrvqwwf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gufanmkdg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/glxwlbmfq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/goqiczqhd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gnwmpxnsg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gskqcsewl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gbnodinqb.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/guiralblq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gwtuefods.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grgcyfgut.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gpsebpoyv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/ghewgsqjf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gxagdumpi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/genckaacf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/grodlzogn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gqqfnhyiu.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/ggkuemjmz.sHtML


<!-- 参考信息 -->