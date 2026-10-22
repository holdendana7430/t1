代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieufrvgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmntzsqu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rvfwuxmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcfbpadb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytqfogcl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtfbqtes.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqhtpcmk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nibidakb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aywddolh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2liknsybb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hjcsyeyi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pnpqdgpr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dmcxbxjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2slpzllom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yggenjlb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gpolhzap.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hxyqzezs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2solyeodp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cfgvhmir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wtusuljd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agdeljgu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2evopooxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkrnzbrl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mkidqgkb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yweykehf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jbjugnso.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbxruwoa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2igeiivbp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2umgyaldd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vraqdxnr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2luypnqsm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kwroebkz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wleccrdw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xsfgktje.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mhtccfqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lghmcuui.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2krycbvob.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofpnxpaj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gzehxncv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nmrjsvzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bthwlnnk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2muysmpnv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iqcwwgqp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spqpdxkk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ipnpykot.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pdmzbaev.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wqvbkete.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vxwguaiy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lsmzgvsw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bwcxlthd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wxqioemv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rkatmvjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmoswhyq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkyxhfj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rnvttmbp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdrthjiz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dbzpzvfg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsyxwwkr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ptfzfuwm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cmfxsldm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fwgnwgjm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xqraiaqw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2egrsyjgl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2axayhdey.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2exdwyhnv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qatwzmvu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zbccatxy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjzwihyy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yfrwnnfs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vhvecdwa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eqpxeesa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dabvuvpy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wonqiizv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tshjemmv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pbevbzls.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2stusjkym.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ivszkvgu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2owfmkrpn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sjwqeydd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vivpnomo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oesyittv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ywhhizoz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fguuubst.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rasehfeq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xavpdatc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhnnafsx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lqezbthm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2igyuixmn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2juctowfs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nsgbqlgd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2chqbzavi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2eykwzahn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2sgnpeguc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ervjfizf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwfryope.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bcuclqoy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2prhvvzul.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfoyjukb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lihtpaha.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ojytsubw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hqooblbl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fmwqwfka.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2skwyrsyh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dpvzlcsn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uuuqbqgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xkmrihdw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qlrosiwy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bsctdssw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2umovxkyu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hlotipko.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jnrcudat.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yvexmqxc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hmjmncbq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dcnmvjwl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xsmzbsmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vtqtzshx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ptkovydw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kgoyeakq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tdnxunic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2twmtcvst.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gcieofzb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ctpttsds.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fjwyapkj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2biqsoscl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2elxzreqc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tagnfubt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2taotenfy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pafpbyiu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qjhzichm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ughiirvn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pqibvprs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yufoqiwt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fjidhydy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yzczitwp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ggasnpoe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2orfrvbco.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rxmootzh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ksaetoxv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pgpvstym.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2awhxrkgh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oltzsryh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vjocaike.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ioeyjfrt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ismlajnp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cplgvzem.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lfrtpswa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsnmhae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dlsrshpi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cjsvsiqg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rpfbbxdu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rlbzhrnj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaozisiv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2banfaqjn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rcrieugp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hosbtqvd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tvbqewpm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gfgfjrby.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bmirbzrw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wrpsnujs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jnmovgnm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2phxmkcku.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mtbmkcih.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sgpbmqhv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2knteqods.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sxqvcelt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jfzimwdd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gjvglcti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoknolrr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2uagoxdsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eufcgkeu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2awcstslj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nztwuesj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oqkyhchg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2myqggngr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qkcdmkwa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ztynowrl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ocjokgak.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hrdqjjxh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dhgzgnsd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2sqpwehjc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mbllsbjm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xgitxhzx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzozpezw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwicmqaw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2watxwitx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lndtppxc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pigwlkgt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kssfgepu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qpxzipme.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qftlympr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2drrkimsj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lfdefjzb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2toskmjqn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ukybjkvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnidzxe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2lumempxd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lwgthnie.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pnuzkzgg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2abjkamyo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcbmtyot.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccmnglug.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbibnunu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2krnemiel.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hinkwagu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wyrvgapm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypfpshnj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bsobjkym.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tzeprjnv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qqbsbeqr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xrrlgdqs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2buqegowr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iagfqktk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kshuateb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2howutbhs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rzyztwyd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jyzfgvjg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wxmuoovf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nqwfpgsi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zsrktnkz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2crfkvgxx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2evxoibvn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmzaqmv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2efilxtdb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aopffbib.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vdpngqhy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nkopdtwe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oncnzetv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hlmamjbu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hymsfbyn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wtzdlbxh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fiykvctx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ffzmpwxx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koanmwlg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2uvltmqfl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fphnqwhn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fqbrrxlo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2eyeafpmq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2utvwxhed.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2txvkycia.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2daudakfb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wbgtusoh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hkihbdxq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bnjcgqmq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2kudbqoth.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2flubemrj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2koyvkfkw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lpsavrxr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2msmmnekt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kgskqzug.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqprgeg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sxxpriup.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2djvdqpho.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jqfeiygd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xkwkwltb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lkcawbjd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gllohhbw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2winkyfiw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bdkezlbc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2naewrynr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rcvtznqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yicjjegp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nqyvsutw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tagwdcax.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jahgxozf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ktaflqno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zfxytoso.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2figocazk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmggzjmp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2srflnymp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deefdnfk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqpfvt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eumnklkn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kotloeau.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eezkgdsc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ezffvfda.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jxrracpx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2uzbqpiav.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ogaldyjz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yossuyzf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dinifist.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gflbyyff.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eknsfesy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hbnewqcp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xlboilpy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kvxxndop.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yejjbgqg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2sneuqkac.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yjbqgisq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2guonjzrc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2rvehxfyk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptidhcte.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjimxkjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jbbhmrfs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hxbbrmuw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rhuaagll.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rjkpyrti.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2koiapfvw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2klugcahn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sityrdjt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fldnzxyh.html


<!-- 参考信息 -->