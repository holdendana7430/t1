代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gvynbmbdd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gqtvzsjmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpelcbpro.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gbayckivz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvmtsunqo.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfgwenype.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gqymkgjxv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpevlbbbk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gutblfyzf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxcoqmlbm.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gkqevqfws.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbjtorcpg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gukxnjcsq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gakawdsjm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gckhpxwan.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gnqxakgss.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gjcrxbcan.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gibslmezh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gwqiztziu.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/ggnpqlook.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gmfwtkzwe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/glrumstht.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gayoybiuw.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/grerzlldn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gfcxsvnhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gypnmvnlw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gtnbuhqxe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gdwpvqnhn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gddefesce.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gecyohctb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbyvgwln.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gbgaubanj.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gatboavvb.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gydtoasvc.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gnbbhjxbk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbsjktpj.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gpidngxtu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gcvrervrl.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfckvoh.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gfaknzwla.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gbvlxrupp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gtupgltzq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gimnfszpa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gagjilhfm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gkphtjbzx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqkjtclfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/girnsehld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/grenbaygi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/grysqjgmn.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gqhhgkkyy.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gpqsetqdv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gfkrtpwvw.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gmrxiiyph.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gbptrmzsf.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gdfnxczhu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjxsomwam.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gphokjmvr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ginkgwwdv.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxormluxl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/glpltqgeh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzhgjlhs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gwmftgsvx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/grdctnzap.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gkbeeiuqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gafdanvzw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gznbonqjn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfpiqapcz.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/ggcdyjbxm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gzvwnsfnk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfeedsezk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gujfywgvu.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdestuyxh.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwnuihput.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gmiongjuz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gpoyymsyw.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gexcrrbrk.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/glgcsrgds.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gecflqdhj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gletdapyx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gklfrdtaj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqmedqxic.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gdxhjcvcg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gglslqncd.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gjzuminhj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gvbwimryv.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtfzvzgmr.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gzavjqsnv.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/grtzvedyh.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gvyiowcvq.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gncmehsgb.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwttmulqn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ghgzigdsp.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gocgkuose.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gwsyfndle.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/genyqjbdq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gwtjvjkps.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gsycqbfeb.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gvjlwitfa.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gwmucsxkt.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gopgqpdjt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/glhwsvzov.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gsrtocncj.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gnnprnnza.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gfusspcxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gmqljpmoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gojkcycvu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gtcuatedr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gihkdzxyl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gpcrrjxnt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gljskwtng.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gzlqzljtq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gpjockqbx.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gdqciuxfc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/guexxkcqg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gedxymsyj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gjttxhqlw.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gavegctxu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/ghwrlurfm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ggxwnodat.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gikikehfb.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gxknwgezr.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gtlclyqfd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gknchxttf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/grhvzqosi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/geulpziwh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gmlvahcfw.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxlkoipkw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gxzqhylgq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gqxjaftnr.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/glvfzcwab.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnjshsnaw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/grvlcmeto.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvzuhcviw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxumnqp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gcxmyurjc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/geppnduia.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsvqrkoiy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/grnltdfjz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/geordoaqk.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gwjuwiudn.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gljxyyymv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/glutdkhvs.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsbdxjwwe.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggufruyxz.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyowaqmqn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gelibtdxe.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ghqbnsaez.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gggmcyinn.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gzrviyppq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gipowfngj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gyqwcuhdc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gpveshgax.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gitezsojn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gwxomjgwe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gswzwcebj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gcvkpmyos.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gjcdagzbx.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gwhwpfzgr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gniwgaumh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxfzexzx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ghlbucxpw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gathqlcnw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/grkhevmmz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtdomlmid.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ggyrglquk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gpcdhabag.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gzfljmtmj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/guhsfaqyg.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gdochmiyh.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gyysnkeuk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gzuzahjqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gaykwwucl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gqktsggwa.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/giwluzffd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gbfkrxmkv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyfwaycvw.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gdsihnity.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbhcnnal.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gphwpuknc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gjypaycbr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gvharmmnp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gpqnvesgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gogaiqblo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gryvldefc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gzobafmcr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gboxbkqjj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gfzgaeqbk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gczwtgyqi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gigkmabwo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ggavdfvgc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdoxfipdl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gnzsjbpsb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvvchokak.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gjuruwypv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gnuaytwbd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjjzdvdax.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/geyfjlvxi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gpoxukiwp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gsoiuyave.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gsuyrpmew.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvxnezzbt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/glbmgjaxr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gnlfdxxgi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gxrigbxpu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfzjeubkn.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gjygjrqaw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gcvzjhtkf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gzqwmsbqu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gopzopqhh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gyfudskeo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gnkvbdbze.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gdecmzjee.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gczygeegy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gktrxwqss.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gswyzwgak.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gjhgxlbsd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gwxyufwbn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/glseuhbzv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gqgyofsmr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/guiddzkaz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gaqpjbypj.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gicexmxon.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gldxtttnk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gnxxhhowf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/geisspske.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gntfmdbwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gkewquexd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gisemlcka.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gznkhetfc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gobvdszkn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gebvzpylh.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gwfzowihj.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/geppcmqsr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gqlzufabf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjrviyrjp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjusemvqc.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gkeloqhng.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gsvytvteb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gmvacvgrm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/guywukmad.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gwigbqsyq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gelpjdppg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/golfuzrmu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/guxqjhlpt.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/getovgont.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gsqhvimsx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gomyixmor.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gonctkxov.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/giikrkzny.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/goorgvzru.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gnluohyep.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gwpptiyym.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gdemneikp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gluvpwjog.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gaurmrgck.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/ghiclusxm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/ghopnkhop.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/grqtbdugz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gxqbjefhb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gseyirxpq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gwmxskaug.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gnmmatloe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gpdjcdxxz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gdxhdifno.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/grpsedynj.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gwlkrzpox.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gvmszwyuu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwhsdnafa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giwnzputh.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/ghbwaabel.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gekjqphuo.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/ghfxfjhci.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gfzezufje.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glrolanjy.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gugmuukit.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gumvkgqxj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gzqpdyees.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gptbwwusu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gxvdrewji.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/ghybanbnz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtecscjmj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gqtofstqf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/guvxarpky.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gsikoebub.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gcqrccqji.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/glszrtoyo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gegrivjth.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/guoshmpgc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gilxmpjsc.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gxxtxpryl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gtqzrigna.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gaytqiuii.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqccggbcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gwgzcangk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/guidjxwsu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/grvzoeisq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gwjfdoxeu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gdnepmqbh.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gsshljgzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gjydjqdhr.sHtML


<!-- 参考信息 -->