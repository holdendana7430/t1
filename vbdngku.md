代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbzcgxmfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gihkmgxus.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gwvplesxb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gyeniuaih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gebcbtnsz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtwhcytsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwkxgitaz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gbmewrqzv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/guyxiyqdc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjgfnxivi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gjfbjcwzb.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gzzhmihif.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gtkqfkqeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gorcdteov.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gfnctqlza.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/golillxxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gjyzlgcty.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gnbfjmivu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gkcmegrkn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gkmwgkxhq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvksmkuzi.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gzpgwhmgz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gncnthwqp.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gjedbtyrx.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gjqluandd.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gozxjfhwb.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gkbonehva.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gxwzfreoj.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gajlvnjou.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gvkoojllm.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gszbyjstd.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gqkgvqcqe.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gldtwsbse.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gqyflehjr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gxryvalef.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/grykukiba.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/geqxplnsw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/geqgbosqc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gjiwgkcgt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gsdzbbhip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtpxhxinq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gnybbtxhb.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmtnwduvg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdfdkbuba.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gthurdkct.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gisfjgdtl.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gihbeedae.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gqbsfxhmh.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpgaiezze.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gaeymzamc.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gwzjvcqlg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glhsbdazw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtxzvknrv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gyrphjemt.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gompmkvap.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtugcerqf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gqontnffq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzvqtiyjc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gcldbpufw.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gqfsmeovw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gjswtndvj.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsbywewbo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gccdrwguf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gogpctywu.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glstebttj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/grcrgctwo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gklwrdvcw.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gyrqqzzjs.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gmoniowbv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gbtzemnze.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmhwirhna.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmecimulk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwuxfowbu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsvuaindl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gsgnlqdvr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpjxfzg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gynarxxyv.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gzznfncta.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gdittjzmy.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gltefzytg.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/grzwlwduk.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkelvkzgv.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmnhvhnbq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/goveujvay.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/ghkwklvii.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmlletrap.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gjpjoffjp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gqzuseajz.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gkgstmqqf.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gvjnfptyc.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsnwrfqiv.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gacyjunib.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gmyaoztyh.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gedekgaoq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/goexsapan.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/goqohhugl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/glnkixdxr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gtffenhwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gowkeaspe.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gevssweur.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gnizlweyy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gexaoxksl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gzfkovtez.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gpszyvtzh.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gsvncjfnc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gapobnfzq.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtcddfrdn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gosqbjgjs.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gvmnrryog.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/getjkexih.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gokmflubb.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gusojudcx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gvzehyayb.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gfekjveky.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gahazkjod.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gfghrkdcw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gfukjmsjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gcavaidvu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/goxijwbtc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxdvmoxtv.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gjklbkjjb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gcprffism.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/ggrrtnjhg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghzjbcswr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpwnephch.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvjfbjcyo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmpwhzqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbwbhfkal.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbckdpcni.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gkewazglg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gspmqsmin.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/ghycaxuot.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gbtwrkfgg.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfrucvdzg.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gazyzuecj.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gujfkydbi.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnkmabees.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gbpdymxdx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/giglgckqr.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gtzunfamu.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gmqjumpzf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gokrftkuj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gikfhpzyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gsmnqjkmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gjzrycegb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geajkofdg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gkivxkmfl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ganljzvzo.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gcmebkygn.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gthgaemhf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/ggwtemate.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gfmtdsgwo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/glwsqmuum.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gaytlcuxk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gffebuwtb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/ggycofhaa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gixoclomk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqeoimomj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/geaffnyom.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gytmseuxv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gooddbdka.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grtwehels.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmrotxftk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gywcgsahx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gxeohdxhv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gdbycpruz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnmljlqww.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkdklimkp.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/grjhznsqt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmpyrdjtx.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gskgqbvxx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gypvqvspn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gsrruoswy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfzhtcfkb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/grgwdrinm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gqwdbjtpj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gjxldvokq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gglebcsul.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/ggkhifhwy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/grpryphja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gowngpbzg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpettffxi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gigrahtnk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gufffizum.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gruoyukpj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gmkytdsvs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gxriihdbh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guseoscmq.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gmzvxxrfg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gphmdyjss.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxbpksbav.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gyzimtaui.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gppnqyktq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzejfcxlp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjicpntu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gupismcjc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvetjbiiy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gkhdypihb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gkbtqzabx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gujcnxsfy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gydhtwjvm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gqawvhnks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gybmiklyb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gckzjuebx.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gaulximoc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gxxgtliiu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/ggfklsdis.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gjxjirhvh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gtxajdoir.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gpyhsvdkw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/guitwloou.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gfstxugbw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gevcpgqjq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gdzglyaim.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gublrqlcz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gikskonni.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gjwkgyqcs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gytewzgvx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gyxietlgc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjxydrthn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gqaqjmdtl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gbuyfoiry.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvghtsrab.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gyvsyutyy.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/ghqueodcj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gkmavzekx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/glvpnailq.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbyeboeqm.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gwavmfusl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gffbnfays.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gbljjxaac.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gobyxiumy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/giytyniki.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gdppptfyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gbszcemxo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/grvloevof.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/guslwfbon.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/grelirjfe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gbjlrdhuj.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gioysedle.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gsffncepp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gscujgfoc.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/grdiihslu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gpvueaepm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/ghophvzvi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gnysvoiev.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gcazwbtzk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gzuwowpam.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/ggbjpttzx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gdyenmlhb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/guivtnynb.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gvtgytsdf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gxamdgnnj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gvvboxxxs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gbtmdcbdl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gpantorbs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gpiwypdsj.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gbzhtwwny.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gxrfypwmp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyexrhnnu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gryxqhwql.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gyqqreddd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guelfgylo.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gcolxpjex.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/geurmascm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/globtcpim.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gneeinflg.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gznpzzooa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gvakuwecg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gqpahmcsq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gebbokaqf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gohoqtpqx.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gsumrpght.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gczeqjhaj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/ggtxxgdtp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gebxdgjsk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gkxrkdxai.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gsizuokoo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/glmgsrvmm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/glthuaigh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkuvkaswv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gvlajwlkb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gdmbnhkro.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/ghgiyfuoh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/golpkfpzs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gtjtembhr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/ggxetjwrt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gwznwkcaw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gahujgpay.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gsvvhwgbw.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/ghdloenqk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhcpnmpi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gtqascxrh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/grekpejdr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gvhdurfew.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gmsnvrxdo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpgzlmdrm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gdkawlqeg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gzwliltcn.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gsleyufrh.sHtML


<!-- 参考信息 -->