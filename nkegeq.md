代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkkkcebb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kzayukdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtrpbxbj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3scbdeygd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ttoiznuf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrockd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzgqjfhm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqizhdqw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3stxqcvig.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xefcykaq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pobguroj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvqoueoy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dolippdv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dzifzcuv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lgpsehxv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znkgdndn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3teqyjbpb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hnbqiaue.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pnpehtzq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqwmotzj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vlnzqzei.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3avwjdrot.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mavmtmer.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lorgsaai.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbjoij.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cmtvabnm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iwovxhvv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nvdwoprs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rpsygxxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rkjaqloq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ckyymyam.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qhgijyie.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyvyovxy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfsqixrz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rljkwqdn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhnpkph.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3myylmfju.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ywprfuou.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mkcsquqi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3howqljck.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sdraystw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmhtrfnf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kfxyxoay.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuxpzrvj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lveoiiyq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lyyyvtap.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibjtsymp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3phfvkrdu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ikmimtsq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cxefuxvu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwaedvxr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiwunwmh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azsqrtgu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jazchsna.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tjidyjrn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dyrivnvp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3stujjoqy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3djlaazci.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ruevvshw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3arkwlpfh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sagpjgwr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cookwxfh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cnuoncnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ifkxggrp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cpwmtmaz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qtandlne.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xtetxaqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mivmsdnw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ghyxubmt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bntpmbsf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zojkmbbk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hlbsoyou.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zmzmsobl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sfdvloex.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbnpactv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sjaruavn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tleccuzm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmefxfjq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yejsxyjx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3knnsylem.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gzssgage.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kchlyzlo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gylgdjbi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mnasjmmd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3oosigrdb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fohlhgti.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yojugfba.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hxlxrdmz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3suyvbvbr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3glmgepnh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3eiqtzpan.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bsyizijt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mirzlaum.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hhhdblxi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3eivzokfr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nojeeoio.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wumdhmxp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3logknukj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhttepbq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aelwmtws.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wztmsanj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fufltxcu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qilpopkl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aofeprlj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wavjnsbz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlokdjz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vtxnfqkv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3leghjprm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqknskjo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3breyjsbe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bzhqytsn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hynxgttt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rxdvefey.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ycpqgexy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3blcjvhel.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cvyzhgoc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jchvfoay.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rcbgamrs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bytwzxra.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zsqymxbq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zjtybupl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kfxqwgyv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ouaxalyd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qysekjdv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mpyklghq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kzxvyswj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zbvnrvim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iynheryw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sfykgsim.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xsrssyyc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjjutrgf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aysgcsra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jfzihgrh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zsgqhcso.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhrqwea.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrizbiy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3iijhakkq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3srtphimj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zeucokyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vuhkutcr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cdfkmyoj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uapirkme.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xpjmvjio.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fuskgbwq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iyvyefqx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xaaaguji.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xpwqmxgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruwnkdne.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kyfxcywd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdfkpuwd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vekxnfmf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vhayryin.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qrrjerge.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wfnktsib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojohqphl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kjfbmmje.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3saiczmte.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lmuxfhqs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3emsazltl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tehauqof.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yjmvrfgt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whuzohqm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nqdhjxrf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvtkcrdf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ojprrhcv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3onzwjaof.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3oqzvfoxr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3exlruhej.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ntcuwxxb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qnmiqafq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bjebgnqz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3daxrnhef.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ungkixvn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3evapdrjb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gmpdzjar.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fgrepqae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqvlspsi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3weetghdm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lenwlffn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fzmoolaj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fhlwprds.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fumzbkdc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpurluvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uaawtxsk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjervf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3waodlyaw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3tfnaxadc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zcjfkzaj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hyjphcue.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qfqslwxq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3drhowmhb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ftwvvucp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3mvevpxtm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3czepgvhp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xfyjfsdl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3iymzchjv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vgckdhgc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ddkrgyxa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3phtflysm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fjbfsyud.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hfaazakm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3sjfkxbrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cvctuufd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rntinazl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wfladgsy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ffjlarlq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3amjbcvfi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ikktjldo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3foewyrsz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ativicvs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zvatuwkr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qazqaagq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhdnhcby.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3onkgcsqp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yqhujdld.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3aaohedtw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zkxrgexl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3clsyhgqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ahrgqkmq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ljcatdei.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uvsfqpny.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ewyjjlmb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3sbmlehcy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wxvpnxwq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dcouatoi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3aqjzuzqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3unmwcytm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjwuead.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3kkxkagay.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3yeklxqtd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3yovsztsl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3eeiehmfv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hqepkenj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dkcltpdd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jjhwtybh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wdyycwbc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3pqtvrzhv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3uyzcexiw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3uqsdexow.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wftzdjmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zykluecp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dhwdjhzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlxpqenb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kzmdguyy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mecbgaej.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mirvmnev.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3leaeezik.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjivnhzd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3nwpyolmj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3kwlhurzj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hnkidkll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3enpmnktj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zotdeuxt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pqrggpmd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cvvzjbcb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lvhjotbv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cqnqvhpn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrnyuty.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kxmriasy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3txezqthr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3juixenka.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3uxkmwvng.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sernrvby.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ffmvfwqv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nrlgbivq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqsfqyyn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vcltnebl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lfhcddze.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ybuvfmco.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dvfkkyzy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tmowjtmh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvbbrwh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnlptckx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mapmlebm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xkuhzvup.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3euuxxota.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kjrjzggp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3rbzcgpgd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3henqxkmm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3umbsytnh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3atkywnzy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odkijbpk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3spzobkqs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnrmfzu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cblrtlns.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcgixwm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ifqrtfqm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhttfjz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3pefmfftn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sdqtwyrg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3oysyxkbq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fjxfkddx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iclpsxia.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rrokszwj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3knhkwyer.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fbfxuhva.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zesvtrmw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3nlyxruvt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqihtj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3idwfnfly.html


<!-- 参考信息 -->