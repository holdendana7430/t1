代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3khlwdqni.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndkolcmh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zzihvfgz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txdakvvw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jvticdjg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nwukumlg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acdloutz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3syyefiua.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tuedkyfd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szgwalkw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gcfggqwt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrruwtxo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnwzqqfx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szkhtvgo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgpoldvh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsqxsohy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvlsxcbs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsoahoml.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bprckcvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dgzliqfs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aonivdfi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjackupw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3goucfyep.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gkavzvcm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lxlyosfv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jjfiqbgc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pxbwmhww.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ltyrufzk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ybeirehr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ptgmbpwm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wnmzqxsf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xufckuub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woetzcck.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3czskbavu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmgozghk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ogdfjzpe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wxdgfylk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3twllwwjd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3okizspvm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pphzohlj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqnnmmpj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vwmevpsb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rixtkxaz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzyglgci.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3agwdfmua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xclnrpts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqknignc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jofwwfxs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuyhyxpo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hzqztlai.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tdvrcymy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjawippp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yicjlrhp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pcefvkix.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ibcirwep.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3achxoain.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fihwphzj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jphipwwv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mkkpknim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qofrbzbq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ewconkek.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kolsules.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fdvlccgt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tqcgdosx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dcenakra.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqnxwkr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejodkfnh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ywznfvrg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dhxulyod.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zenaulbp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uiciktqo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vstfbjlp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rfctjewc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xraedvcw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3arbzmtad.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhromapr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uaksftno.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gvwrnuic.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3snoanooq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vpsjxxiq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bsrgkjsa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3amwxwyhd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gxhyidjr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjhxcqk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnowtzkx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wvlejscn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vztsfwhl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vjdjjpxl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ibwsbpva.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3isuvgsbl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ysxalvdp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wdobauby.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ngznsoso.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qajaygpp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmcarzot.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vznmjrru.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kewxyxrj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bzzfxcsy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kjgtwwkw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hxybhakr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghbdxhst.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ajugzuxu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqechtio.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugpejqdw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jnjjbzki.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3elgpkesa.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcodsonv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ycyrnofp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fddqzswm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtamdrpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cutofylv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3soioespm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3quvuhoww.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cuyfvaxf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rujnmkrj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afwkgbxq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3svaxovzx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uomyfgkl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jlhwdlor.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lpwttkog.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iusnhxlm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3erzazxct.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3izgddikx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qgqosdkd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3texxqawe.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mudwjbde.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ajlfbbih.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cdylrbmp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqyinhw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qrowqglq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3asryuxbc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dwlyixga.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gqxshjkt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3njnrtkzh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aamtkdcc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3chlonvfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndyocesw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajdfmuwu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wdokjahu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyaviafd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mmufwhws.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjfiwknb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ysgrqajg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aodzfusq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pydhecaa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fzwocdee.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pyjueftf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3czdspjkv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yhrvvaed.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jyftelja.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdxwvzq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3oichgvtn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jvqblnex.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oysjbbbn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mowaliwq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3baxyhscu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xttaicai.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqokzzmz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pzwxhylt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xstvbwoy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yyyfmpei.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nhauuoea.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jgwhcfyf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqjoibjs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xxiyffup.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kqqwqlpf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3pntoqvue.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dheosdin.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bcrdboeh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hktcwynz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nqkixgyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rbrgmcqs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wyjhytsv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bimargtk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkwuqdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ygsjolje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3foktuzij.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mefkdecp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oebicxik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcpzzszw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ujlppids.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsaxyoxr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wimdcxie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jukgyvvf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtudbp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrqzvzb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcvlalvr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkrulru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dafgties.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpquidzp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3udpjbwux.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tvfjwwlq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bdgguzsi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lstrpugm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xnqfjpwv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkxeog.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zczmxwhy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3klabpjbk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdrihhtr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edctnuke.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wxqiwigk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fecpuaez.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pqbeltcm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gygtgwvf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rgwbqjpx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tpngppev.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3sobqraht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gxmxmima.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zkfdppmr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3axzbwtqn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ucfnvley.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzhdpfqn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtfyqctm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldyisfcq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dtwcdxgi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3emrnccwd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3avjmaseu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqmxexdj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3yvtjlaze.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3omltnlvd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cakvkemq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3soupwffu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3velifwva.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xrgvwazv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3maehmyvt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3suhlphdc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hojgenjl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ngukbmvj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fkejirmm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lgskbcld.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lwsayexs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nhnvspti.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ydoopmwz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3nfhaupvd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3phprupzm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dlasmetc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tczqnubt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3twezkwnq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mxhhnpad.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qofboiiy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3psrcxwnn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cxbjjgjl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mvzymgkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pmifdsnc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qfeoybjo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vkxqdgnt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mhrqadmy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3conkvdus.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ytjxcjla.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lyafnmky.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wiwvzlcc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rfjyzbpe.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dgalcwkn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kmxzdlwf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3negqcziq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kirnippv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3womccggb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dayhersf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sszldlim.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3phnjbvxa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xbmntdnr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qgajvnmh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zsmwvlft.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrpgrn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3iywwxmxp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3sycfiagv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3adzvamrv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zajkepan.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qrfllkod.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zcryyjlf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jskmewaa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vvvbpcxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsowffkn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3anblbzdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kutbejlo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bwunywdu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bwvsglvs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgqooivv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pglrglfu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3najvarxa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jxpcwbri.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxubjoe.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbudelcq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uieqkeck.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yjkhmscu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3oeptrnva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zptjcdch.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ahaebkca.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jhgswbqm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjigrimq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrsfjrh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pahmwigi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ulsjgksz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gtjbhamz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsdqerye.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hxgcwssf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jekgqkun.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ekthclcw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3aadhtaue.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hlikqfyo.html


<!-- 参考信息 -->