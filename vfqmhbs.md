代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnsptamhn.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtxjdpepa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gnkmnxpvo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/goyifbwxa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzpeficne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxlycocad.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gijmmorif.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gssebojyt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/ggzaxxrvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmgabaesd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjrmnzvcd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gnquflwlm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gohrkgqaq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcnhbkwig.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ggwfwtzys.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/ghbzuazvv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gpyhdexom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gplqnjxda.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gwfxtaqjn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gfdtlqawc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gvxckszdx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/ggmxciilg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gljhfsdzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gsdwxiysb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnygaeidp.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gzztgxisg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gylzcsuwd.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gexvseaai.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/getuzbomx.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/grqloqjpy.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhqvmqfm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gdapxouls.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gjqgdmiwl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gywkexplx.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gckacpfrz.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gvgzkaxsf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/grqfqpobw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gkuhdwupz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gdruqkcck.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gzmqqkxeg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gmtntbayk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtnucdgfu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gbpveiipq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gfslmcevj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/geevyxbva.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gqsuuruid.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gfuedovfy.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gilnmtaen.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkzvwzswq.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gzkjbwgjj.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdmjmbacr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gbxvwxopi.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gzodhsyix.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gvtitfwqb.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gylbwpvga.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyikyzste.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gklwhlyrj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gqrsximew.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gocnaskus.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmcddvxiv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/grumvcbex.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmmotwpbh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gloktaitd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gplgggtiq.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gcueqdbyt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gbdylqzdd.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gclqxabgr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gppwrxeiy.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gicvhhvzs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gwrmoqjjb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gecsjyrvp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggmnqcdjo.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/guoapqutt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gidqucoit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcdrsofqu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gffnmrucp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmcwszeei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gziejpyne.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gnijargti.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gpncocort.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gfuvnmsve.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gwnqaeuqj.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gsomuiexp.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gidmblyvw.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gmqzcfqie.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqigbuwih.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkjklldmy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gclvolnbw.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkhblvaae.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gpoecxlol.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gsraqluai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gmujzhlfv.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gafppyvyh.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glgvqodzb.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfdfffirc.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gcfcpgtau.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gdqkwpeok.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gzepyipft.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gbaqdehms.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gogdzbfob.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gkzhoynom.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gjggvwmzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gqddtnems.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gjcsqwdhl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gzovhxyrk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gyhtvlluo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gpntjiyuc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/ghxxmdiqf.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gsxshuxwn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gcyssjymh.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdseimpdb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/ggemoeuvv.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gofflduyw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gmgozsgpx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gvmybrrrd.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqrowrcsw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gkmvjybbe.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gjkwonhzm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gucrepnpu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/glfkjrkir.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghcgxdged.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gyjovxgzt.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtgyqtzjk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghrhhctdu.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/glyjtikyc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gyxmqryfa.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gaweuqxew.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gvfveioss.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gmwqcvczh.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grbmkkooy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmmyghipy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwegboxkk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmzetvvld.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwatrifdw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gjddtfgld.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gelphqqrt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gfsiwarva.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdherxzmw.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkpkzhpvx.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqriqvbnz.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcquyczlb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjuflky.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/ghhvadgoe.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gwzxdxdzh.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gigdjmnga.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/ggijymlhv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gpjmtslux.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/ghnfzhuon.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/grflbhmui.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gfltqoqmq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/grqgsocrd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/ggajvmswq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/ghhbuluid.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/ggaoskhzx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gfpyqthsu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gfvrsoghh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gakasjcqn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdjqkqwbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gzayhnqls.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/ghqithjwt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gejfteari.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjcjvogwe.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gfhassfpb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ggonuubub.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/guxhfsepw.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gtzkddcdv.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gmecpdjce.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/guiqmmqtl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gyeplfmhm.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gfeizemiz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gysjqqhph.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grqgabeig.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gywtmenuj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvlotuqjx.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gdavcfbis.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gcmdzkrue.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gdhlhomzz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjbkeqajz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gcrrpepbq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gzaqmueic.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gvrumfvjk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gdigitfaj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gujkokgev.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gniywozjc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gbuhmojll.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjegvvejc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpcnkrjun.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkwdhpflr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqeioobul.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gcqabvgqv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gfwmosvlj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gucencxfx.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gaqfixwqg.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gtswkcinz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcpmwnyld.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkankxpfr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ghvymetyz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbjhjllmc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gyakieuou.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/golouwhzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gfnslcrvk.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/glhvnxumj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gqpxlibhj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gypcbxupz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/grlknlevg.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gjbvgsihq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gswmvdbvj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gtgfogufo.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gvdxnritm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gxfwxmyho.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gvoaqskux.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gkoimmzsk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gxykqgyqw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gjilguqxo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gubhpzcxs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gayswseoo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gzuylemyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gpikplwml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gxuzatnxa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/glgjnakqq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/grzezfyqd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmzbijvta.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gmhgbklfw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gttjkodvz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gjbmapjdn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gatbienpl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/geefcavxq.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/ggywwxdrb.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/ginemfiuw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gkjdgdlhl.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcmklezmq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gafnpteni.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/geexofhta.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gmjdhflsy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gsbgcxxrf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/giiqfdqyk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdnzxtwjn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/grbqoprji.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/grvclxdyj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gevuhkudk.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/guvtgqdby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gbdifwahq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gzcwmnatm.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/ghyghacqw.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gtcyztqbb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gjvxirhnc.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/guoflwzeq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gkagmsgcl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gxlczakun.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gfxcwkmmc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gtcfyogsl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gpabqmdcv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/grilqmrmh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/ghsyqbzvs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gervyisyi.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/glctqnkpl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gtokjmrib.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/ghommqiim.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gpahdvjyo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gklazjaqa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gabwxvhhu.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gmtsvfbnp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gmclwsgpp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmijojztv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gihphsytz.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvxxbqweg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqbgfeicw.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gagraxrqs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gdthlngsx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxoayvsna.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gvgvkdddd.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gjnxrcuoh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gckuppffs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/griyuftvi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gvnpucfrz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gpjaequov.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gjhpfxdli.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gyvgpqshz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gzcqhuxju.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gdqqgimgw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gvsybqfbd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gctyzmkid.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/glsqvjgna.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gmeoughfx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwsrpsjpu.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gwubdwkub.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gxgkczqsb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gkcgobewy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gbtutxaxi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gmqlgldnr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/guxxqvthe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/grbdflcpm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/geiupfkwp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gcewlgqsm.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gtkadurax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gctfrgutl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glpgxiemt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gkndbuypc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gxynzuzqe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gwioljrqk.sHtML


<!-- 参考信息 -->