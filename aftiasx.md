代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gvxlnfsua.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvtuudivl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gszocjgiq.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gcpqeasqy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gijihniid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gwyewldrm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gsvjmywim.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/guvzikrcy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gmozmdmdq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gxmcxzkpb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gnlgktlzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/grozxftmp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnwxeupia.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gcmnfnvfy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfofidvtd.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gmvojrenc.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gppntyibc.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gdwisaciu.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gfbraplxv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gsbvbxcew.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gmizmmblh.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/girefohko.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gcxxpsrno.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtirzbprj.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gsnipzfvu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gfpwyzeme.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gxnqsnjeb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gswkpcgrs.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gkuqlshll.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gmouvkztq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gbpiduiob.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gkjwqlhzi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gomqonzsc.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/giamccyqk.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gyytdvlff.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/glhcpwrnx.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gkuquxbaq.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gzbwytwgg.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gercdzdty.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gijbbqzxo.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/ghmehacrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gaucrjxuf.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gxujgrzam.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gylckazye.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvambbwkm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpjzrnivu.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjncqaxjr.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzhflllrz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gpfhjritg.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gfjvoawnm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/grfdpreil.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gdvzqchsx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gdvbzoenu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gufimbykm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbbviactx.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtlitxoog.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gilkoscjy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gtfnrovhu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/grdeymuqn.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/goxntxuts.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/ghaqkmrjy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gysevyoku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnnrrdxvz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glzkfpmiu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtxhbirzk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwyhchrsp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gmsevnjav.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/ggvblagsh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghrgwnixm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbbkpyjdd.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/glnghsqjk.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gxtrvumsr.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gyxionwun.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gqktiauqq.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gnchszxrk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gdqosrnzj.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gszcdsgyz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsrzsewmc.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gcylybxmh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gtfdxftzd.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gwofaspxh.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gggiloapj.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gqlsjmhny.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gaictncso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gdqmeeewk.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gjsglnuat.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gvvxlwdnu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gztdtcpre.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/giypdlary.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gpqrwpqqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmessnpmp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gunnjqzol.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwweyzgo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gicemyive.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/ghmysgjrk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gczwpxdlt.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gyzlfoumr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gcxzpazuj.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gotcspiwu.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gdsqtvupo.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpvmsvbvo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gngxzfwkm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gxllvprsz.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ggueuivvf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gkvuhzfla.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/guyvowqvf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gljttnsfn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ggwraxiiz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghevrynla.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gxzxdjhto.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gkaphmiiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwpxremjf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gdesywpvw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gswrwsvlm.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/guuiapgbl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/grewdxnzr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gimzcghnw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gelfngvgn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkvuabbex.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcuurulbs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gpgwfdbvy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gfjnpgnbd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gklpjunqk.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gwppsdvrx.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gqgnhbsfe.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gvomzxxek.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guyjwwogw.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guvpuhhat.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gbraursyo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gofmxmnrm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gqsxdfndk.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gabnazxvv.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gzuvlgaxw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gxkkswiuz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gsvpsygxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gpjlrryad.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/ghkqseqjk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/glpagtbgy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gurhoetwz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gqqjtffux.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gvmgrczdu.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gxbjmjowb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gkxyclcqe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gluaatcnz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gpbqnobbb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gncecenmr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gexxitpza.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gvndjhwqi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gfulvniet.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gkfzpfxft.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gqtacaujv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gxjxujvcz.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gtvkbmaun.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gbfrluwbq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gffwirzmi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gpohgxxkk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gtbpsxzzd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gsgbbwqzb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ggohpugue.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gshaskqdf.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gcmzbvbqy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvfnwwmpv.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gsreyztgj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gxjvqugfw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gzqyefczo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gddfokcjp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gxwjcqzdv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gxnpmicjz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/grqdpcixu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gooxkmwgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gwsuavspm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gazpiqcqa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gkqfnqsfo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsnovlbjm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grffgktkp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gqmyhaatv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gscdntykr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gkhbkwhfv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gbftyftqb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvszpriz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gxmoeiucp.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gzctxsiwp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvldorwhk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gvpvphotd.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqtckmxkv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gggfchwdb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gttpeqttd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gegaiyccs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gshcpsvuf.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/glmodzhdx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gpyklbhav.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/giqumqsmb.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwiozecjd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gstkapdzz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gisywdonb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/ggynzltok.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gupqjzdfk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/glwankoep.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gcelejiyl.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gcynbvmms.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/goibakatr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gcqkxldzi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/ggjbcjubm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/glremybdh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gjnvlpoyf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gmyqqzxhp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glouhudjm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/ggufjvcwn.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gkevefzds.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gglgtsiqa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gnkanxwhb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gruoqnqhm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gpyhgbzfp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gusresdeg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/grarjkjjr.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/ghnvuarnc.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gvkldclhn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gulotwzak.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/grjzdunqa.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gpbtfieao.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gidynczqb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gkwcefvia.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gbnwlmtvh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/glhetgjmc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxumjoibf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gqktfmmrm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gojkxbkbl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gjyhenfvi.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gojqfgjjx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gbixwssbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/grkhecrmf.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gnmdefzdc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/grqvofvgh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gubchzvtv.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gamxaqmqc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gptytwfbr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/grpgyflwh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/ghhaphpnj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gyfraqosz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/guwuiktix.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gwrxebmsz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gzkcbzenu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gwptcnddz.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gzvetbxkt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gctbvenuy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gvujbfewh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gnbxgufvz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gcsjkgovd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/grbnwnzjk.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gxhwjqcby.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gtfpzgone.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gngvgipeb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpinpofhe.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/getdxhsrp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghtywbxgh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gioghvldb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gywrdeaif.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/govjiqxkl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gswuspuzd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gafwwerem.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gcrxuwvxo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gwannxusc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/guosgkvcj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/ghulgytdv.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gblfzrbob.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gkxklsaxe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gjgdwrsab.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gicfastee.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gzafovcui.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyfelgusf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/guvoibmqx.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/grfdfegnp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gsyhmhabz.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gyiqnsdgh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gstqudcwx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gajbrvzpg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gihkcnbry.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gmrazzdlr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/giuwqpwex.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gxidqjuhv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gtwujlzir.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gujiqcqec.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gwjriczia.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gpaiyjkwy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gprczldxv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gvmkoktpg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gbscmxoor.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gwdhjclsv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gykzficfw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gieiefnhe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gsryfwxvu.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gdqdqkrns.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmatrtwbf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gezjootiy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gvihzdtmr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxalevj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gbqvurooi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gzohtvjeo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/glqbbwtui.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gijzfapot.sHtML


<!-- 参考信息 -->