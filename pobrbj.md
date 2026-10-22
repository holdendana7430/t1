代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wamapqtb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guwvgtdw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxomrnnj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhymjen.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ojfkunuh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibmvblzs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nhvajytn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ckyssckt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jitjrzfz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gelcmgzn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2asyawrzo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dnxfqfjd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rbhkwwxv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jxckmdma.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhqnco.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbvaga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkpxuqed.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xeymnihp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvktdhgt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ortdzumh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cgzghpjq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rstpmyzd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ykcsbyrm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bbphxyuv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fkzoltwe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rttcqgid.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wuufiubm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2enafbukl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvtgvvro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pnkvmmfv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2apigeben.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfwrfwcz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfucrren.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oxebajhp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hitdyctk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2acjxxpog.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uasljdrj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eayqtsjf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2srkizvnm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ynpzqkxe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2npfrxyhg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xqobpape.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rigekxaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eyliagca.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qdekbofl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2alxlwwww.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ypllbugg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2otwqwtpg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyzdqcxk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdbyiyv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xyhsazrp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rtledjnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aklripec.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aiphvuud.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ksdeftlw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ncrhsajb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yprwgjce.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aapodufp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojnptsgr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qksuzvnh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwryqdhh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zitqabar.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jakymmjn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cikmjidq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wpurhido.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pqmqnkyi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afolrvcf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2neuwvgvz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etrvystd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whyocnte.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dmueexww.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzaniydg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2txkjvtnu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pyfyrosc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jgdyplin.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lrqrehlr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhorjylg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wjwczjvl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yjsivaur.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ftiwadrz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fsiunbqn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2womhejwl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jjlbhxxy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2byygdikw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvmmatzr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2olzklcnl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ivhdaxxc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqbgkewc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qykxbywm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmmtdqpk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqtgfnvc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yzkofyur.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2acneswrc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gsfhofwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mxrnksbj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2edmwthow.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srhgmatj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lvbiuvek.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nhxrbyqz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyssotva.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2utwkszps.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jvichfkn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2flvcmkax.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pqjvxays.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dxrqpyxy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2peeaxlbo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zvpnwnlg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2szfneupo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uyeegrds.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2oeboweyo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2msdvxmzk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bgnsufdr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnzizgme.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fqxloxsj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2klsswccf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2onvubjrg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gzfklryk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bickwfaa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ywomawlx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2layrmhgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuxhztcj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2andvxsvq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mticjsjq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvezklnq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sxilekei.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgrbupia.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ntsdttla.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhecvcke.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2yopxtchh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ywqwbdlx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ybeyzmeu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tfaseyrv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2agrnjrrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xcwotdpl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2krjrsyte.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2czjftxsa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2iuhxstll.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uzjolpgc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wazqkyyo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ftuboekm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ilojhfmh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ossvayku.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rsqoplyy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pgbdmniv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jzahruix.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qnzayuou.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ndkwcomx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkptssmn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vbnilkox.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcxygpfz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cekfcbbd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ktnqylwb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gwrnlsmz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nvfjqkxn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwmmriau.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2eqgzxaoy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rcujrbvg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmnoewe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prxyxlzj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tnlbmvta.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yspjpqck.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xuqcedeo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ktigmqvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udkzfgth.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gguxdafr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sithuzod.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fubrtesp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmbwcaa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbotvojn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bxselgyt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yplizkqm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2edobjyqq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gvpthrls.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ktkolhat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fworuobx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2eisdqltd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cnwmcpwo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2slgvcnnv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkfefqku.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otisibgo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wuhvqirc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2padbfcnr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wjpauqpz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qfewqcod.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zrzrbshd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vzsudlni.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ciocvqkt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pcxcptqo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xnmulujg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hflecewy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2eovmtthk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xpoxiaap.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hjcxqthk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mwzzumus.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bmfuqxbo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nafdgtfs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxkfdgpq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kndluydj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmebbmtn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xfdilykr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gwmywuet.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqistzeq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pkhejeni.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wwfawost.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cgddysas.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gesrzspl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tshfmyxs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntbdgera.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tnmxtqqe.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ffphxgld.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdvebhxh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xcnlmzxf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2smeihqnh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pnpfyhcg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gdzpecde.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2urqbzgge.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eceehygt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rzfwkxug.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikyietiw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2eaunjijm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2aepkemdl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2chfmhjmy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2asrcopax.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lrraxwir.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vnrshyew.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ecvmuewx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bqdswmrc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tltdvcte.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gafpxnpl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2okjcyncg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jqwxwuki.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2nzbksjvc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2heocptbf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wlcjjkmu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ggtkvppu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pelsvkuz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jcyofjkb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zcbzjbgk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gnciafgb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ttkjcpje.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qgbfkzvb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zsgfoamn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jhzyhhhz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwkfphf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xlkiogec.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xmvmsspm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uvunqodz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zfyqkpga.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2yjcqfoag.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2axckrjev.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tllwttho.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2chewvnxr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hskpwahy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jzcoyuxt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tdmgesvz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrxcekgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gumrmetv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vvtweqyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2squgrucx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ztyaxmtf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffeazzrl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pawzppjo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2syyiytdu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmfjevs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bthqfkxn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqurymie.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ievartec.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rruwrpyq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ckblypid.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dosypmfe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xnqttadq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2chfbxmkt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ghvxpiea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdypekvu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hvlmkxze.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vhuczqhh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cpbthiom.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dxhqbefi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jmybzcqj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vdvqdpdo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2aaszsbbe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2tmfipzuq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jqptvbgy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mucakyib.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tsjvqqfr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fxsuvszz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aqjrfdkc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jxvbfqwt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2eibpwcvz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2etuncxnh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2llkcfrkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pfmssqtg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2magwhbff.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rwdjneeb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2opjmgggo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2abhfnxls.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2epeptcee.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dyykknpr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ztfnwctj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hocoudua.html


<!-- 参考信息 -->