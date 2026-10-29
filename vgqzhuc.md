代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gskohynhm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gcewgliid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwesedwkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/ghqhhsjga.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghlggojps.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/genomzhbh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gchbmrfvf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glopmhncp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnggjzhfu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmxckpzrd.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gldyohsia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwxkfmzmn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gsasjmpou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gsbhlahog.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxdswvfui.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gdvutzzvv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gdbskzcft.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggzbvlcqe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/grwglvsit.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gbuojpmmj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/grvcipvrq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gxnntjmbn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gwqgrfcgr.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gugskhzpv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gcdzhltit.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gdrrxxqmx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/goxgbnjxy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gigeksnjs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gekvmtafq.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gafaftrpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzouneomo.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gtcthfrxd.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gifntsvdl.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gnnzrzayh.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gaqhyklcb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gqxtviobo.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gsitctyjs.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ggwoleutj.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gxzkmgztf.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gdhrmrral.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gzrxzcnth.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gtkorufde.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gpmokqpyh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gepnjmxkb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzhdtmfex.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gykbrqyqm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gmeklyxnb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gklviktco.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdbzyqdu.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gituzgaon.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gcolnepqa.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghokiqbpb.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gtxxohaot.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtwhxxcsq.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/glzhzlxtv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gvmlxqgcj.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gbcusimxv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gbqkoggkb.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gkptztmrr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gzakcyanj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gtriqnubk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvemxnzwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gzzuwnbzs.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gevresmuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gfiteiore.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gzqkuezpy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gyievdppi.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gozxkfixr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gbkcrgurn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggsawnjzw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgiezvgo.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/glltiojtn.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggasnviaq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gpiwcejtf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gfmqdxmia.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbkjsdjkg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gmsmaqbjn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gttlvwiko.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggmdgfxdl.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxcmlmxdc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbrldaqdf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gegfnwoux.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gframutxy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gnxuzxxbv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gbzfuhmmb.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gywipfyke.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/glbxnqibl.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gqlwfpifc.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gkgugctgf.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gleubmucl.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/grxddojgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gxntuyaic.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gqvpfuqpd.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/grvsmuciy.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gqwychhej.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gmvqwbmim.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gkibpjaom.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/glfnexuno.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gvyfohwvl.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ghsnvbvri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gyoyphkvm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxemtxmbx.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gmlvzvaxj.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/grbycftxt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gcaxfeqjk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gtnodmfgg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gwhdgbihf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gdukotonp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gketxqfmn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjnquiw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gihqfsbpy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gmehbzfwd.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ggjsmsbvn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gzpdkwkyk.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwvgzhsrw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/govrbungm.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/guytutlfp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gcjdpwbyb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gkoyboobk.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gbopbnudx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/grbmdmklm.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/ghivepcyt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gjehblyir.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnsqmcayq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gertukvuj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gecpnedht.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpfmmru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/geerhxish.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/ghhrhtbbw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/goabpsmme.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/ghtzvhcgf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ggtrbcltd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gpwtkuqdo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/guxsabtdg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjtjcrhkx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqlzcmdzz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxtftdicn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gidocvjza.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggnkmcvqi.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzqyucnzy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gchdnndmd.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqmjnzifo.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gyyeigqgl.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/geebfbyuk.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvjncuael.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/grfjfecvd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gcezyuddc.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gnwcybhxq.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gfnoktikq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvohqxc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gdpgcgjok.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/glfibfbsu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gurgyhrzg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gwsiyabxo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gqxfkpodu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/geekwicax.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gtvcuexkw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gnueqduhx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gxposlqzj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gwfugdidg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/guijmsjyr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqntwmptq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gpqwhlyqw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gxoocejig.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gjtyajqgs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpmzdhaci.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gobobaxwn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gyvurqsaa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gpgnhztip.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/guklwjqrn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ganmynbhs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gncwhexwd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gotehvrol.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gejthukzq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gvkjukhvx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfnryrkou.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gzrccahev.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnixohgrr.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gemuftogh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gibfqxxsg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gsdmcjzze.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gmdmblswl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gaoomtvbd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gkyupcdcc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gmeckvrkk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gnpzwvlwx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gotstcbie.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gokvxfano.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/ggvmsrqwy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnfgzsovr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gagyklunk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grkvqgcig.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgajifpr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gbxpkjlht.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gcifjrlhe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzyamdeli.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gdkewrkzt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gfmcpxluy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghdxcebmo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggmfrudua.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghmktmoea.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghsjxfsty.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gavgcdplf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gwrkoucqo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzxaxcwex.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gmoxgqcgh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gqipciiyn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gfllwxpsn.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/grehnikik.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gkzmzdkgm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gjljbzrwb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/ggfqdfdqq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gehoftobg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gcvkdebsd.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gcpdcbnju.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/ghwyriyhq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gsegaevhd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gnmcylxrd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gkanffrxf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/guzztjdvn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/glqjygglk.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gpgxwkcox.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gynlgdfuf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/ggakwczks.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gzbirdfev.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gsevvgvpb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gmworczao.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/ggwxaxvro.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gkkdnrobe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gaeooddxe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnmhmub.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gyridneaa.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gcquvgcwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gemwanioa.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/giiqqruqr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gprhtcbxt.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gbdlsbjli.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/grgdmrwoj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gzbweeefo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gtshmteme.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/geznssifz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ghqrmjlra.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/giuzaxsll.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gmqynpmpf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gspsbiefz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/geplaphaa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gpksjmrre.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gtvchpqso.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gcofshtaa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gmecqobgn.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gcqcddpve.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gezgpykxz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/geuhakjvm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gqyqgrebx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gnohizidr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/glykaahrg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gbpnsoicx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gvlsajgev.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gkjlyyjow.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gyvzegglh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gohalduzy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gdgvquvgt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzfrleq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gmdjemcvq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gzqomokob.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gahjjdeqn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/guegfszyi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsumhptbj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glcjhqxsw.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gawzltgxc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijsphglo.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gzycukfbw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbexjax.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwgkdcrmp.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gcxbobrtj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gxutlodgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gqlqxsurt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/grwtdniea.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gjoffnzuj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gajdixsiq.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gemzjjfba.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/girpskslr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/ghvbdvhqa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gsgzgcyxt.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/givgknwfy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gdrpnfdch.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gekskfywb.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/giuhadffx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gptyryoam.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/govjrxzid.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gremqlboo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gmpuagboo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/ghvpwrdra.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gfxivfttl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/glrxnzakk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gosznppwg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gbhilbksn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gnlhlhfdg.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gfnxtprdi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gtbsocxcg.sHtML


<!-- 参考信息 -->