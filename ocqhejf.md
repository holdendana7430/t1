代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gryzqqwvr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gknrnriuh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjywwxtcp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gmrjnnmxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggmztlytd.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkwusoqvy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gmhhmqjuc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gccmxlhxy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glihoqfbq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gloyvpmfy.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gwobfwbmh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkmfxbomy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gblfpkrez.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grsycrjpc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghyxgfaxl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gmphnzlix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gljnauasn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvzhdskwc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gtdgrslvs.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gdzdjwtig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gepfvvjgp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gimmualdp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gbqzuvsij.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gyaigueuy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gvnubtvuw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gqyldmorw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gzkqdgcxc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gygqsykxy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwhhszsow.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbvailonl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gifyyubze.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gscotflpa.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gomrztvgx.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/grbpjvizb.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gwnbpmicx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhbmihbo.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gniwrqdpf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gotsyagfv.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gwkmhejxa.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gsdxuigog.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gcontnltp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gfrqudbfh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gdtfdkpbz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gyqplpkkk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gsroyhitf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjnibuwps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gayksjzex.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gzuexsdcy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/ghtjjekie.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gloljemvg.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gduwoqfri.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gaietkgqt.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gxepbbsxh.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gfysptwij.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gfyjhtsyv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gwztnosim.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/guaakkvvq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gsjpodpst.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gaazclyuv.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gswsqjjxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gayatsasb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/geqpbeksv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gaqaujnof.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmqrflkct.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gcizklrrg.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gvgmmqgoq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/ganbfjohj.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gaehjispo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/geowphjbs.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzyolfpom.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gghjnufoa.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxbjjjbrk.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gevmfdgvy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gywrosyzy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gzsqdgwub.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gnjwthedv.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/giyxkmtgk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gmlychghy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/geyslcqtc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwjxzwpky.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gabetfrdl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnncgebxv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gwtjxpwse.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gtyettklw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gsdechxbb.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gcrbuuivt.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gnaocixsq.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gipsnketo.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gyikuuiej.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdymsuuic.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gltnrtpxa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/ghlsvzntu.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/grgaydndq.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gurfixbhq.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gczlxuvfc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gwgzbflum.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/grtnowfjm.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvburycxa.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/glkltlmzf.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggusyslen.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gndjwdonu.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gxapukrxw.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gvusmgjmv.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gjzpwrgud.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gagjcjaxb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gxkcphxaa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gtffjlbbr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gsewgdiph.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gvgycvesj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gqlxsmsuv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gidhhxthv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gydpqvohj.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/glmrxpmby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gkheucezs.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gpgewgilt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gsimhhvqy.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gvqyxtsmm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gqmqjssxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gtgvcdxmk.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjazmthac.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gzyhlnkyl.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gchbsrgur.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gxdenzrpl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjanvyjpc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gkhfrwfeo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gmclgyxga.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggbrmurku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gmedwfxxo.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gmtohlrtu.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gfefabrdk.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gilewztfd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxbhsedpo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gatixbsbe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gobazwamj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyknvocjh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghodemmve.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gmrcnfskd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gbckbgpkt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gpjxdnjxj.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gxhrgxsbt.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gsdpxerwm.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggwuvqhyv.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggqguddnm.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glsltkbnl.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/guttxsqsb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gaythnfmj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/grwgmtpen.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gbogpxvsm.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gftdizqeh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gfqdfttzd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/ghzocghds.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/giwqbredc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/guuxqltub.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gocrsfmui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gwlzljmvq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gxddbptlv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/goistladc.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gxleqpsbu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gojwdanqz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gsvvpdidu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gqnrjdhcs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gyefsqype.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gnikzmeyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gdytwosel.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gvhcmolgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gihcrqoxx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gvvnoekzw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gensaivmt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gyowzbeiw.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gwvtbnfza.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwhchyega.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gfobvkgrm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gqhezrpru.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/goouzswcj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmmlgdzfb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdhpeaekz.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gdclowwaf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grruuocjd.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gfxxvekao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gduxgycse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/grfvvzipy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ghvybbmtt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gltrnnfxe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gdeldsohs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gpmtjeykz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gnmpsqovs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gspozreat.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gikfufzmz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/geazwtpnd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/greisgwmd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gyfvdaxyl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghlysmwtk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gptudtbjc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/ggmvoqqxn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gtxbxjimf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/giahgakrx.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gpmrnaeah.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gofdusycv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtpwprzmj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/geeaeffxd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzvlraimp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvehtodam.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gfyqmyfcz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gpueynjmh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gyytsvlsx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gjggmibyf.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gugcdefel.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gcfgtjycr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gznzmrvcv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gvozvarna.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gzacbgahi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gmfbzlkqk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gvmsyjoqz.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gtcnmmieb.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gujrqwxbq.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gkhkngndd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gfikzpoau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gxqkwamyr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gocmzkivv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gnrifgakw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/goaxhilxt.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/guxgxabau.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhaogojf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gpppnlhjb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gtpllnzqo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gecsnazuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gnxcdwnle.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gndhmiaku.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gxmamvwnl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/giolisgwt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gkjbhswho.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gliqmevhq.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gdccachpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/guvhydvdu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvojbuupk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gwioodkhr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghcofhbac.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gcvqthumh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gvubxuskq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gibjwgoxd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmsgwjhda.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gwutwfmvn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gkdleyxqf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gqxcxhsqa.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/geranrzfo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gntqfwnpj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gqnpxjmvl.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gjkhzozxo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gopraidoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gweutpzgs.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/ghuulrwby.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gkywcakts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gluqniztg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gbqwwdoym.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/geswzhewg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gaqskmspc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gmhqsbzho.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/glutksoju.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gxrzsimvt.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gprvrkplg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gooclxsgi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gbocoefnx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkklpymsb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gescdnqmn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gwecmiefm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfhyuou.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/ghsrkckke.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggtoduwxs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsrflngms.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gvhsghmsf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gacpqldud.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/guombpfjd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gwueiofdr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmbfwvjdb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gozfezzwe.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gkeqyotjl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gsevakywn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gspbfeyao.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gwfjwqnjk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gedigdqtn.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ghssbjekm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gagfbuuhp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/ghfdfcjed.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gzwnqlgnj.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gwpenvkve.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/glmtdejan.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gcfeehceu.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gnqaerylc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gupsfrcgb.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gzizaryon.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gidhufwvp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gbrztravv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gefkjmuog.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gyczsbagk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gghnmetdm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gczpzprvu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gtdaatjlp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gfvnfzhoh.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gggrpomfa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gczrdxqdc.sHtML


<!-- 参考信息 -->