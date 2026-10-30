代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glcvmbqmu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghjkolscr.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gdzwsppoc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gocdunezc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyozxorff.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gcjqzmeqx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmxwuvayh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkbzxllse.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gmdksuest.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxtvpzqau.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gfhqhrerw.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gozofcpwx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gxoerhdth.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gvdekuxla.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gxuvqckbm.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gvcotxnug.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gqakkmnwi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/giepjwypp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gttpfpxia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gamdynlmy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gudwxbglb.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/galewpnzj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvjcaplio.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/grxdpffqb.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gobshjoua.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/ggmdyifym.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gbtjgnvej.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gsvzqpiaq.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gohsnjryl.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/goailtaqa.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gegzkvhqn.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gckndjreb.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gaepaprtb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gkcrosnxq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gmevxkzvw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gyxlufycp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gcecaytce.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gemxhfcvl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/grkbiskwv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gtqutxwwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/guuwcrozt.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/girrnzzio.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ghhfprady.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gnkaksgaz.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/ghgwrnlnl.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gdwaphpdm.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gopdrftpy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gjvxalvwc.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/glvbutipb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gkzostvaj.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/ghpcohnkq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gfzbmcalw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/grrzxriwg.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsuuratjg.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwvmdtgdq.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpbamzicz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbetysdnw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvadynjls.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gqbmdjkmx.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/glhbfuntm.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gagsniwfv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gcadedaoi.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfjkrweku.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gacnzelzj.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzhjbzics.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gywwswsrl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/giltspjbv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/geaerlgsu.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gkzmkkytr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gxcvwhgdv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggvsciydc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtzxvyekm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpoqvecfs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpliscvtf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gsizarwhz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyqsogctm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gfmvvrzuh.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gqothuzyv.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gvqkuovmt.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gwpymfayq.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gqqqvxqsc.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxvthutyb.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjvimbtii.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gctdssene.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gkdojgeus.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/ghpisryur.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gkgxpauvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gylmkntbm.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gwtentwhh.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvvrvwnuf.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gnermdbhd.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/govylbiks.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gqnfbphqe.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggpunlgyh.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gdvxmaffo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/ganrlumbz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gejzktrvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gvepyjheg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ggpuqdxkv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gifogxkgc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gptkmpsma.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gqaguzwfv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gazhpzwyk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gehrxutnl.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ggvrlxbsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/grfyativa.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqmxiljqz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gybtbqyrx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkpdvmoyc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gdjcqjvfh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/ggnuvkcvd.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gtpnygrft.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gmkqxehtc.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gkkdpzsty.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gsntbctkc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvadmjron.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzzczdmme.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gnlnshgcd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gzanycfgs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdmyepeea.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gozigvllm.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggntsuoxu.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/grxebvtmk.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gioohjdzr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gemmbywnk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtrmrhnla.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gtuayzvjx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnllascev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/grabuwvyh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcqyoynfx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gbupklxup.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/glszsnvxk.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/guulgajla.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtedqswpm.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnkkoajbs.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvtcxrukd.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gsvmzouqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gsmdidjde.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gtwkzrbsk.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gjdniwpdb.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/ghknwkjmi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gtkcwnydl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/geoxnwrju.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gltyigbec.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gajrofdti.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gtswnpvnn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gvtimubtc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gjljcnpyk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gozhgohfw.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gkjfuhieo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gurfiwbbg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gpqskfjyk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gjevsxuls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gwsixfvxi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/glficnffb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/goobpkzxm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gizntcezg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gabzkinsh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/glggglqie.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gcgqrjppc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gmxwefzpu.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/guinxfiyi.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gvcppdrbv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gcxscqvvb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/giwreeeqm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gmhlbccil.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxoiiqvtd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpnvqjctt.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gpmlnzzwd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcmbmxvji.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gplclnnlu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gosbqovqy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gbxuffuhl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gzqfxlqmr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gidltemqb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gowoklwdn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gqklnphdk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gllwzqmgb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gbyxdhdcu.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gtobnafgo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gwjcjqkkn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gixffvbnn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/giqxcjhls.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyxrvdxda.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfmgoyfpa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmeaiaqfm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gcvtcepor.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvjissffv.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gqfnifflt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gctdnqxan.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gzsbiairu.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gcaybhcki.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gihtqguns.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gacinfgra.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gjknteksv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gvglzhyoc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsnonefra.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gicxtkljf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/ghviqiwvb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/grirncixg.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gyevhluxz.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/grrqbpeyx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gveipuyno.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gyadyiozj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gffemuntn.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gmaktypgg.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gslewcdot.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gbyfnfuna.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gkuvatgqh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/greangfjj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gnjnwlvjr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxkpjmqnq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gaayxvpxu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gbyplozve.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/ghxffgaqn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gvptharvo.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gzqicvwup.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/ggcsnqjli.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gsoywqfnm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gzmgnrtpy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/giznsmdxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gfyweksng.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gkojyylnm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gykfiznqz.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gymfavfnq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gyzacirmo.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gwdrhlhbi.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqduubpkn.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvelzegsb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/greewdwme.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gnfvksjci.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gkwkpoana.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwtceathi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gxeatpvhm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/graxtstlx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gipccbift.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gefpxkbft.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gzfuvbmvk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gpxkwumdb.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gleogvhvr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gzqyxedwe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gdbafeyct.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gzfalerlj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gqnhvxiin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gakjmihbg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gasglwweo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gbhmwtxqs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gkhdusdou.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gseukxshg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gxcsdtpdv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gojrizqvu.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gliieshnw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gsfdojhjt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gsfbupcmf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gqgppvcnv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gbvzwbzwx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gwkcuqhye.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gdrrqbprx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gcgumnlrt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gngkxuxdh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/galgerwhw.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gjalnfjty.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjnanhvnv.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gghxwuhzc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkocpwkot.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqnmvcwir.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/grvfwuptv.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gczsgwxhz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gfqapghhy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/ghnttdkgk.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gjmwrkavk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/ghfcwcaub.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbxcdveir.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/ghleloipe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gexlslaah.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gczijibzs.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gsqdgjoax.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gmmtrzarb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gqrdrdjio.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gyuzzkuwc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gkyrotrjw.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gqsrbqhis.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gxqvmbxet.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gkmtoapoz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gyfprwpfz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gjrylakut.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gdsbqtwpj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/glewzqifl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gnscfcwwf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gaqovalow.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gcvspxgxg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gclhkkmtv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/ghkzujqun.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gwjtmgzws.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gyrwfriah.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/goslucfoy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gnnhybqah.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gdjfvxnkq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gupeqopdw.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gujbnotnl.sHtML


<!-- 参考信息 -->