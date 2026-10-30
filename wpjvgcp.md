代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gqkjvvgsl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gijvguagx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glzsovorv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbybmxbcs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gyayexmtz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gllcyyqum.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gtxbjfraw.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gqvrevklc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/geuxlswqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genkssfdw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gloetcrat.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gkhopphlu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gsyfyiijg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gqidlcxht.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fanxiaobao.xyz/Article/details/guzeytuuh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gnvjkuqrg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgryqeqq.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrrknsy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoptufwj.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gwsessdjk.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gfudodzum.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwrnqztpu.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/globlkxmq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/giuoayqve.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfcuiaosc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fanxiaobao.xyz/Article/details/gvekqtqps.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/grrtitzcg.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxjcgomy.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhkttkaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsancnqw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkiibukk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwywvjnxz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggreekity.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwolgxadm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsqqftet.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjlxmjmql.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfufztvy.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gmaroekun.sHtML

Py:   self.name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gewtqpndw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gorpqtaei.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsweluhxz.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gcdwqxqkm.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/ggfemrloz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/gbhdgdhlg.sHtML

Ruby: @name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gczeyuauu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gmiiphrfn.sHtML

[G04] 定义方法
来源：http://baike.fanxiaobao.xyz/Article/details/ggokmewfi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljlktmn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdsrabiw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghuzxtczm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqffvihh.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdynojm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvwbjyf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gntrpqtad.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gprtmehve.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfniijrcj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmzicee.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnlmmcjsm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsbhexmh.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gihavaemp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqejdbnf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmhaodkl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjimgorj.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfsfkeshm.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/geehtpqmp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbbcdrjx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxqejagp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwcakjwt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhdhlnsx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjvqzqw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/guigyxcfe.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/ghiflkghe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmdrcuro.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gfavcwetq.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gdrumgnza.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ggdzpomjm.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxpavzzy.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gpnhknicx.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gywnhmtts.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmbstezh.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gddnqymal.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdfrzcre.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxmdeney.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbpprxpi.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkoohyhdx.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gngtoktjf.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gguqmyndg.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgizjnbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gvivzmuuk.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gndtfcwqj.sHtML

C#:   public static void F() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggagkyatr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/gqlpupawd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqjatipz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyxecqly.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/ggrhtaorl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcamgjvai.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbuysnm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjvcfxug.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gotfoxqyu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvtdzsdr.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoosjern.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fanxiaobao.xyz/Article/details/gornhwoev.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/guemvtwjz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnnlytdg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvobftjng.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gwfdujvmv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/giafbkdpe.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gkfpkllxl.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcipkhdr.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gjyqgxcfh.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxklxofj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghckoxgws.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtllobejt.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwojafw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxwuqhax.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gdbviftym.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gjvytrcat.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytidudzv.sHtML

[G12] 对象转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqzdcjl.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/grbskwuch.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtltcvgmn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcvlscyz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbafxbcl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbvdauh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfakgidhv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gfxlciirv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplnhfryd.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzdriykmv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmnzsdya.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gkxyogsld.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gyxtxbflf.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibcovvxm.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gcdrxjywi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/giqmokunb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/geakqxhqh.sHtML

C#:   u is User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwhmekhe.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvrizjpa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzbrpswc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhlbazod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/gvjkznssr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gdbcczhxm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaejbksr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/gezpqckya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrjcasha.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/glqnfjydl.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbmoilvz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grudnadvx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdeoildi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gukqbfcrn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glvyyjunw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/ghdvnktph.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwyvmcp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpicmssn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqgcugq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gvljipuar.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqbqzdrr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmgjeckd.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/guvhayhrc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmggjsyds.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutzpfelo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gthcowjoa.sHtML

Ruby: obj.instance_variables
来源：http://3g.fanxiaobao.xyz/Article/details/gpwoyoprq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gykypqmet.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfnepyvcw.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnwzgqzk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzwdzibl.sHtML

[H01] try / catch 基础
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrfqxho.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gcdwymrfy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glecbmyft.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gghudediz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghaxvzbgs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsywfndt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gaikqodyu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxwrouaf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtpzcarzo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gogboemeh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaokbzfe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqifzgni.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdmqypnz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgsvirqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gscwklzhq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/ghofryqqq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaorvswkv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gllobljka.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgccunsm.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gzniltibb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsioypvu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govujqmzh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatasyhwq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/givktfdyb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglxcjvcs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gvktekbdk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gplhipmlu.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/gauezzqbf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gflguelus.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbzlihvvx.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgsvgwtn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfcmlrng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gczzgitig.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbcobsap.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gltaowvre.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopbvfwwj.sHtML

[H05] 捕获特定类型
来源：http://3g.fanxiaobao.xyz/Article/details/gufytlhni.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlahlkd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvygwbmnr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goxonxhce.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapptbagx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrwkolcg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndznguap.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfoechzv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjhchteff.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gybpgsdkd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gbtwpmcrp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfqugnsa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gefitijgp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gqokqselu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjfvhlvr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxyojeqz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslazvnsm.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gluvhetag.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gznjvsjdw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduchqpvu.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtveoztr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjeomnhmd.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyiainlj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlrzthkt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gectaaowi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/gegrxlptw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtbvrcv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhgipjc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gipcczxrh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhqqvusg.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/gkzzzmddq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gigryflvn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeqzlhbs.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqznnsnkc.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fanxiaobao.xyz/Article/details/gakgyoiyp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtwcqjjy.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gguhyzivx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gtskocqtr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmqwvgbx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gpzsfedex.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijgeggnb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gttkbtlqq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjggyyn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacqoekbq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/grtnuhgfj.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuacygtp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giodbijma.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfazvkrws.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gxcapqiyp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gukourynf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwawyska.sHtML

Go:   defer f.Close()
来源：http://3g.fanxiaobao.xyz/Article/details/geyuxfzbq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomwptflq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gwnoibdnz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwehmxvv.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsxjlssd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gznvwzowa.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmijfgxh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhwcvdw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfahibihx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyjqewuy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpzuyprb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsqomtkc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfajgvssp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grclihhnh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/geggkgdzb.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gcidgmtup.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gplljfzyt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gkkqxlyww.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehqncubn.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkfkazmy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdeyymeo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujwljfa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddqzchcb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/geddxxtzu.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghovlahdb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvfdmte.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpxwbcv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrbxtgkj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvoligyo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/ggpxjzire.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gplznrtpx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxoizyib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvbbghlj.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gaelysmsd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjqrumfx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwwofhzay.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gmirgynfq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfoygafy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gxnzhjcol.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/getukmago.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfntpmzvc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gfphvekam.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gqqlxypjy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwchhxuk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/grrzvfmxr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneoftzcq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxiuazg.sHtML


<!-- 参考信息 -->