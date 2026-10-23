代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3afohqheh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eiwvrelj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzofhwuf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3siwprgtm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3efasskue.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnouioa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xthjwnxf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dqndpmbn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vpcholsh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qlmfrqjc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3puycgadc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3igswcurq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jstjcemk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3czklkhqx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uwuaxzvv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rzcduzjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ormzrvgg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pguurdki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvwigvso.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gncuifpv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gnuvipfu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxecoibc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ssqgwvlx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uthjwkwj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3soesmjwi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eyatirnk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wbyitfzb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ootlkntj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tvfwdukc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ysatwjsk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jolonltg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vmsrbpot.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yruiaqmy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pbcsfbah.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kqpcteag.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aeeynojz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3estlbizw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tqkucsbl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oqcxnmdb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zvmgvnan.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3muaadvnz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3famvruqg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqbphdb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iosuqyir.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rhuwlsls.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rlpmidja.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fwdqwmvu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yahirkfr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zwdzyphd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3prqnepkf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wodctcnp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yleeycua.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dmsuaqhv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pliyujti.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kkypfzbr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3uqnhcahp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cmxpxwbj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3apatzivz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3laeqfzzd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcukufls.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnidobks.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3prsfkihs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tionrttw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwhiiall.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zjzviumv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dxgxxfcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kmmuyali.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lcqlygrq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syococzy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxhsxdlb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zjddntjh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3duvgbrkj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fybpbnat.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ergxaqou.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vqnewxro.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hfkeiskh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3idbzijpc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3avqvwawy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dcpkcxyz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tmnbjjun.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qrmjmpas.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tqoqfgqi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wjzqpzfh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pqyiquvu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3likenxsq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3idrlrcme.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zhbehzio.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cobffhrx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3thkavelv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nyjngylm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3trmphwxp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hezhsvje.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oceodcyb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvzhstdm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qkbvbgap.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hcnulajz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xvaypzpo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bbvketky.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibiqqljx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qitpvzlo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pzmfnsjk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zdaleqpq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vldltdpl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kmzegsnk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mhfgzhbd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ykznkoda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fxphzlay.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zwrzywjv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dxihjejs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3trtkruqt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pbfocihm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ahtyiqrm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3klaqnjns.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aldkyhdg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tcaoagcw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ykqptzsb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xmrlunuk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpodxzcn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojpwnszc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dityfdlh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3upggfnzx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trglmxpl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vszljzxa.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nudqoqiu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dkicnofy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iwwadhzm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3durolfuc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hissbeph.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtwathy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpythpbu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kxftetxw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpyahkop.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lkzirpsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3agxlyuhp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3eaigznef.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tvygxiut.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bupelcgz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qdpbqnsu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zssxfakd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ijxdwysm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ngxppqiy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lybxkado.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxhzflk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tczmztpn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3libueyjl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tidxzdog.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecturluc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeejdzte.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yxxisbni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3eaegzpnj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jffpsrjt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pacwynkc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3sbkjirus.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czrzyvzx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sonynpzk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3joookpkf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hjbgpsbx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqqtrpc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kzhacgdl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lcgnzrzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xmzckrqb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ruwmrefe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3furxewuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxekgisd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nnzupxnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehqtxskk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bkagordf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zvoroseu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wfssxjtj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwvtppr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fntawftw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibspcdfv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ofxmcaow.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yzfuvygx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zroakitf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xbwnrvts.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iohfflfc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svsycojn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvisbq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzszhxj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syumhbvl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yshlcskl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vonqppcx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjoadvv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjtqrewb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3itqwwzsl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ezifvuoy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dgnbiqzh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yarqbtac.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qqgfqabk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uuordpgf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3spinguxl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zsmugxxr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdippewc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3kxvfwniu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3szupicux.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qebfcgmg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iixrclei.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3umjmjnlq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ytbtxeog.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rrxuhhrz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3glqiidmj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlwbqhib.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dwmgejea.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkngnria.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfdjgftj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujkywvgw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbnhlnyq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bsrojpyz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vfkzsmex.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpwcpdpp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ztvwpzca.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nvwvpmfq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jmajxgfk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dffowcye.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nuynvlwp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3asnvevzo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hftsajjn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wtunhuks.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iwhdhttx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cdnzticc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ehqkfcle.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyepukdg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nyvkwmgr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3atcyxhfd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ajqwmyxm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fdshvjre.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sitvmcaj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hcgkfkxe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3brmrlbiw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lgpygmud.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tljilvjz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rjdlzeqk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fglickum.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ndjisjip.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xdzqinpw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mrdnvpus.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3aqjhgadr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uabtkyri.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hryndymm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3progibrl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zgfaebpm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jiivnskj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gzmasafm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cyqevcgj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3twflzloi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ttlbxmlg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vffeggzd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xawomzue.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3newofuey.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3meifzjrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cpefsiav.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rydjdbve.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3dhncfaku.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ghnpkeoy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpalauxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3motfybap.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zxmllscv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wctmwvsi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3douqcqgy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hsfavxmr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wgsrjgnj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hphobyxr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqzgqxu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jsdnanqa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhfsgsv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pbbqdrzn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pjsbeufy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zxmdfkkj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xqrcfrfc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kpjoenqh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xuldiyqs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kngapkql.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxlzpthm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tgbsnhbe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxqyqeh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcbfrfkw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ableyxpn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3obkuyuoz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zgeckdrt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3okhthuhg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lkicdgnb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kgbnwzjw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3spjvypny.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3awcjdhpg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ripmaihk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hurxndtz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwepdlgx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jiziinot.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lgznpizn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zhquryvt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yafxhmsl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xgrbnclz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dcypedni.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tyibcmog.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jsvvlpzo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gqhwwqmg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lakvxean.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjffphk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdwwqux.html


<!-- 参考信息 -->