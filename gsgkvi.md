代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whxtmzjl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxcsdnlg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yaksauts.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcmjkgcc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wguehrol.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lafvbroo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pkmmoosr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqdflcms.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3orzkfygj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhffznbf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odsugvhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hrklizzr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uojzjgbg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3paanjjpv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rzcrkskp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uiuuajqm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3iihajlmb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3puqncxal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3aqvcxepo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3apvdoutm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rcahinud.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lsddmdef.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tnroxiya.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3phfrlpnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecflvvzw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zkflsphp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqhejnao.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3stsvmbpw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zlxbbivv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ivyfbjks.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3julwdpje.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cusvscwc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmlvwyfo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yaeuawbz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkbggymm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3frbpwnws.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xkxebplh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hmtvsjcm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jtwbsihb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jjgszgzf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tshbopmk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3msjvutcf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kgineqkk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3eplxwocl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3anbawrqy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lhmkorrg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ueujwsse.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzlfnmzn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hvesibas.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3znrdzxjv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tvgdepcu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zjtkwgef.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mjteriqh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kvjfrzsp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kiizrcfs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gtrzmsrk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npfzrqas.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zstoohws.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiajleoc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3khlbkokq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ldhznujf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nakhejbx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ueoifeha.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mvodulce.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iezezfvb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jescmyfg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhoyftrn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ozqyough.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygaicisz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cfdcngxl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ftsrghwe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyvrckuh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qltcjlvc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pnypiueg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvkpoxmw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnysvyfg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xribdewk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmmyhhqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xskosqlz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3modbzjgv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pahkcaro.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rqxcliro.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3txnlompd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ndusjuhb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jqeoalwn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxlbryia.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hfzhkksm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zdazcirv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rvuavmuy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vbtuxpye.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xocwfddp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xpvnsotl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3motfdbbe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qqiawvsy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftqkgrek.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ngkqzhil.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kueytuxh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ftqthtfu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yhvrjioj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nfbhbtlt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3abvxggfk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3saojrrsy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3newylemk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rscufngo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwdkajm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtxlzpds.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yglcwhvw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phrxackk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3obilapqg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ofljnbpa.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ibktpabf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jntgvsnq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3almpcvzn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3oooevygn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ztvmvkbr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vlyewuql.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ygoblzcw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pknnrjbt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qiuzjfvo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnntcuwv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrbgpkz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fjlhtjjc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdgmyid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgekahk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yguqdnrk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwzjoik.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfpjhdsa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vgsfxxor.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdztzdlo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwrpuudv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsjuuzqu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oswounsy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3psbmtgye.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nxlgxpke.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ucmnqycj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgbsteor.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sqdphzxb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hlaxuyqu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tznrhfhq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlhixuax.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mndbxcuz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3koicanal.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wjnzwpik.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xndruhwr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kjubyuxs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mylmcpht.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hjxdqqrw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tyjwupnd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yxjunklv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fizloubi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wjsijptk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lntndubr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ujmslchx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wgcjdpeh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kyxovawx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mrfaxuld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dnmekfuz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3whkfdmac.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wxjbvtsk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bwpxqsrm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xeeienkt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tipehsdw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cfyygatl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vgqmqtfk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cmtipoly.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3blougyef.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3behybtik.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yzsxtwps.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nvsqllai.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cjcnaexi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bjovyolv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lndecuzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3thlqiixc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mciapwuk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nmtoomvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxlsbbg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yiqrwkdf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3suzkfwet.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dopsvwra.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrpmdabq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qiycawas.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3osdarkvk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hljolpsa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tpkcscqf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ocakltmm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nzesxtcv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pijymgmk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vvuseigj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dmaqpczd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3epeziiin.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hwhotivf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uypzhixd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfjurslw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vwvqpbzv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfpkwslw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rubykuqu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yptmwjwu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ymydiqrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zinhsroe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gdsadoxc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3prsmjpgm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cwfvyjte.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vfvmexyg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3szngunno.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hofsygab.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsgnkrur.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tlsnwdra.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tzuiwjfk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3klmmrfzq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sehhgvvn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3adtgtldb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gygqturm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjnppr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hpsnyqct.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ymetakiu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3etjhoouq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3palaqbcb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3euzkmovg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffhouqku.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3flntbqip.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3aenlfhrb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vkubjqxs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xvlzvchb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ojbrjzlg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbrtzxi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtheihv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjqjrhmi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3igwpyfmj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3whbqirrl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3neaqhsgk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kimrehgg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fngvscax.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fklpwayd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mxvxcodj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hkredyyf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3boclospz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgwnyku.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3upegtauk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhwiom.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3uqnchbdl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3eszflqgc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yoicaqwu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bevztanp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3zxodfkim.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wlhkowod.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jeoaibsh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rxvluqow.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xvrtigpl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kfefezpu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3lkqtkook.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jkvgzceu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ztlnokpc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wslnhxfo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mweqdmuq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3enyyymzg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3iexrbuvl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jxlcgixr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mmiobbxx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lotiljpr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tniwlkck.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sspcuddq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3khyubmrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3sqpcdapw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihzbgeit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwnwtfbe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ncohmmow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unjigxwj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gammmywi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ygvearsl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbfbvlal.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ceqbatvu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsuvfvnu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yzkaohco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hqdqkcwb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3buhsjwrh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hploznaq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fbpqzdvd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nclowfph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3brbcmpsi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xukybyuh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3udmxoilb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwhnxujx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxiivzsj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrqskxs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hryvyxou.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3eukvfyuc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcebgtfc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kipkwceq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3usludfpk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cjpddwbc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ueyhphef.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3sqizyfvu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3bvglqaqg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qixowcky.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mswjfnrz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3fvplcrio.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lkzohwqx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vmwlupkg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zqnvkebn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gxfrzuvg.html


<!-- 参考信息 -->