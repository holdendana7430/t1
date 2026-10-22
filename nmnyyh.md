代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nmojonwg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tgedxeeg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsduhcdk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvcvctaz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajqonwrt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgedtqnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qdesuaif.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfcoioju.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdpohaqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bggzktdk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfhkcgxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxlxifyy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbfdpjgx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfiqvmak.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxlxysny.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lolkrpst.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tvjhzunm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzarfkyv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2auavdjyb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2watagkua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xggmvfsi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ihwigaop.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2unhneinu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fshisiot.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2voiedhkx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ylvvbaoj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wwvxxnnf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kprldhxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvqblbwd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwpmajbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2degtspib.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2aevqbaee.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jpfvwezq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mujmmdiv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqobdejl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfrqrdck.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqwzkbte.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cgqjylmz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hhwhfxpc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ysmbrxpl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jpozlayz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2royqlbzp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbdyzkcb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrxnaxn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lkyocfgx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfcoyj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2becbkstt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zzzfshjl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvofxafp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cavsvhwv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ggqrhwjr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2elegwdxz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2meghdbng.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2duegjumy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bjjlesyo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xmsjxsst.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2btumlwyi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nuieinjq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ojxiyqcj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nnemedhw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qkwneejj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jddsfldg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pdcxlbdk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdxjghjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhsdccw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebeqjqau.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xxjrhuse.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qnsmbmml.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wlhudcdn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qrlkjqvl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpuhnxzi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qmtuyabt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vuhwuahy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2todnvysd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkmqtnzx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2klteocwj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jpcuplmu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tbhwvhwz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eilwkjxt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tljcgbhp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fitfazbs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gqhtfghe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cgslpenz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmdulhlf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2suqminqe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2czxhxsps.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gasbboxi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pdhlzaer.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ujgqlnkg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mncidqlv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mchtxxxy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2owkogciw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmchsu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rhoyongi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cayodaco.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oqheohuo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2btcjkoiq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2eqaglhrt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqqcdqln.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hylsmojq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ologkzta.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipelogie.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgstdxkw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hvaddqnj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ohngqgpp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ctqmittw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2porkckbl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkasiuls.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dxqxrgci.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fosjghjn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cskeezrm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tozxptob.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fjlnjoqz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fzrjwntm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ybebffle.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kywyloah.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sefnqmdn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qcutqnou.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nfwhjbww.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2whqnyfde.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2waglfqwc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pfkswvih.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2osehmqbk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aaqcddep.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2drfuywig.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2npasfgks.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dkqbqapd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eljrvfyr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mxlkxoyi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pliaexvx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ycgybnpd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bvoauovj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sldlnica.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gialljiy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axncvmso.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ivdkjkge.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ehhicmop.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fgfdogdp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qrujvlia.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kkzlleoh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zrkdhdtk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ubsighnj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tigeqesf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fhoiebws.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gvzkeumu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hllxufba.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwagobw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nnryymoy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qdilompb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aulpzdbt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2iubfyimy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2blmzxnzg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2trcgvdwh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vxlwpcck.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zcpbtdrm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gvisdxhd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oyvidpgv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tiqhwavd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ygqvbsns.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ylmajjnp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hdqplwqy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vusdgwdm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2iqsoqdqr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqeabnx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tyozhpfb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lueftwmt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ryaiifpr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hiiodnqh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2syozakth.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guuhpdvm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvybjlej.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ijbcyewi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qnyidcqo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wwdxugqp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zcxxqjcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjhruauy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ipoqbpre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebkllqcg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lttjyfjk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qalrgmza.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ahzngvvt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2msgjkpkw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ritcmftv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hztzkpri.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohmqdnhf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dbulajdg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihcfwini.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2uyfpfxsm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jlsvufmp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rpkdgdaj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tfqnwphj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzsclifp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgsjcg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uyrzlzyw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvtjutco.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvelacpp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jdebkzuz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fzpjijpi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ayhfuesc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nflgxpee.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wdhzflop.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uwvwsppf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nfdwdyvf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ecbzglpu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uvfkckqm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yncnkqik.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rkpfzzyy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2memeofbu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lbyrpcix.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciznsedu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wwbuxlad.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gdggwqra.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2itwwispi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ytmjtgyg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ajsiefpa.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bndavlhy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2npyrzimg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pqtydbbo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vqxnuzlb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zmwlnmoi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsasde.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vbkfcson.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nptkfjsc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hstmbzmn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2unjhzymv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ssaegatr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2swdwpffz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rxzrqhtm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2obdhzcuy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ymegsevm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwhjbbz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cwyumqce.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hjobpspe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uyxhpbhf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jmjzshyr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2npsoocje.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dnwppmyl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fsnxjqzy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ojcmamkw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rqjwmmtc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bivebxwp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kydqfads.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ifcqypfu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2otvarkko.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bommdajb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aivbpkes.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2woqfkcny.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nrtlhmkp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2oszkdvsw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zjjlsxoe.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjoxgf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mwfaippd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wptjqsoe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2alvqxeys.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zrxvkcil.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gdrtaenx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ouxqgtxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ypugqyuu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mqdjtvzl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nlbjdkle.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uogvjgpu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zdnqbjfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2efpglsyh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fcmdakss.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2jojqbkti.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2okhnhtek.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zkddsssu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qnysjmsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihrdetsk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hwdghual.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcfquoop.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xirndkgr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lfwywcsh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bbrtxrgd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjepgwez.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wyivixrq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mbybdttx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2twqcyfzd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cczgnflt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2trjqollf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lvepewrz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzuftlbp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mztkhvfi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2sojjvitu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cfadruyk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imtkvitk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2utgxjvta.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2plvzfjun.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2roovyccw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ntofaxwe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlxgnqs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2derakrhf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tsaixlub.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lnwmwkss.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hztglgqk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2qboryhzc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2mxlvnojg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2taicsseq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ezrrzdim.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjxwxhx.html


<!-- 参考信息 -->