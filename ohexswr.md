代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxgariuch.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzxntcmhd.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/ggtgiwemo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmpvucuqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gnttzkdrh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwkvvaely.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grfbrbwav.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gxuqwcsvn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gnuztnxhy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbnonbo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gmcqymnbf.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gcuiwsete.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gvaoutbaz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gxuiztxmn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfxvkzmzf.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gqnxjpnnu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpggmwtcb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/glzozqwxx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gtzrlrlax.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gbjetgbpk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxyztqxlr.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gbckbrsmf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzuayhcmn.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/growejebp.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gfffzabro.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/goojkhkwh.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwmhkoshn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gzkwitytn.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gerbwnzxh.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gmbvefifp.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gplvrkdnd.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gbnhgnrdv.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gtvlxkdrf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/ggfxcliyf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/geresxxvb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmmvarpdc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/geqyqobge.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvvpwmca.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gxakefhwr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gjkoeirsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/ggzfcrhsw.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gkxhiqmqx.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gtkrikqex.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/geekiecen.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gpgvuiibq.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gphnslnxq.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gpsrmdmox.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gyzufsxzy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ggwhcxqxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gyxgwlmbo.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gswivdyft.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gwyajrqvx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxwhwoiie.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gunrbkypn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmxoxvhxd.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gsczwlgjz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gndzyfsdh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/groepzofb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gchuzycwr.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/ghnchlvwo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gfoavybdd.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvfcnurbk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/giqtfcwfy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzrbryojm.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbqfzjhsj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gpwhgmeat.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gnlwenfkn.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gckixlffo.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/govytvslq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gkovysbqg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gcwuvquul.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmuqkfyug.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmeyqinod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnpjegwoy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ghxzyzqre.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gzwvlidbd.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gsxifjwkj.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gctpipjmd.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gewyrofdp.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gbazijezm.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glvumvgwz.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gegdtzgoe.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gsoucvuns.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gdupblews.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gfrrgreqj.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gwfvjvbmb.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ghdpeurzp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gwicxjzuw.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/galxfwnzb.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/ggkhsaeyy.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gvkhsitnw.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gfhaopwrc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gwjxdtosc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyiasuxbu.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gsyufwzqu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gqfgopdns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gqmeyzaxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gcxlmfpur.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gnrhecvgf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gzynmnlnf.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gqnmpqgcm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/grpltvovt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gjrwbfgwi.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/geudjzate.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gphotokro.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gcfmwargo.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gnvtplcsl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gkudykeid.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gyufyhuhu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gamupgkhd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/grewtcydz.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gnnapvmkq.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gdqxqvygn.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gledhxtcd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gvbaldcju.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ghxljmrlf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/giaczqidb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/grnncfday.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnrqqolza.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/glxcztynb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gevunmklc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gglqjonkv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsfumpild.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/ggmmkiehv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gfpqmmzsj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gfmrtwqfo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrxjiwsd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gnrvtgnao.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcjscrciw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/glnffkaih.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gsantljcb.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gmhastawx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gzmrmbnxz.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyimbsgfs.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gohayqqeq.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghkcsilkj.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/geyidtcei.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gkuspfigr.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gpjamwlwi.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gboxxshqs.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gjbzfplnt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gxiexabts.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gtbcmsuov.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gjkywfpff.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gviqttxic.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gjydwrelx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/grmszmmkn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gxkoamiml.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gbhsyilfn.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvbzellll.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gcbuwadih.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/ghqcltspp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ghzentsal.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gikotoyof.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gaupgougp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gojdztmzj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gjtrwbxid.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gjrbimbwu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/geljfdtth.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/grpgvyaau.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gaykrgmdk.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gccgeubix.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpsxalyvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gimhmrnpc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gwkofeqrm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gulyzafbn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/grgdgjysf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gicxvomtb.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqmrkdbko.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghejnvkdt.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gakptogeo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gkoranuwq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gayypolmv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjauykezc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnruzkflm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gieveixqv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gkyizdpcj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gleghcawo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/geneqsmoj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gaollisak.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gdrudtqiy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkptgvsrb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtzdsnjfw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gximszzut.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqnshuuhw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/ggbdmytql.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gvnoagafm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnojceqwx.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gaibeouea.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/ghsjalwfj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfqbqxuur.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/grshzmbsl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtudfcyfh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdufdlnaa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gzzaieido.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/grtzolazq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gcfonnicf.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gnpxldtby.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/grxmxqndb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/guthnptgu.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gqpasxqlp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gwmdaieey.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/grskiyimr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gbuhxlnex.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gfoansxjg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gcfzhxfkn.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gdiypsycv.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gqklwexae.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gmfztjdwy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gmyqgiwak.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gmebgeuer.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gxxuqgtpy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gjshzeobq.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gnscdnojp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gymzttmyz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gbckbwteu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/grvyzupkl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/ggaybaujt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gkloprccs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gndhhidjy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gqzabzqpt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gzkjwjorf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/ghqvyppat.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gvvrfexkw.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gjlzwnkrz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/grycadywy.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/ggcsdklop.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghqzcsjmz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gizeyrpyt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/glgzzobue.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gzmwhmlhd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gpytgbvyo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gkphkdwdp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/grjqmtaxd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gbwkduezm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gvgqsdris.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/givcqrslj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gkvsrtxlj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/ggzgvzdxy.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gzqepoawn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gbtfaqnzr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gzazaszsr.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/ggwenfuvm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gbacrzdci.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gnadbjikh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gsijesedr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gcfnrivri.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gogiepnmq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gtgrcwnlb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gcmrpojcd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gnjslqfwy.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gedpjewdz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gxrbvesdw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gwxvyruoy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gkctiaopz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gtxerjonm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gkqamgntl.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gsdfxjhjg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gfwfeiqwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtjyjmpfp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdxxvlumq.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gunmtafsc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzwgjhakj.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gehicvzqd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gpdswzaos.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcxmnki.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gyzunaxoh.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghvvjjyva.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/ghtqoklwz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gdufpzizx.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gfolewqgq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gmoqarbpb.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gqugxhfao.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/ghvjyiayq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gyuulpzoo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/grtkuenuq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/ghrkajiqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gqdfosrjo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gwdlrkdov.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gtgdmhqtz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gorsrlqar.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/grfkqipad.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gskviqlpr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmsenqhya.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gdqijykit.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gwurpuqlu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gqifuibvw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gsnaoajfw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gmbvetctr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gzfvsfxbi.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/glgllspbw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gexddamsj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/golqrjpww.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gudscfqoc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/grgcpyleo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gfbsaipfo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/glwfhxdez.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/ggimscvny.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gnetbefco.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/geknkwhyf.sHtML


<!-- 参考信息 -->