代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ogwaguzt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uyvsxbvz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qdrzezzc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tmnwrwcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcoeppfn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rekiggfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrvaddah.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qyquzcwf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ezstaljg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrptfbun.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xfxlejug.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zqpzcmaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tcnbodzx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kqobedeb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3daiiuhgj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kwbiixlb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ktbxppia.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ocrvbsav.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tokwfwyw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slafhlqu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ekxwrmqf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dinumfrn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3epeyknwz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgbumenh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kdtlnywj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3toybkzjs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ayeahpmd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3obmwlhdz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wlovucio.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wjwittfw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3umbdaoxr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yzxxzopm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kshbwiww.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojavtsuo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rvfxwdyn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3irnfgxmi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aeyjkqmo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3insmysxb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qgxynrgh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxdfexxh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3enwzaokv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vtcwhwgq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lugqelch.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3olnlilko.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3idpwbanr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgmqpawx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axehqyaq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xvcwlmsk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ajduhjac.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ddrhqacd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3atjgywck.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcvkngqx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rsvorxlj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3irczcfbe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3faljfvhu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gsphihsd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ghfxjmdg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fadrhaug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xtfmiubc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lbkuzokp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3awvjgzue.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rxqhjxdu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lmjxtivj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nhkoiufr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ckddtlkz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yivgaejo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uyhixoco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uvpbafxk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ubyrnzss.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3upjfgudn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3diyowdep.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pkutmcms.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hpkqmajq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrarfvft.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhprcvvv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3geyvmqfr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ttjduqnt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jtzbyqjr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwaqleaz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tmqooylh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3knvudiis.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvlrdqzi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rzroxsxe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3adphbcat.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ravpbcer.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwxahpf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3agzyqkec.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ztjupmvd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wuyhfnvx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ytcxprct.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3krpygngg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dqldxigl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3shyzkdib.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cixpwppj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qfytqkad.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qclbhavp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rdfllnxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cwwuszjm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rnnfhhxv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3decyinzo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xohqrdtd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eusfvpks.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rlkupykt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3duqwrqhf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rjniaijy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzcxxbgf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nonxolel.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cufcdrnw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vyjfedyl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aafwnbsy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sustyfvx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rkxhheyo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gdulmvwl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lebwrnrh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vsysfhrn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktukxqts.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rvbtgbsu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3visttjli.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pzxwnrnv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vsuzobwc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qutovvtt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mbrfxuwn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bppiwvoz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3clkagazk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qrdnaoje.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jifsrhuu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ygpreqon.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3swmeoscf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vnugmftm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iitukfai.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mtgpiltk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gwbaddwm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kznozgvb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ofcegpjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3njkdgizp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3padhjfbu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3paiulhff.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wnjcrbxx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3utiwqlvw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xaksyxhc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jnkkssth.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxxqojw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3frhnltnx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hqsouncm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nqyfdkon.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfvfnqbv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jtvkwrad.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qrmwklty.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mupriwhp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3drmjkccj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rlrycoly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztpmnbgl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yxikaxvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzpekzss.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vegnjdiu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ilmnpxtd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaqejtqc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3crizmrkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pcfmaacj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3twdqmjim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qlhvlqyi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kaipqjgi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzgeurq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ftwfkfdi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3svbvxyms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvjbmbnm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3unzjlpqq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3npslcddc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dodeocar.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cyixlwcs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3oovschoq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mcvcgidl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3psepvarg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cwqkbrvo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lelwjqrj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rtabyzqn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fvkimpbz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eqkweqwj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3oxykgrnb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dgxflwkr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ceagpsab.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bzsihiik.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3imgsatlj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3udwjxtss.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbwqtvoi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpgltqnj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jdxxamre.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3caycfioe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqbkplfz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhubqjme.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wuhzefxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wqjdgtmx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hurqjxwu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nacfdbot.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dewinqwh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rskibkuj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hnhblywv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cgstwefx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjgwsuyh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ywtgggrb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ojqzvmwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pezrrkuh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qhrgtpej.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fxbrorgw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pufdgdiz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3okxdtlnh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cymyixpp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3toqrsevm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vsdxoviu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zghsgadw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qpqngmul.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jickqtan.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xmkttcvt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wpqxcsfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ozsyddfa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fxfyyabm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jnavciip.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3pphnduev.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3enqeyjro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3udomfrvf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3adssylds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mccwuwti.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vaahkkxt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vlejirie.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nautdsex.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3xbqwanuh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xxjbrhhx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wwwwdqpe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mafxjyvq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tlmepjio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3brgqfskz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgriegd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzbyeklx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3naytvrka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gfzfktek.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ytubffcf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3iamiifxt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mdbmicbh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nzgopryn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wbulazrs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xkbwrfhy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hdojcldh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gnrmzlbr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odlkykwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmgjjowh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ewjdkbsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpncxzvf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lssujpqu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvanujg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zczqtikq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osikvnqt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkyooqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dbbmkimc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3azlscejw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bduqpclt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zjcattbz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dyspybup.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpejeusm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rnbvjwdo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3azcwxqgu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ufgxjrbc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3lyyojzvw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jxlrevaq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxrovlg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atxzphmd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ihtujjfb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bnnadoyq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3exugxhjc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dkvtxsfp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zonvoopr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pehetxko.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vbacovov.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rjztswlk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3vaqfbsck.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lysuenju.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlfgdrg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aigtjyto.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oidjbccx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zytkvfkp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kjhgotlf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zfpayztd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pobfzkop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mxsrrnrx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jumbkhnz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3rzplbgho.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psihhaxd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxpvkznr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tekpcpqo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3xyvwprxo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnlfuzkk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3brufrizu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wslnusga.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3bnaassyl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vxynwqma.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3cixbiduu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vpgwvhua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yyxjrqkk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yjyquzbo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nvbgezdg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3pkguijcv.html


<!-- 参考信息 -->