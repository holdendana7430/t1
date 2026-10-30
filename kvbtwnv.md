代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/ggdjtwgxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggabqszam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfngiqprm.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gvtnbiast.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gjlslljis.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/geuuzupwa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/ggmopivxn.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/glxkrelir.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gqhpjxtln.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gxdioldgv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/guxerbsmb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gxvodyggh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzmunszrq.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gxcapuvsq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gakzmzoml.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/giefztjxb.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gqemqoqca.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gcnnoczwp.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gmyctqijb.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/goqtkjzul.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gebmgmwiy.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gdlqgcuxj.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/giveqkjwo.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ggqatounl.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghavyetqq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gimecmrpn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gxssdujwl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gpbvmeqpx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gkvtglpuv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gatfgfmrn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gkmlywphn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gjqjgghok.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/glaqqacxb.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gsqtozvui.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gensnpdql.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gzombwiaa.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gowptubbe.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gaaynetqi.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbxuahqrm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/glllprxqb.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gluhzhgtm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/grrgbjngz.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gwpzsmaai.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gbpkeinyb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gzwxxmhgm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gfajivrya.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/geayhnuqb.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gkinocmgx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gllufpils.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/glzcduzht.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gyrjrpoci.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gibshasyj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/guokswsgl.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcjlxamjk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/giznztlgh.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gciyhjqdp.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gtlbzclku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/garuwpsjg.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gohjpnmbd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gachmktbs.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gctpkahwu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gspodkvae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtzekmvou.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpdgypodu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvshzwzoy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqkjlxbyu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gahtfbsbi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gusvfrvqf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gpzhhdxba.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gsrvgvaeg.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gtdxffpfq.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gtgusjoih.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkohgftld.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/goivjlxvg.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxrjfuizm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/ggzkhdoxn.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gxsbybimz.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gglqdwoke.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gggctqwij.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gtxvbqjzc.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gzsjchebc.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmnqffdko.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gwcqtzjie.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gcgbiisnd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gpduaxhiu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gsfsbgndp.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ggazkrqqx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gojtbkvdv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gvyiebapp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/ggmedktjt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gahxaaykb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/ggjivzqaz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwmwstgsi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gwohyebzl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/giqunjzcz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzfcxtahp.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ggfeimoyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/guswlmoip.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gipaxbolb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gzemextck.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ghvkaynbd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gdnaxnvnf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gisffwqqd.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gkrtwaepk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gghxtimzr.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/guteyyquu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gmhbniudu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gomwrjoby.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gaixburmn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmafaylpk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfulziefy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdeghuwwe.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gvwvpomkd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gfhhhqbut.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gwwtmjcdx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gzlpmsgjm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvebizuhu.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjwtovkyg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjwrjmszr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/glmouyfsg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdhuscnqy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/grodrlidk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gpntsesrd.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gmcblwvut.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gwygbqtuy.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpkkrqier.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gkxpvofdt.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzykixvgf.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggtbezbiu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/glfsllbvq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gatnckxgy.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gsbrjfltt.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/grconijsv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmmcffwcf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gispznzgs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gmkwspdrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gaheqdhoj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gxewywgdp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gdrrhavaf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gdryuqxpz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gfepzzzur.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gliforpcs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/geeldxzqx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gskxxryyi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gzasukjqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gsqmilpqz.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gqqgyirik.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gzrhjlakz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gofydyqcs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gynaxrguq.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gxvzstcru.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gzosobrzt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gezcyazje.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gvcozxvci.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gwcxlrlfh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gcfrcnzdb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gikhkuhyy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gbhfmgsdr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gsmyojcir.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gazvdknqi.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gcwfpknzr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmkfbpcxf.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/grjxyodsp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gieoynqbv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/guauuhpzm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/goknpmvob.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtxeewxcp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gtrkbbahq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gzysxthjb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gquscwpxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/geplbgaih.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gbzaqfcxt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gdsfsftpv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghixjmdch.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/goxsqfdcp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfragwbky.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcyrqxipv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmygnuhge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gbiwswfse.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gehskbyiv.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gteafawdw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gswrfiauw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfodhzswm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghwxttcpj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ghlcjvgcc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnkbyatsi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gujkixmmb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gmmyqvlsh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmbahtfea.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gmdzhlzfb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gxticprko.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gfjzuxjyz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gklyuadlf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ghqhlwswm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/goqsuolev.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gvmczvxpm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/glgbkrovv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gykffcjwd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gephlvbgz.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gezfkwfkz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gbelmeafs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/galrhuhmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gearmriqg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gvwxqaemu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/geksdloxm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gtdjygzcc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gbqsnddsb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/grehevsky.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gwdbwlwzj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gdsavafks.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/goqovczlx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gugkoxsru.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gjnrqqpac.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gxlhayeht.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/giutsagim.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gntbyfjmy.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gzpcsdido.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gtocfvjza.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gewsdmmmq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtsigclta.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvhzimzyd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gckwbfpfb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gpgbuoymg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/garnbebyr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/glzwdmuvt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gkwrthfpn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gcmrqbqwl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/ggvecdojz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gxbymrdql.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gbjcyimbu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gymaklfsx.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gomqsudbu.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gpydeezuy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/goiznngqg.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gybmhivjz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gsigaakjg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/ggxkcjvzq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ggbbfrdfd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gnqjckxba.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gpqeyeqff.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gkauxwpzi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gpeoajobe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/goemvrgiz.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/goxbtqtca.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gchszteaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gktxlumnx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/grtflhhll.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/ghmniwyzw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gjswpmwow.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/girxwwulk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gajkrxyrn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gogcxzerp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmhhkuew.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/ggrcocxth.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfonedofm.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gnwakwibz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gfqpzrcrx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gdybtslud.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/grolkgnen.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gfubmnmvn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gcxqhhdpo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grsnavihf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gnkuphsed.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gpzyioszb.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gycuxccfq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gkchsexok.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gipweeiwv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gbtikclie.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gneluzekl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gpfcempzn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/goyesclhl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gsljyszaa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjbhurjch.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gkouptjjb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/glocotszm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/geefgpgne.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/geelkjrkl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gztalptqs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gekexwpwo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gvjbdhgfp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gwagbqoyo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/guqykqbtv.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/ghegrzgbl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gsqcmofuz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gzjqlqtcp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gewiwpsaa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gagufexba.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gecxllufm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gpfrtisih.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/glzgqhmsr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gcfrlzeru.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgmkzgk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gxqjjjhnr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggrghfntl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ghxvrbdbm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/glyiuganl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gbpnrgaiv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyfynjvh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/groxxuzsj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/guvdovdnw.sHtML


<!-- 参考信息 -->