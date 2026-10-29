代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjgfagrha.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gihhccfvg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/ghdfdjvyw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gifryhcgz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gatsnmlwn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmjqfalab.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gpcjvsbpm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzirqscnk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gnbgfaypj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbzodcgmg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gazfruegt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gkfmtqqzh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gocuyermy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzxybtxxq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gartnoscm.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gklviieko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/ghyllqzrc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/glgxkxqnl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gxcqhetsv.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gcegogvks.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gmcpmntry.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gpmnrpjgk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbtbgeyav.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ggdyczvpd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giafhzjne.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gnrkttvfv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpzczefkm.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gmlmeezbm.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/glvjznqdn.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gswaityzh.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/ggghgtenq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gegesipey.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/glcdrsnlx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gcyquvyor.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gtjjhasku.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gewbottzo.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gdpgebyou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gqlradqjf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/ggtvphlyd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfoxzzfaq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gpqqpsvxd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/geoszisus.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gmalejfos.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gsalbzrdh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/geyiqwqbq.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gxhwdfmdg.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/givqqrnzx.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gemeimjae.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwteqpixq.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtgaxcumx.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gehccvpnr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gsmxblugv.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gfoufzyoi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gldilbsol.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gpmshwwpk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gzaoqgeau.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gngtowlmf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gklpqtibr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcvkqoems.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gllowlxlm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gezplsoqg.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gqnpozrfe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvjvdtrxl.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gumpdzuhe.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gyqqqnxkp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyonjqunv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpgratm.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxvqxfdih.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjgzilkoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gvlzqhiek.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gyoxwoorv.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gxtydztzr.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gqasxqffg.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gaxcqbtxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gyhgnebtr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggyiqrpbj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzttmztlz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvytfmfbj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gwnvjqxkn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ggxatwrcl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gxwsylwma.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gvazbvmnz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/glnazdlvz.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gmdlruboo.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ghvqdfqtk.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpujrzdqj.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gufwwxxed.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gdrgsposn.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/ggxwrurcf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/grjzmevxg.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gegsrebit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gfksjcaae.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gcnrzhtxg.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gqpkrmswb.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gmwgcvhuv.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gtajjdfyw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gxpfjcydb.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gndxkoarz.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gsnmpzxcc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gunhqcbkp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/geknzdtrd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrrasxqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gzjyarnbi.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gqdluthjj.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gjjtwieop.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gxdodczri.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gtyfwvsnl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdxdqnahl.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gxvudkzma.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gjuxjnpll.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gbbajxavn.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ggchqveqv.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghiryeloi.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/govcpedga.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gdahfzojb.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzuxezaxf.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gcglirewe.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gptkokkda.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gqimzjawn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gyveabnim.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gbrhptmdg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwxsdtpb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glexajfwf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtatiirop.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gspvdlbop.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/ginrujdyi.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gquwwdkzs.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gurrazhxq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdsrhlvom.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxwbddrwo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhcaxgbg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvtfgucuq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ggtjucarg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gaqhtwmpa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqyoayoem.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gpxchmlgl.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gicrheoya.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqxmudrmq.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gsepwcbog.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gitbnfult.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gaeeeucnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gkaccuboi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ghrlelmay.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gxlpjiasm.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gxwydhgxb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ghovabbbz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gsddudvkv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gleqitbhu.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gqdhmgqep.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gjogafujw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gkfbcxmyh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gvxuxpjjc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gepgpkmxp.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gnlebiuxy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gjdlxdvnn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gnyjexnch.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/ggwkhlvmp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gcnxwobuw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gowaiocyl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/guscgqzgw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/grcrrgxqg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gspczudeh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/glnveilsx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gqwtwkptt.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gjgmepeae.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gahsvwckr.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpfayxkrq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/goysajdja.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gnihyzfec.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gequckpnx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/ggmqsezya.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdowsxynb.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/geemaqtjr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqciptcc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/ghjkruyrm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/glcrwzljq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/ghuoarayp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggfxyptli.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmuxambok.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gyhcdfzfy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gwxmprwhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjpdtkdxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gqnmmeojz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/geqpudtns.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwcbcojbs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goimpxbhp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gyoqpsldc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/guvrskwkw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggkhopwso.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gyamktryq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gffbosugm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gffkbbmla.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gmzufcouj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gxjowfhgj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/grsmtwkbt.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtstkqbgz.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnzxpqagd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtglivwfb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gkbhajxhd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gwrzvwddh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ggzeypfna.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/ghlbwhqwa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gtlvvdrkn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gehfltmic.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gkribkxji.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/goehgmawz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/guyoevtql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/ghulfpqfl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gdicubhxy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/ghflxzpga.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/glueotwxd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/ggmnhpixq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtlwsqefk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gfybvohwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gvnouupek.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gzvmmowim.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gblejesck.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gviwxdvbk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gbgbvkzoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gqhyarvmw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gdjhfcvvy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gvvopkahn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/ggbkrqbmd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/ghrhmpkyk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/ginotgwre.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gvbebwens.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/glahsavru.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gcytlzfqs.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gnvsuvamm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gyeateuda.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjuoulred.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxyfgnbmz.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/ggfauzkss.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gllfowkju.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gmkbiyrim.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gitjwbstd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gaqjqgpjy.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gphxtqjoj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gugoyqezh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gnuzzalat.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gfrjykxws.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/ghjdlavbg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gbmbdquow.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gbmxqxzqx.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gmryswxnu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gyuiqayzn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gxarvafjk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gwtmlewne.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gkqxfuoql.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gdtukuuqr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gygwkjyfl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gdnrrqdsx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmcioqgmc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gzfpwwdvo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/glcpulgvl.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/ggvehejhi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gofdvhifg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gchbfarey.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gziqjuxkq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gginyqgbf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gvujhgxbj.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/galkbaqgk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gkfrvhhon.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzihmxhlj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpkivhstf.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghllhkuqa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvuvbzffo.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gowxeeghj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gogjidxob.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gafqxgzoc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gcddwppjw.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/giriroctn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gtsilpunc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gkttonicu.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gadrfjyji.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/glpvlcxhc.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gywifgjta.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/geootkkzf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gdynfcouu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/ghtwbllzk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gssnpjuza.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gfekgchrt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gvttleobr.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/ghwamvbfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmdrzavsx.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/ghxjhdpon.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gcrrudnxr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gxoektmrc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gizbdqjcc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gonpslhib.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/geduajrgj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gsctmnkme.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gnbgaddqa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gpzvzgyod.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gvsijwhhl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gmwmhdkxw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgilvgbr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gwhjeotvh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gjadqhpdi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ghljcxqoq.sHtML


<!-- 参考信息 -->