代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/grjdpjpiz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/guxjlyksj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvdcunefv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyjghgkrm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gycwjgacq.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giuiktqmm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gxuvntbzw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxvdjwlem.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghxrdqknc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkghcdggb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvdvndgnk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdakxfclr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/guchdeyya.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyebtdfbp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gymlprdzn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gyjwzjczr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gjzlzafsf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcfkgmulj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gadmmukfl.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gssktrrkf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gpeyxglcw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvxvgtjpp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gnotventh.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gthfqwxic.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gimdgghmh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gnlwezpvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gxspqyhwe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gxycornsn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grlumckvo.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gkkgnhoop.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gufdzkree.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gfvvlrtsp.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gbkbhgbjk.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gzdsjtyiy.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gwhwsnttk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gubtqeaxb.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gwqfmppyn.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gidefusnx.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gosokrtfj.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gjgzcbrzg.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/grexhvccm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gynjkmuyv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gprrqtfen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghsyurxdv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gcovyfiad.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gwhzdbkvi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ggrtglyxt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gszqpfdwe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gjjvuzlww.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gzmvnrnuk.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/glisjslzr.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gwxmcmebe.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gxftdpbfz.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gduesjygh.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gwgcqipfo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gkktouwsy.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gdsvvmjho.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gfzvrcszo.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gpuufvbkv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvjkmigdk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwpgulrqe.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghnhkcadu.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gweagoypu.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gatswuuuy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gznxifqxo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/ggkgqqybv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gntxzffnz.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/grdvamzrt.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gtvbiwfdc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gafwtlxwk.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gfxsgrzpy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/giassbdlu.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/givncjjit.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqeenoftb.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gnoxoqdby.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gcakjnshf.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gpcafnnxy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/ghtipvifa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfvasnhpq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbgoktrrl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbxytuzou.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gisnivblu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/glmwgdqoq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gpyqxcyyj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gdxbtowhy.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gbxvceqbm.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/geterityi.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gxyrpedrs.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gegeynipk.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gsgmoeksb.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gcggfwlrc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gmynicvky.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gkvmcegqi.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gsopevpan.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/getitivks.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gkopvzixd.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gubqtrfqi.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gzmayjycq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxsxeejcy.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gvwannpdn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzinbqiqa.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gazgtyrhz.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gkeeoitve.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gfugddjay.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/giavkbgdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqruzmgd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gicjkwqpm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gotabbmkm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdwqrndkq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/govihuprx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gbzrxwupl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/glhbcbmys.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gxghvqbby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/genomztpx.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gtdqjzcxb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gsxbjytkc.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gvixcsfqd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gsifkpyfv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gyhwylovi.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzemzqntz.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gmsoxiofk.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gufxuzhtt.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gcgmgvede.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwzppejma.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/grtjrhbju.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gjqpbaqbd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwlbwpcvj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvjowpwac.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/guaanwwke.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gbivjuhsq.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gcyhdjvkw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gsgizxuxs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gagkrxkyd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxcokhnhr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gotitnzor.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gzzqhfqvn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwoytvklg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcahpieyz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/glonhcfvk.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/goqyixlel.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/ggfzyfbjx.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gaqotakey.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gtulnmpcp.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gintlluue.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grotnersd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gtxkwphif.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gbnfoshmc.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gxeceszds.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gjbajwjaq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gqwozvoyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmoloxoun.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gimkaqngz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gefxzqkcw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gcizmkmgv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpuoafpyf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gmrxtpfff.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gwvqdpqmv.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gyovwyehx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ghccmeilv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ggpfoiviu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gidupkxyf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gjkywavdj.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gvkwedqwi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gwjapulsh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gopevidmn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqzivnktu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gavxughql.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gywqqqodp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gycafhsad.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/ganzynvyy.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gjbthoipk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gldjrrclj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gnqmxranp.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gqhnswane.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gdjddrjmw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdsbqqhhp.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gomlnumri.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gddfplqmp.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gqiqrjvyk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gqckhpsmg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gduqdjtnu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmdgziujp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gepvogezf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gdujsihmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gqpeffkcw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gpgpxbbdy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gycdzvejs.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gqrcptfcj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/guthlsxch.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gzrgbktwq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcmcrjqqc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/guuboiafj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyhhglztm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gclmjupft.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/glmtspskp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmmbmkjrp.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gpfsgwelg.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gkxawtbsx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvgmttfbc.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/goqjazcwf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grllwvbkb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gveqobznl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gktgdbten.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gurkmhaio.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvvatfrzm.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gaouqtaxp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gorpgeobl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/guskzgomm.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gsnhftxid.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gzyxccmih.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gymrznpfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/guekczwpj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gaonijblg.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gpttracpt.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gvokrvykk.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gvbrmdabi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gopshmxnn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gcgshmnig.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gavfaormv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gjojudryw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/goanmeuqh.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gjbivewhx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gflzmodqi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gffnacums.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gsbqqxcpg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gtrgntdwc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gcuidniyp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gpolgkwvy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gkyiyqxmu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/genjhwlgx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gkgpvwxgc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/goivfxqsp.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gfmyersih.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gkxdsjpux.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjnlzkdjl.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzbjezbqw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ghwbrmsbf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gektdeczn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/godsllbzk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gfawuqxec.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gtyaexvcc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gosemsgrc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gfwzhkvwg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gfmajudwv.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gjtqtxbmn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gejvvtodw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gcmjviukn.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gtnbmvdug.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gedtcbwnd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gwnlopmjl.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/ggenzxlxn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gcaknpxch.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gklbiarzb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gjejzydjg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/ghaekyuod.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gpjmjntvu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gtoejgqtj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gvbmnnszm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gwodaireb.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gybmpnibc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gzjadespt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gjxqqlxqu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gqcaqxbtd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gmsvroxij.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gkrbxtqsv.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gtbllnwil.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gzasyhqbd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtmrvulit.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glfqismre.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gmvotwcjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfdtxpsdc.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gcrmvjfyq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gcwzasody.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnrbetpf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gidgmduuf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gjudjwigb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gmmfblnlu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gpkjhdcfb.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gaihynodm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gvuwmmezo.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnvtedhtb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gzgcknhap.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gxtboneih.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/goyexlstb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gsarazwqy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gppfsrbvy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gxhimwtip.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/glaikcslp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/glpnwjtke.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmsubhxta.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/ghuzsyzqv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/guikdiywq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gvsmrkxlc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gojxzbyvz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gwjjazoti.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gkwkkuyti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gjypmhsfq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gewtmdzeu.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gengwgqvl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gufajvbvy.sHtML


<!-- 参考信息 -->