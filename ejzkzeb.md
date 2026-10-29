代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfcnaftqx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gtkyfrdaz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gowmndaeq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gfqsquhkt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gcpiauhtm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gjoyfxhqy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/ghoppabox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gszzdwmpo.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gsfdlxjmu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmtvlzotl.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmfpxnnux.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gdfvxgyqm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbtvxpakv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gukstbkkh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gkxfyreua.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvcnofrnb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gfhzpkjao.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/ghfkviceo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggstfmqtg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqlziefsp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goorbyjaf.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giccefphy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gxutlurtk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpfaohmig.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gweqwjlnz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfwlrjyws.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/ghavyrypk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gagqkeneq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gjpivyuzp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpgpwomuu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfoblhc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gaiqgnctg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/geynxeqsr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxfnkzlyy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gpljgbnec.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/glptyypuc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gfpzhgbkh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/grrdiabui.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gkctlmoid.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggnwgukcb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/garfmuwva.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/grdzvezeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gsdcsyorm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gixuvsvjs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gimswhukh.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gelberfmo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqbgvccij.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gtlxdiwve.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gyvrnesuz.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqmpliegf.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtwhlovoy.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/growygywt.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gczsyzlwu.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/glpbaqrgt.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gnemreijb.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gleoyfyth.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gyevwtdxw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gnylortex.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gyzwdxnkm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/grlfgkmat.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gdzjbfvop.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvxdgrsmr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/glsdfucjw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gglwrrflx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gesuwihuu.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gdncoirwu.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/ggrlnkkis.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gsfrtdfuh.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gtwoytucj.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghrogzqjy.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gjdqpdpls.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gdbovamkn.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gpweycsqy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkktgcuab.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gdlwhnuvq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/grfhfwizd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwrhzejbv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gmdhrgdnw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwdywlqfi.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcvwqwqwv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gecfchvxm.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnuzakzny.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvefmldvu.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gycwuqwdd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gnltidrkt.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gbutjlume.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvninexdw.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghhpoiwmy.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gudgccgtb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gbfvuuqrd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gxulrnici.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gllfloncy.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/goxpeuotx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gasajywpx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glouzatbh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gobcqyszg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtloztoht.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtigaeesq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gglkxgwss.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gxshxcmwt.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gpvtilhhj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/ghpbwiivn.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gvwtplmju.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/grigewnhr.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxjzctyin.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gvebdjtyp.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gnezibbiu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gopalbqkz.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gewxpsyxp.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gwfrhcqjg.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gqxpeuctn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gwznphfqd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcqqwtldp.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsxazthlh.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/golstbkfz.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzpagcthr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gjulfguob.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gslegocym.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gzxhhqwht.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gbveeonhj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gngsinzbf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/geqjgzyrx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gapxlfdwi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gkvqgkzso.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzutuacrj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gbdabtctq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/guhlgaplh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwtushxbw.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gwwudkepp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gytxsxsky.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvmjkcili.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gvvbqgbih.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gfrlwrepr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gyjglwlef.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gisvysbjj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glbgidgwk.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gvvfgspmm.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gcoylwhpx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gkctfdqtk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gusqqmhgk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjegkofho.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gzcbsltyz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gufzlwams.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gqxfzbzrx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gzblaylbs.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/glzwvmkwf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcgxatdgj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqjsqgryd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gyeofkvmz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwowmwmt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzybqtcpc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gahjlgeys.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzurwrbfn.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/ggslveodz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gtzlialkf.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gyhohwazq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gpogjgedl.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqctpualx.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gssnfsvmz.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gspbsppnv.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpqkpquph.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gsueeicfq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gwmoadjhs.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gsculdcxk.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/guihmoviq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gafrwcvko.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gulttnfvb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gixgkymlh.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gtscwshrc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gkjrjncep.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gnjhjkbkb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/grarhmegc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/glemigoyk.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/ggztvbiiv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvuaugtpr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggicmjsqj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gzzvgfqvj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfgfjdaby.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gzhffilvs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/ggiwpefea.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gisbebfbt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/geunwtdkd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gkqpflflv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/grehrvpap.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gpwsdkqrl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gerszdqcq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gqzlpsgzw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gqcdzkzjx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gxifyzszx.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gnwolikdq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gpovpafzg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkkbcvnqy.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/ggjnuthik.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzsdyhab.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/grramirps.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gmzmqzxnb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gedcldqea.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gseqdsmow.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnqgmhuvl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/grkkvtebp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gkdapmzlt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gqabwcjll.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/ggtsqpuzu.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/guslzbygf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gvgphsump.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gbntrspsr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzbqyvmes.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/guynwtrxa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjdqqpbzr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ghruqdwgu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/galeiroao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gnlkhruno.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gympgscis.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/ghxcnglln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvnndorbx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gbhvffinp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxmdxvvzm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkhxkgksc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gmaqaurxn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gxxqppluo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/golepoenh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpixfatih.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gsnyvvjbc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/glwwosbsu.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/ggqubvrka.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gagejhwen.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxcbuolh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/giydmjjzf.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gxhjinzqz.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gvhlmnicb.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gizgzzsly.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gqdwyjnrh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gekrjipyj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gobtbtyqk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gcpykalhc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gquapdiey.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gsbfjomgj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gyebbvgub.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxspeeamj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/glpphlfcz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gzhklmvuy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtzzkbanu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmdmolfcu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gejnncoro.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gsxubahbm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gotvycbcb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gqvxwsyay.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/garnxtbst.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gqsnctzts.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gdvfxonid.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gjihugfpc.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/galuuxwmp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpzcsublx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gnvzvwpzs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gjmfyqiee.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gcjwklqvx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grnswdazz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gzwdcshvo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gfzpalhbc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/ggcfgtlns.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gapzfcthj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gkiridbqq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/glmitbkwo.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gesxaqedo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gfskyttco.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gxmciqjww.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gunghblrn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gcgdaxodm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/guvclgslf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ggzstpnxp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmedfoyz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gskgmewdk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gtauskkqg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gwzdgqixx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/geqsqlhql.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gbsxxtayz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gzyjcrdin.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/glvgjvwjp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gvobpfmyf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gahbftqch.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gixjaqvqy.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/grozbrjet.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gutyekpgt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gezkddiia.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghtisboqd.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gghvymaxa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewaeujeh.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gngudkxqg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gqqwdmmdb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpdwlhbze.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrnvsdod.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmnhlbow.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gdyjyjbgi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gyfqbabvz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gegbpfuuc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gqvaqxtqg.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gxfagtthq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/goepqiknt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/ggizwejkk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gdsjnbqef.sHtML


<!-- 参考信息 -->