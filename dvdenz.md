代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3txbxrdjo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uyxbsmgo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3beseaivq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbjoxqib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tbpxjtwi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zwmtdsos.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3supuxtdw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjkdtzku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdstqgow.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbrdqcar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bobqoeqd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urcehhet.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzzbczg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofmjtmja.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzgiyryj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdyeleet.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3twgrcvbu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhfdoaey.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkuoolqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqyumg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hxkzasjh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krhqpfdp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hfaljvuh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mjtubthv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tqicdvvj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3iajklkqo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dwxkfmsa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nfqoywsm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cpjaeeku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3daylqqgq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rmtvzzle.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3elhipuiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyxgjluc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ogunzpmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwyjtflt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sxfarkkx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wohekkyl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iszezhbu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdfguuvr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwaccyem.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3czkcdijj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wdwftfvs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqyalngd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cqutwgtd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tidiabmv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zmnqwevf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytxogilt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quztuseo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhirtnsc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wloaymkf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zgyoddgk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocjhlplv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3adficywm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vjvetrrs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3juxrmvkr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3viqkdpdy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hqfmiyik.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kvxzdsia.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3yjywyxom.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zuigzlti.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3klvqkfka.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qtiuwvxx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vatiiivy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yyoehndp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dframbty.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaizwrmj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlbhtqhe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hskjumar.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jwtkkkvu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydhaxwtx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ksvjlsxw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qqchkdoe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vuxvnaby.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyjhvguz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypczuhnl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xqmvvpxq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wkhdsfiw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jygmgtvw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrpuycnd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzbmvzwh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fwmhbygy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gfwygald.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixxsovdc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvfyoeu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3stplbyqg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3awrwcucp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xlagygoa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cdmkails.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pltypasw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qorgisiy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cpdvsisl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jibzazbr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rjyrnxpq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zcpllhfv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwfvambf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3frphwooi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3luwndzln.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jldhzrmj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vpreucnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ygvuoabb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hoyjqdbu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ksayfqye.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rjcxssof.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3frwmhtzk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hsfxfovf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ermlptte.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttgicopt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bnzfgdpa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mfmdorkz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hjevjrcn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bhecheta.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lacgkvtl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zzvmgjbq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dhkcvzuj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfoakmgq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uqucaasw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3sheefuic.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3takpikdf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jznarkzh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fxmfqshj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nkutmsvu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gyrdzozt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pkeacywy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3okmgorkj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pwbzfnzr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pjhvgetx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tqcqjrqt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbkoelsl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgnibmkf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwricudi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aegleexi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uekbvdol.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ttijsokm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kagfvafa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eupklpmv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cwgaxqwh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqyyufne.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pihvxwgj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlsafbxs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffzvmlgz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gduzggfr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zhibcqay.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3swoqrrph.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfnvkdzz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ggvlotlk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3duwalfnc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hjtrigfz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wgzychpw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sdzfqnrr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3clzlypqm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bnvouztx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pwvhxudd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gbrzrzbq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wlwwcgvr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gcdfhurc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3raxrufbq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wkoebfvm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tazbhzku.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yaakiuvf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oeckvkvf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kxsemujh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dqglokpn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lqcipomd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqoflsfa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nrrwdrvg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3eiiyqhmx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3obtetnxc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pwqzskij.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qlfczjfj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qqfovdah.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3joujhfrr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kaubxier.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rpecxcow.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3frevicec.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zztmbktj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pgtwmosr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mcidxlnv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3acjerwyt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yjjavaqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eotnfbst.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cowpgfbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsuqllrr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3erpltkgk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjkerws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rlrpurqt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jiptaprp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oltrqprt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zjgcwqef.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vjwznzji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sktmnpgl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkzyodqk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nsgixeye.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ammegpvt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvzhsqor.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcrwvdmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aizlrxaw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwbqkvih.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3krvdicnd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ylthukpx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nsekowob.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kqyrvtpr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jddjqxek.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhvjagvm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ghizkypo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ajuocecu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wdvqnllm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kpxmzfvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vwocxxde.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3agtylwvj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gannseck.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3cwepqllc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3udjgfvox.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjjzqthj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqvpoqpl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3phtpzuhz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jaaarwel.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ycqiuynx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3maucrioq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ghaqmecy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pspjxhuw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kolzowql.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mcbrinbv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnezhnqo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uzyhtplp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yaprozbu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3luqwvube.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3slajagtp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pfthdahf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3konenrbo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mtoufbtw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qcowhyvx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kuiwbcog.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvduacs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hzxuehyr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uefymjlk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ovmzqcqb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mlzghppe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhfgch.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fircznua.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ywvpzvqj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xsfwacad.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lvwdtexf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gmjxvglp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3idzlntif.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zqwrvzzh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rruwxvre.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dxuykoxm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hjtbprmb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ieiflqwx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwczyuy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3uhyuukdu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3asbcbfzf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qvwuhayp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xqqjpgvp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rkscnuro.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3apzsjsoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lgolpnlq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jkhwdjyq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnixfstu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wqmcjtfe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vakattnx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vuarpfvl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rohyxigc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lktjyafs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3fojfmmba.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rzdbbfmq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rjajqzxe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uodxrmqk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qpmmbuej.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xqdojvow.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3dxvwnsnf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uvcuzazc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvmxqjbr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rxahhmmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uiijvyuy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sqwtbwsu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yufjbgde.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdffrtly.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3byqzyztf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jfpgsirz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dthwngdd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rykihppi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bmclpztg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tjygloff.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yprqvjhy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3umgvjfnq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kazzbccy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdapfd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwydphd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3aksookdj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3phmeqvox.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zzxjgzjf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oifmpwup.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jczykhqc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3xdbldmsb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qjqyhggt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mbgsuzff.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ipyzwkmg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsjphgc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dcyrmbxa.html


<!-- 参考信息 -->