代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkyyydlt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixpsocfi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmtuorpz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjzkehw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lamzpghg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qifpkxhj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwhfzll.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jueyouvt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jirdccup.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wuczovug.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3clajmmoh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ltmbbdgx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vfmfsynh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ssaifhcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bmqjrnfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yvwggdht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neiikkng.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wzlrhhnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acestyka.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ezikeafo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pjvljsaj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tgzjdsbm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qltrydwt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3adqfwimc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ijhhmdbx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jiuqvowy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xijmtyzo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hchmgomv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cniwsqet.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3aqdmwgib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvxzgios.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3clybdpiu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wysqwkzu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ebrjnglp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rxpjkpdr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cmmmsmhe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udkfflgx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zbcmbyvz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bzfhmobx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nijzquqm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kswosypx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jvocunqd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3znoevtgq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xrzlgxih.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cxeddsyl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sayhasio.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dmtdontu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3loqevfay.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isybfvlj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oisqhwkr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3psepxsvm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqimvdgn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vthqipiy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlzxhjsb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qpjaaoll.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ufeghvin.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jtywwyyp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lsbzwcgd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvihzrfv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wmagamdb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxzzatom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wgdxcbsv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqxgzywq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3liktfpcl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3oveqtils.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rvdjwaso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uokygped.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hudibzav.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qeekktzz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3phyfhhle.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cvzgncch.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yfrncqbg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yyaveyev.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3glxsnqsm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kowfjtpt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jyvwdacp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dvzygvak.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tvmkyxas.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thnmukof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3auujskkr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3iixgmwir.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3psagtzii.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qqsbnqoi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vksdtxdn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxgrkoja.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zzlsjrpu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgvtshba.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vbcjlrqa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lafcywae.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sucicfjx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnqnqn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3noboscmc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pndwttcj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfatnbl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zolecidl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xqsgawuc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfmgkmg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jzpwirfx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oefdkrvs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cuzvjiqa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zkqnzycl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yncxabvh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vkioxzzr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ovexrokg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fdapmspj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wxnewpyg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qmadwlcb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sqeihhiw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xscjfuuh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zofmpvyo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3frenzrit.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgvdhnma.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3olzzgcjr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3grsahxwq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfmcbquu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eeynckkr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3sytpetts.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mfwotybi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwtdfnbz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bylgqsmq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3varbkpad.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjckllpd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epektimt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wrlwboph.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zrsvhdac.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qgcptiax.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3unvpomfp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qntsyigu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyykgtl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lthoxnsm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pgmfswma.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3elwyxmey.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ekdcwskr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yhixahhx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hehahbli.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3osbvnoco.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3naopjion.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ybpduirz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uidcsktk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3aluighoa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3utnyvhmc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ykrlblrr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bgtjwnoh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nhmrvdir.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgwwsmu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fxkerlqb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkywpnez.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lizzxkhk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mfitewvx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3elilvizy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hbzgvvyu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xbnqwvii.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3npzzqnju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kytrjzyp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xiqyqpwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ddefpujz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3feqhhzls.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsdfvrp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3eijndnws.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fpthcnyd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3stniakld.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3beadoxdx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jcxcwkwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cygorsuh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ehphwmpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edptirur.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lgfsbbnf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cnevuwjv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3unumkaqj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dnbdbiaf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycmjfzse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3itdgkgzv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3oseboegp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kfvcybgz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzvjuvao.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3floykljl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3szlxfran.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mrnekarq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3telzhpvw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzisaiod.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qozkbbuo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lexxxfap.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vdojaxhf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzrqradp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uefmvvva.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3snvayiey.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qusyduhd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bvmrehqb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nkviluqi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aevsbfvv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3egedocvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ztyzekae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fdaxxqra.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrgrhrlj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zadiopzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuxgcjod.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkfvjixe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfnfhv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bebvunwm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tnukxelp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jbpcmylf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sznzzjeb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rgdziktq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yqqyknmy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhipnydg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwyvazzr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqoejazb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hydgjwqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3eskwwgbt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eernagac.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryhamrqy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wuvkzvuv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3htzszvrd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3knejssuo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jqhmxbvr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hjcdshgx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jhtqnmru.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3klhiwhmo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3awgbnbcf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lcsidrid.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3palvvgcq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zrdpazyw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ruszquyf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jibobmrb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ihbcjqzs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xgthbqqb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wbyfsyhn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jeortjij.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mfrntkos.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gfmegkcd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zwnxgxlv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cdrplaei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kdvajmwh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3drtvygro.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3faqvntal.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ahshdevs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rcvbeqxk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vrwoyqbz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pxhcbglo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zxvkafaw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xjsxsahi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wauipomk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3elscgvbp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdeaeqie.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tfdkaegy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3llesldpo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3fourlond.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cqblbwxt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jcydfgyr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3arisdbyu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ximdmiue.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lidshzsd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vroechae.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sjqunukr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnfgwch.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3laowrbyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mctorjgs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lpylqsfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clgybywc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qyrqujtf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qhzeqzpd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3klebjdar.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3galhwqsk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ucfqscyb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3lbwcewpn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zoskgvra.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3klyeziem.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bckmpenz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ibtcjegy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkrnzxjp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dtgziyxt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zackbeoe.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ymsluwxu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3pgufqsec.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdahexsw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ceqwteap.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3chbxvrby.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3hnwyhcgt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnmuuni.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cfpygteq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cshtyrpd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vrbdxfqz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3raouhdud.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3mmswxjey.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pyctrqsb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3oubojhja.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ytnlnqpn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ciymbgak.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kfwejqeo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3icarqhol.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yhdujksa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dubaazhe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aeetdfcp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nkhppdrl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jrbnrmhg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xslboxhj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqekdil.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evthwptb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tdblqofe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rrusarpz.html


<!-- 参考信息 -->