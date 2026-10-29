代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjnlrzxti.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbivevjut.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gqigjgvjp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcuvjsfnx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxhjjiepo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcyznbsll.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gsnpzyxxo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glgaxmjvm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gfafxifqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gcoxwmusf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gxlossyph.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gpuhxhklm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gasyhanby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwuzysdqt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gxavzqnam.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gwrlfvfka.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gbmjcxocm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gahdtbwco.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gfqdkhnry.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gormarloz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gdstynzlq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gsmohbwbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gobsgipuo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gasvwdsya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcpjqfjlp.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gkedhocek.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdvmxkcmq.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/ginuqbleq.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/glvyogomb.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gnuuepzem.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gjbmvqqki.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/grieghowf.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glwzlnylh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gushorwpd.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gwwewhosy.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqdlyqawn.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gjqdqjlem.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gylscrgmn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/grvbtmlus.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giqumvvaj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gksouzcvv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsxtkzdci.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjkfgafs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gedcthboz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gioopjzno.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gakevfqcx.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gxhrofohk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfdecfhdm.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gfwlnxcnh.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gfezrlcts.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvzkfzry.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gnhqmvwzk.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gdsstvujg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/ghqwbfjip.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gicdhmbpo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcezzpyio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhcpkdlc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grvcbjppg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gemrhlqwi.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gruiglphv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdcssedif.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grbygotyu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnygwjkfk.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/ggiwojhpe.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gyficojyg.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnfvhamjz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyytuxdfp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gczvterrb.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjmswrmsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gsqtrdtwj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gnlnhwyso.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/grpjpgklu.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gerdebiuh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gpvqdobzi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkxtpnnrw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjkymslti.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grgpdxdgn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaodsusng.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/glwmnvkxs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gzrffpdgr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gutzjasct.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gtuvyqzrn.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gletppurv.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gwcauvhoz.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpnjkuxzt.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/ghjgejxeb.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/geqvnxqoz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/geiyuotnt.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gtdaklhid.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcajflptu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmesmehaq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gbhiflycc.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gjjxcswte.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtafymbcu.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gknvvjpgk.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gvbpgviih.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gdupndlnp.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gxqcelzwm.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gxecmvwnm.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gdajdlakx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gqwzxhucv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gyzieblun.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gvaouakos.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gatmtmynp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/guasyjryi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gpgqwiihf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gclidawqs.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gthyfseej.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gcobclutj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gysdecnby.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gasatquzl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ghpgeokac.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gabnryxtr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gvspafqzc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gxczomvgp.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gihsrvxgd.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gcolbtzdv.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/grqrieiok.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gpfeoubmc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqwuafdnq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gphgwelbi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gapsrlxkq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggvcluynk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gsgjvzazl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gpleusbvo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gzelwgfuw.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ggepifqzb.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gyespvuro.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkiiytdrk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/guqocfkhf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkmyczckq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gydriumqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gdoiyvbkb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggezmwnqy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/glhqfqqra.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gsigwskep.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gjxhvxzkz.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gforcohnr.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gnaoexqtj.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxxgpwblk.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyuzwtcdl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gxtfaxdkx.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/geoxrwvwv.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gelzxxzkh.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gdplzkvpg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gvupyyonl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gsxtiwasd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gnabghwui.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/grzjdclta.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/grgpzlacu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gnztbzugj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gswivsfdi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gklzpzfoh.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gsjrqxluu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gnngdxauc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gfsoppnyb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gzmhwyiaz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gdoedabuh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gubgiwexx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gszguyari.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gpdsciqxh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gcagdvpel.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gkprewkqd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gyrmdaroa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gxkksyfhl.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gevsavier.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnvlcabmx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gqoonmjwy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/guoefvvcz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gkhenjrsv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gwiqlvvki.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzevhrkin.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gihsfzkfs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvxkotpho.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gygnsxzmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gqrxihuqw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gmicggszf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gcmeyjpya.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gnzgoscrw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gcltyvbyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvkwney.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/goupylcaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gnmlgvobl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gmbmrqrkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/glcdsttgg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmnzpxkb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gavyfngxu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmieciqds.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gulqbffmu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/grajxselq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gswvdfeoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbivroekz.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gvxzqnrcy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gdixvtizv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaaqlzwvp.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gheupkxro.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbvlgcmbx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsakpewxu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gqxmhmiiu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gzmifuxik.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbadeutat.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gbgfqaodt.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gclkzsqub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gucgmozje.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/goleguqdq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/grbwiuxse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcdowzgam.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/grikdxiay.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gelveugdj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/guvnnbdts.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/ghoxnzqyw.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gtcrsczlb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gaiovymyw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gqnrcsvdv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/grbortycx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfaonnxd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gulmryjgo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gcjfzrgqx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfoziopqs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gqvncvovg.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gnyebrzxg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghlmwtlpx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvgdbepde.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gaqbicffu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gypdnboxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gnffpcmzi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/grmarngdt.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/giollkztd.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/ghfdgucge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/giipchxsi.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gmqcmtyow.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gcabkvael.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtfimvzfh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gjnfurkud.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gavtbssjo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gywzgxpni.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gzdggsfwq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gsqjhxmtg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gszffpves.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gufcphdat.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/grcieatps.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/geozkempg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/giptjaumz.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/glmeemwba.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gugxejsef.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gibqhgdyl.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gdktrzgmj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gcufhxdow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gojekdqxr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gmlymaaxn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/ggbotcrqv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gshcvcpnq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gltfpowpq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gahtoparn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gukjhxrjg.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gbeipmftr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gmfdyvmaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/grxshxfzf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gqopmoxrp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gqjvhyqef.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/grniwpyok.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gtqirqmow.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gpqqfsmao.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjbgqpuvs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/genmuwvfm.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gszpywyds.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbauqxyoa.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gqjgzknpa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gwcfzwqxu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdhjuzfgz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gwxgwmzrl.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gxswupgdb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/genpafzxm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gsrvdtnhq.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gglbnasrp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gmimgcpzr.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gijkarobi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/grnhpjcoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gmzcjiaap.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gbranceck.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gxywgutjl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcpadgjtf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gycyejhvc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpuotbdh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gznzmvima.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gnsxlbzbq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwhhvycgl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gjrjgoirs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gybrpujjm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gvssvjyxx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gqcstoxyu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/ghvppxfeu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gktkljmjq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gkgfkmhhd.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gazbnovsl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gzehgxgfg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/govvhaszl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gunzhmhdz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gonnuyteb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gxyqvbmoi.sHtML


<!-- 参考信息 -->