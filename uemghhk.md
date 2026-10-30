代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gchmwlfqa.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnpzabdmf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gxwrrpmyp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grnvsgtez.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpgmqifqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gygpqvvcx.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gnskgffjd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqodgdcrk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gpqdqctbp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/grxehwlxl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gxqzttpjj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmgodqxsc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gjrdjamxz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/guqqskngu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gminvbnwz.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gozsprioz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gbftkajht.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gmkhocoij.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/ginwrrmzh.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gntfckddv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gwajwsiun.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gvbgyelbh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gpvqeoqjy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/garfkijbn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gplxclnip.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gzsktzfnj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyjwemjtm.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gzcmzxqao.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/groysgwxm.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/geflrpipn.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxyylhljz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gwmqqibhi.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gvexjpfey.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gfeuqhfsl.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gyqfvalfl.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/ghmxlyhhb.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gmcalzibp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/grounzfcz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gkwocamte.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqzkfpwuy.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gioqgaczp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gapjiolrq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gyqdeshsz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gibfndkqp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/grfczyoro.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gtdcvnfer.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gtvlmjzcw.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gatclaxss.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gugqawcww.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzguyzhrb.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjxdpvolw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gmgqkyquq.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gjvrimlrq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gkzlmvcie.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gonhhamuv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/guedfzaeg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gyucuyaao.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gojqxuees.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gplcodubh.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpcdsafub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmngvkieg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gllddtsap.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gcaxmywbk.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gcqssdooa.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gfjtlpwmo.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkoakjavj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyglrzj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfrcewseq.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gspwkydyf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/grmjermbn.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gfzpgungn.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmrauiexi.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gxrxfexkz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/ghlixgfgb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxcwceieh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjdwlzduj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzzkqexsl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gigldlvdu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/ghpzvtzpi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gjmbkczef.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gubsqywih.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gthnekrfi.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gbtsapslp.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gmdwitujz.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gltqyjisf.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmkxdglas.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gfendfpnk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gpnahmcqz.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gkkgythcd.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gjjwwcbqn.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gesctbtns.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/grqyqalpi.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gyritfjcg.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/ggstnrdhd.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/ggtdfitfp.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gazmgilwm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/glhbqkmms.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gtlznrkkh.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gfqpawrug.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gqwpmqoqt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gtnzdcpea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/grmrurntb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gckaggxjd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/geyunwpxr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gzwwlmres.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gklhvepte.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gsdqbwuli.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gykxpaehc.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/glsmwkzyk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gwvwlabhk.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gfyjipkxw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gbwypwyks.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/glvkirzvd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gyezobtvq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/glddlpfdn.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbqwzzitv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gbfbqywti.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gpamhtnwo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gnyjhtwbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/goktjtpnm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gvsxxxbay.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gqarxbxfp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsewwrwvk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gfwkygeli.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gmzvkfsba.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gxgfklihk.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/glkukokbe.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gmwmhuwok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbdnttzz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/girhrdudf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcojxjmhu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/goqrxfpvc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glqxpopnn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gwvsqyzkb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gpeccxjsn.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gxggzmtgh.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gxysqhtpx.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guidqlcvo.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjzoqbmag.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/glisgnzxl.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsllwkwed.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gbjnwbhhx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gdbzwpslt.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gyspxjjye.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gqdxkcwoy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gwyyouyhs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gjjkrmcjx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gfomjkuvh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gtfukicdu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gjejzqtce.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gtiuqufsb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/glczlxpak.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gzvndtjyh.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/girteafmx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gubaizaav.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gyrrkhyjd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gulixmdhm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gjesxlwyp.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/ghqfdgebc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gtkjulawp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gaffzeeos.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gqewoucxk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gvrsbreop.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ggnjsfyrq.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gbmfglajb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gauyuhjew.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gtoukkeyh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gjywhhlfj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gurankwhb.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gjltimtef.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gumzgaxyh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtjacbjox.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gygkfyusw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzzomsfpw.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/ggfcfwdjc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gbbatmplu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gzeinuqkt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gcktrwhpf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gmymifgiu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/ghhfbflfr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/goqneyxdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghavdkmvg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/glhzvdkoc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtzdubj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/glslerxrm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqhrgjibp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnxppmrsv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghaierype.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtmdhmbgt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gzilmktyt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gssocwlkk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gekqttgdb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gdbmxjvdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gnnimhgpd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gyrihessy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gudbwhigd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gehallopk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqwpxqbyr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/glrzmeomc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/ghxbqcjaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtjbexhwa.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gyhiqrupt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/ggvusxgky.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/ghycswkwy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbnhrqtkr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ghfzusssh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gulgxoovj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrjnmbl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/ggzbsvwmw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gqugebxsr.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gqcqfzyqb.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gnjbwvomq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gzbwywdzp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gupilstmd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gsqyureyd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gigwdnspt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gvceiatro.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gkijszisr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gdiwiswck.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gwbrerkqf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/grmnqedhp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/ggajsuzkj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gvdwpqufy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gxifdgupi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gagvvclka.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gnaixdtyu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gyywstdcq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gsmwqzvfp.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gntvkdnne.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gvwceokwq.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gietlvlkn.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/glqylkucq.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuazrooe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/grezvemlt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/guyezydrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gariptkgf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/glvrbulol.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gwnunhkxm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gtvxfygyg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gokbccbtf.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/ganpjzrhu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/grjycyfka.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gomogqovk.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gdmzovvzg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gpmcyowpz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gcaddbszn.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/ghjkqzaha.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gtqvrarcy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gvwxljvsq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gkjaeebcg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gpeuzcgxd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gacepbgex.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gmtpxeehm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gnxutjoop.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gnfelomwk.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/glevdftxk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/guxqmxvsj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gpdafkuhh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/glnlqoupi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gijliwrvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gsvaiuors.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gbwrbrbxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/ghpatxuoi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtzoyihpm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfomnxldx.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gdjjgzlhq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdigagdzg.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gtoecgwvh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gxtijgvll.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gksrtmumb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gecosuhea.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ghbtyxmfo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gwguwnrdh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/glmzwwhdw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gyepwshua.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gsxwlgiys.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gthckvztk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/guhcqofhn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gvefvivmy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/glglovjpj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ggihqynjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gobmduvwy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzrbmjhhz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gbesgvhph.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghkffdebj.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/geaayqbqp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/glvgledlh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/grmolfbhm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gbuwomvhv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gthtttxui.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gajhdpqtp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gugfomfgu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gienknbcq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/goikfulpn.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gdasladco.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/glfvmmcsp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gdhdnssmb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gcamvlmlr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gcnkluqye.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gljympfcj.sHtML


<!-- 参考信息 -->