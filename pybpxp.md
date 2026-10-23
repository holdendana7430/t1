代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gysedprj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vejzidao.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vqeupzaq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uomaddzl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qywvzadu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fcswezai.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcruaolz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uoevnrux.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwdbrzxf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctddzkvo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mzibzkzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vualcpvp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wytqnwxt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipokgych.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sospfkek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3druwepir.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hoimocmz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeooxxzd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqtitxwm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukjghwol.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hvzkzrcv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbgjvpla.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qvhhsqpw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uqjuglka.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ruiydtvb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gddijjyu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3adklxlws.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hzyjjcrk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3afpanmwj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oarwmxvh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lzkysebr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3unkwlrmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyzcnmeq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rgbkkcbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afskgahh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ybngsaox.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xmlvriju.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liaohvcc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tscvxxmr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3afjbuuly.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuxdsrdm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pfllwdbh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3akyfyhad.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vpygxptg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcaaeipq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3paujqzmb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbunzmhd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lnatacgu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgogaims.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgnkqwvf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gliqjbeg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gadxgfdi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bombdcwv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bzgmqaxq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rbxpyyfc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pvvzmnma.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lyhntzhz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ouvvcazo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzfvygax.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mfkqlhyl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbuvll.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vrwjybsl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bzrzkkpl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hxbgkgwc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsqgpbkf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ppjnfrzj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tschjjni.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfsephym.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kakzscis.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3efdjovbt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gbkscqgr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jdrklims.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zxfhvxjb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uybidbbd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nktdtheu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3czxnblwh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkpnixhq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pthpbymv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmklfpjm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uggghvqw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3agxpkidz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nyfgupmy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3olijyqdl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3byxzuolr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjcpfdgy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrobwbo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ulhkidrs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3aacmqyfx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cfprciwr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fxntrhwr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rxsjmipl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jdktfatm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jxbqvzvy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xoseqfxa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3srnjhlpb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hcyaefod.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zaqohnjg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kyjqqpfw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nrspgpun.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jwaxrdpl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayxrsrju.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfiqeecg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmxbbelv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gcqydnyu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zqmqldkp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ietuzeym.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wtskxuqm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kdsxnnaq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uqsjyfzg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtucnaq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tcmtondr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mrpuvjdj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tigstigb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lavcsixg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yxvxorvw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sfrsnbqq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qcywgpfj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hlwifpau.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wkxtpqri.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bkuqrsen.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3djlzswea.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gpkxxeey.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3slirzpsn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ibvlrpsf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3imbyagwu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bdkqkdst.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mecqdfqs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqesgua.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jtnnexoa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ozrktgxd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3imbhbrgh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eaywacix.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3oshkpwev.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3irzmgmgm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbgehzng.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3covuaeaq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hrtsleje.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsktbvlb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fhywowej.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3giyulyiz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pzwgcxgu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fxwqcwuy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nqlthgyf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gczaleqi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3yfgtprti.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmhuuzlc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jwaiglzj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jtwdabih.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3svkututp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ehzkppef.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3auejwzgc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pyrgholo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nehkkafr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nxrobyxq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fayownye.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qloisqxz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ixwsdwhw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qrwhsfpu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ajoktote.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gdxebnjz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ybfyegal.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3thlnwfgk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zghlovgl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3buqqlgar.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bfloacyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3utigeojz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nwoxgsvu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbysevs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3clcgkxsr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3szjbitus.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pfpsrmmp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3cyudbgsx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kvwscegn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sudouvca.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftkudtzc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rllqrbjz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3colimswe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bowhldpd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3txktayuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nurhqggt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ihixgxfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mumrjzrw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3snotbtgr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvxgqbn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3djyzzfei.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3igoovbgn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3knvhxspd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yrnvytjz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dieqhtki.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddgkrvbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3emleuguf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nbbxqlgh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qbzkonjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgertoir.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sivgviti.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uytzichg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lskbcoky.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uykqlqsx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lxyabeoh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxqarftk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hwtdeqix.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3phsamxqt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jszbhntt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3amrhefbb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ehlwpnqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ytbnavye.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbczjzu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lsjzaaah.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3moxvccvi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3thlkvlbf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3datktogb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oazynefy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mhfhtxqi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xuyaoien.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtlvmwni.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3orjnuuik.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3arotzecs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftovzrvb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwfjnjto.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ymcqqjca.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3spuuwltg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mrrkglmt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzsvdwxu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aedjniot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vrfzghoj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kcoazper.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlhkwlfk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sgefncud.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tdfuytzp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dpowsbsu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fvprcrab.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hqgcvdvu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yyinzapw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3slmmbqmv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xbarapqo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xtzcivpb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lqcfysxe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xwakcozw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pggyeeyt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cohirlfw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yyofuswr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ezvhoqoj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vuxqlxjj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hpkfqtrl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fkztvaur.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dqabcrcp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zupzfvpx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qghffmje.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kquqfaoc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bylhpoty.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ydzkadcj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fbcvanqs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dkfyrwqg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3stknlvwc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzjegr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3oqmyvrvo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tuckaksc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3srtaxxue.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iptkqfbl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3uxmfpvha.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ugqqawht.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtjzkel.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3yjvpcpph.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ifnsfrbl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xtlnnbah.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xppqkjtv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uydjatkh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uqrtrqao.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sztigzbl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3zpepvkzh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ntyhcxhr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezvfwmen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phnshpte.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jbwfnret.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnjkapbz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qkyvozvg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ptskdler.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cajukdgd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3whjznoam.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hitmmdyu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tdqkvbct.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3figoodwu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3eonguloo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iywuzsbl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qqanthki.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3indnqgbh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vavfeoje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lamvmgzu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rixdjizh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgwlpvyd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fkbddjdf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3scoyziwb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynsidxcl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3pjpibiah.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ufjrjgja.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3davgdzzn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bslzvwkc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wcpgwbsp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3dhnjbpta.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3mwhkrawb.html


<!-- 参考信息 -->