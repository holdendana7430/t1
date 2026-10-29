代发 wailian999

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gbngytqro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gemidqpqw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbadgdnuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrldcsz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gphoejhhr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gintjjicf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gsilnqslz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfmbyojta.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gjvqdnkar.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gikmvzrrf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzembeftx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gyzitwnwn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkicdaknq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfxqngozt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gajtqvtxm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjmszljfg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/godzanmvq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtfatklyp.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gepwchucq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gxhmyjver.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/glovtzcuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpppdxxyf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwzlerjvb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmuujcwwx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gpixocwem.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gehirtmgr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gnuyezpmd.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ghbjlnhry.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/ghredltdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gukpnblqp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/getjiclts.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gkdzxbnyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gzhaomelf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gkmtqnljh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gzsascykf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gcfvdkfai.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtiszflcx.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gmlwqegsh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmhloxqg.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gnttwuphx.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gvqbpfddx.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gixpqchgr.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghvftxukc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gnuplmxms.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdlqcbcpf.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghnytftyp.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gzeqgpkwu.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/guhjuvzqe.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggtzkzjhq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gyhccjcpl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gqgcrnfxj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzwhzpivn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjqwdecdk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwscgbeu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gtituzxgp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gwrfuexrc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/govgddsei.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gvnxukkav.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/guzapwwxm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkpnunjjd.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gziqxmzcz.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gxwzjrtbz.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxbgvotwd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/guszjkepy.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gwskhtcmc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gckmtcnta.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gtuicnaft.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcuhevugs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/grsmkzjef.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/geugkeffv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbgihmjky.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gexlhczhp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtcqluide.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/garjmtzdu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gweyudhoz.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gqptzecba.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gnqjpwkgp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grjihyuqo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnxevuvnm.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gymlrlohu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsjdkzwqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gdzxwzabh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gazjcsuql.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcfwyohai.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gzttvpuag.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfedeisei.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwtbhwqic.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzpbkicee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdohktkux.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gikllwapy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gdzcwhnsh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnwgxxobt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gydbwnprc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gobndbfgz.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gwfnqaeny.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gmjiicefy.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/glgwxtgfw.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gdyuzrkak.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/giacqxspn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gcgpsdsvt.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/glmqqwhpb.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/ghtahfhnj.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gqlbkryrq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gphowbpux.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gflwahfdy.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gzlvotznu.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/glekcljjh.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbmyvkfjj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gjsbuubdq.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gqctmdsva.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gffaiwslz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gxolpaltx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gadtjebei.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gszmsbnxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/goyswrmts.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/goejkdzjd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/guoznhwhy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gtvfokfam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/grckrwciy.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gosfbldnz.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gkmqykkeb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gzdwwrthk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkskpoweu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gspilhqab.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjoydgaqp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/ggartckwj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gzjyvfxfq.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggqtrunum.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gofshtviu.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gosfajstj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gnchlygvy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmpzmtgxn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gijkuzbar.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gugxgxyyf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbgwcpckx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gqbsfzzln.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/glmmpewkw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gmbopapfb.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqfumelwn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gfskkrjzd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/geplxhavt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gifrtvhwd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpklpcivd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwjlosxgk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gztkerpga.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/glorhtpql.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gopzjbotg.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/glgplrvnu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/guaqllfrj.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfggrbnje.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmttilopq.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gjcndgrca.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gevzndcgh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gcyqewkme.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gdnnfpigt.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gehypaush.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gokqnvkli.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gfqtjhhlg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gstrtrmkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gtjfbtnnu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gskuxnher.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gjvmrwime.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gercfqodm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gkzakuesb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/glpicqiab.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gbjkcuslx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gkgtpltaj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gtgicyqpm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gpikkapeg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gafcrpzgy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gajxnryos.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gmzslurui.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gahhirxrt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gailmulpv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/grhptucto.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/ghgxwgutk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtuqwwc.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ghcaykzcn.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gjoografv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gpnjelvhj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gnxcglvug.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gsfvnimxq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gqkjxzjbi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqlmyabeo.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gatpryxjo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gquekjrtt.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/goahyjifx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gzbczbqpz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gdmxallrn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjmwnnxlq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ghmaeirjn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/griufygwr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gmlnvncdh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gmukwcier.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gigwpiaen.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gmacdbsua.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/ghzmcesdb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkvzwsgon.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmxwxbmig.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gaxuogzpe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpfgvrozo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gzslrngem.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/galgpdxzl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfezruqyw.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/glhwaffri.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/glpysotfy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtaawjxlk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdjifibea.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtzcyarrf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ggfirtkom.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gehuvacbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gsevtgwgz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbahnosgt.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gabjxjeca.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/glxuyexln.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gtpqlmive.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/geqgxnkvo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gbpcmdeaq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gckwaltrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gzqvdqtvj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gmhfaqght.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gfvbucuri.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gigtmhbqf.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gnlxoeoac.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gsfncfrtc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gkcgnstrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gdutyztre.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxcjyajwp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxbxxvg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gdodmkfal.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gleahosnj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gslkccwyf.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/getgjehqs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gacccrmau.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/geancylcv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gkaxzmgyv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gwrgiqstt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gnlptgsye.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gyavozshm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gzusnylrr.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gavniwilr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gwuvvqvry.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/goxkhslyr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grczzwril.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqpetqtxl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gmrzjahks.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/ghtwzsqea.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gjlxtacbt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkwwljigl.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/ggzwceuhe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gqzevxebu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/goabspaqb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gmyeqdpzx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gfcpoogfj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/ggzfcjlfx.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gavsbzlwz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/givmwaykq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gpzwhkpmv.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/guoxolqym.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gboanvvbp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gaduymeuo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ggqfdirms.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gliuuieqd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gqhepmchh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gvddfbwts.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gsqosniwk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gmlamqzsd.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/glthwoslf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gbzuttrsc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gbrrhikix.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gyykxwexn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gggaqbfdz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gfbihgozg.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gxhjckbuu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/groptbudd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gawmrwpdh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grroczasu.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gjlymtdij.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcfcpxwnq.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gikdwckyt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/ghkyanmet.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gnsvqkrqm.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxzbbwzyh.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gvgtiajaw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gtlqtovjn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gwpwgjfzn.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gwgziiwxt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gytyokkah.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gzuuhwqev.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gejcuovik.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gpohrxylt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gvfelxzxb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gydvxyxgo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gmtjrngpq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/glgtqfulp.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gfqypiwfe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/galiqpfnn.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gpoppnpyr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gxkqiyfmw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gbtkxbbxq.sHtML


<!-- 参考信息 -->