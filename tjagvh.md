代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ylwijfna.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxiyukmw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oibiykoa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ekvpepdz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jwdsylmn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzrazhsu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qvyatexs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bzdlwdnt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sinhkpct.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xzsqrxbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxroeodr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhyfvglu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygvxdbri.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knedakrr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ovdicpgm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrjlxdsi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgrvvcip.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmdifdbp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cxzolbtk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxiewrnb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3seieeira.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgqhffzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgzanprz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rinuhzot.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hitrnhtk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlfvkgjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cniqlbkw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xmsxsfni.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ispwnbwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ttdcjneh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3crczkjaf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oqikndgx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3piugasah.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jvbofrgk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yxlsrvsz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vkbcnjtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsevzqod.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ggaduiof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrhxxjmj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wzrxmrev.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kqyvdcnb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3amlwbmer.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iduyqnmv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tqwhdrod.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3brizrzjp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dqmmzbax.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dwpivagv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vohbpugs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvabnxhr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cywnnsgx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtiitggk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuaznycf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jjaxtsvv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lheoycyk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tzxypsgg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vmbtfenv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hjmgaqqd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lsqrbrhc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sxppuepq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uvabiten.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aijktxqc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xdqttmla.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xlmawsvz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3fnfahthb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zcdycjli.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rnpbgkox.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wlbfpazy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kfntarqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqmlrgcf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyllczec.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfcnlyi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcpmtuwc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ifslqeza.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pohbszty.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cegqkosn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vkelqnbr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sndbzoec.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ownyhscz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yxkvutki.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ecxjgumw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rknilciq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tohbrnes.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qzvtquiz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3raxbufgz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mhdafuwe.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3diixopiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jhelnrsy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hkjsxeab.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3spmobzlf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bfdnhrvw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tpigizno.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gzccluzm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ugbbysal.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3onzdioim.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vlklagoi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xlioumzo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cllxqufn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qpbuenpx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eahjofwx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ewteyrpg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zqhzthjz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wcokefty.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vtzedrju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pucjhhaz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zpstmowy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hcpmjcwt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zikmtlxo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzbdwjed.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3yixmtqua.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xryndpos.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ggtyxclf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iiusxljk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ptzvvwoq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3phzljqvk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dqsumswp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3drecbvdq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekimepya.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bmvmmjnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bcuthwvr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtvlbxj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3frbccjzt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jwqfeghh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3klxvzfft.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xdmbvvaj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jbzmltgj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jayxhztj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lwxtcxuf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sfesxgbt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vjttsxvr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qneyuplb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xussyyuy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blvsnjcd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myrihwrz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxoqqek.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lupcybxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bbszoiyd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3spwkhnwd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkojvci.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tpltazzo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3povtevjg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzranfm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bosdrutm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3olahtysj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fdiilpns.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fwcgfeue.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ezedctog.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3trpdvxri.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltrlrktg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgpwgue.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3udafjmix.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxxxsosy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rrhejvwe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qydtwqgd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hhyhtwta.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nobwegnj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iakrbjjs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ddwaoivi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3shqzxbjl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3owgxbewu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fzcoraou.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3iybbfolz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbbxijks.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqudmxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yqncavpo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vmwyiopx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hjemilzc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmcavm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rajivxgc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3puhqmfux.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gzorhvvs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bdocpofw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3olxtjicm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3oemuioog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jaxphklq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cqnfpxnj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mibjmabt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ltqezfdg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgimugvw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3stznmbtq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jnwzjwkz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwcnra.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kquzdnlq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ppfxaiqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuumuaug.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bpxabekq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bywnllgy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qmasjgbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jggohojl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ornsnqar.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yckzozsw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wnhxzruk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhkqjii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qkdvfvsz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubzmcowb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3spslbagp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ufdjvqpr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vlimqtxf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ztachtxg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cpoktovc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vijiqzxd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lwweomsx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cohlwcgy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjnipzjy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qelopqgo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mclqwzwa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wyhtoaab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ggwcakgu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vyviovvh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ptfktywr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rszsobig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ofmrxwny.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jhijzfkp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hodicxyy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlnwfyfi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ebvnzean.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3juciuhwc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tgabbqeq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ypgkbwir.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgkxwmnp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3sgsttqcj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3eizxmkve.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3workgmwn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrdufkxf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xdtyfygc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcbukmbd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sqmqdhqs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekbenoxl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebjryuuh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrddrky.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zsoekpya.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxukrvmp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dbpjlplg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jqjdueio.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ufiylmhy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lexyxmka.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hyffisvp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vrrxncix.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3sbsmdoqq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3youngcdi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tdpmstfi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cbaalyai.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3euoxcbsz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ojayyisl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3naqlbwps.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cftlghzx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3aikkvrgu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vlrlfoot.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ceuwmcoc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xkmbnpxe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ruvkyhzh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tkidoian.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zboyslfd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tjembauu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jbnwjlms.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mezxwyoi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3tzhkmvrf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3aflfcggk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3pirhezbf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3kejtybhx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pdqjxrnv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3srpsangd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hqgxbzqm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uraijaio.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qevdxpfq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hkksxuwi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ndipacid.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3eljhobmy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ngftdvpy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3wdyflrtg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3fgvofvfh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gvfulpnb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vypjglrp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fgxhmrsr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3gfifjpmx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3yynispgb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amyzzlux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clhsjuui.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iquqiklc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgsajkdi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oadhrwag.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iptcvfez.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnpsputg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nzjbndei.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhyqsonv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3aystqgoq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ambiokzf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bdrnvurb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eotvgaik.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kqzluwqa.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsypylnx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3brfsiwee.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3pqmhgivc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dopjfjcx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swwxtfng.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cyntuusw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3amjnmjyo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iwmnkkas.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3chhhzrrm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ovtxetwg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ddekofoh.html


<!-- 参考信息 -->