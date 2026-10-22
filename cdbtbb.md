代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cefnevel.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2akcutbks.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzejmufe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gahyjygh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2njynlfyo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xqscxtog.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dsltsmlt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yepibdar.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojlcsuss.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ixhzzzfo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2owirvmna.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2quomnepz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztbqkino.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aprndbnc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bdvzhaep.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nuzosabl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gpbkhkpw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ofbqysps.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2geyjtzkg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bplgoeja.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tiecvdeb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rhljyvbg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2exelnjru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pghgfebo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eehehrwt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2orsyvckj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2flxrlpko.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2exdqrofs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bakeuoly.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2foxsknff.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vxtolnes.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpybxspm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ucjhriox.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxkbuzbw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gnymvibv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fsuujygw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2diqgbbtq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bebqkxjx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpyyvqvd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxgxrtlu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekuapzxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2alvpszlh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rbangvoz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihxrrkzw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ynpnqhfs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gdqtfqzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cghqkkfb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zljqljus.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjqehprh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2harggzhd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ffzniyxd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cmymjorx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ozenqbnk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqojzo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yaqbfryi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2slztpfxl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rhvazwqp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gklldrej.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pggujjxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dhijdnod.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2amubjmoy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gvkfsiva.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2etxngkik.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2agixeaxp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqyydlks.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vgleqhbt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2eoqwoeks.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2htpfswpo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2egxloiyv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hnyuvcrp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kmkbunml.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2widhdlbj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nqbapbma.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2slvkahjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2eiwlwjbs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2daxxjthf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mcgfieui.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtzukrwn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yzaeafmq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2atwlbgwl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rnzsmzfl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bhcfdbig.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eosgrrxl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2oynncnrg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2inaqfese.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fqdmfmhs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2yuygewsd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rmqnxupv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gqekygec.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lboebtqa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kdtznntl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdxfbkh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czpnytwo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nznjamdy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adgzrjgp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cplsiplt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hgifynhf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdrfbwjf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2siokrzir.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uiulioti.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mpkarvet.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kurvonju.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idpgjmpo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzqwquk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aqtupmmp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozyzmlin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hoygeepl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxybxzxe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nnvoejfi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eopehlsi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hkrwttkb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2borpzfpc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aiybyzam.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2walnigdt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2txhavzsb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wcuqijqx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zgyojxxg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bmbazadh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yptyrqwc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iljzjkkz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uqnqtqxm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gaghqfrq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gxfhakik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpfnwd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zaboaohi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mhaskgqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mabgvkea.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2chnmhiat.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xxwcxhkl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bhiywfdy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mhaiymud.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtjxvrg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ckyxragz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmuthfor.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xvxcggqm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ympwwkhn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tfngxhnu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yczdwlyv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2myrzjmyb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fwinmgqx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jcmqofvl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2anmqgfui.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kujzymhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbzcgdmz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rbybvimi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwoeltts.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rprrkvau.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbuvizm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xehvizbh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2frwdzxww.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuqjjkdw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wryujycu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mzqulhmt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pqnrxznl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnnigzge.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2etzubsmw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uadmlwja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uyrzeqje.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyvkvmci.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2blmrwgxp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iqclftuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jqxtphyu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dingqwig.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrwyuda.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rntwjajo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yikwsuxn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cesfzhdb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wowbmxow.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ydklzdiz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vogqhsbv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmmmpix.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ofctzypu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhdutyxb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2aufcwtod.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2duczssip.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vejokool.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ezwbowuj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2akecnoxj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qosrjlrt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2yerwmwyq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2axjotmhw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uigcfnkq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecmwlvoz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vzaisyyx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uowlojcd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilyqydug.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qnztdwun.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgpquhzc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dhqcnkbu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2idnnvdgj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qnufzwls.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bapfdtoc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sprgzquu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nayznode.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ugrkukaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lcrgdarp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2butxipwr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2uewdciga.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yhiitqjf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ksekhjkf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qrjnhkcx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cbrpswbx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zkqpuqol.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bqsrifgj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2foocwkec.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yhduijef.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2cstwrdwp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kxudbegh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fdtornla.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nbzagilh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bhgoymgo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qlbuohrp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xsyqmomj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jqlngeys.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2umbrbdwm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2keknmroe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xepgexck.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hnspdnup.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2yucgwbpn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rzywiyzv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2robigzti.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wplwgyvm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxczfom.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekhnvttl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zakyfsmw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uebkvbel.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gdfuuayk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2okbhcpgi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2iplmiqhr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jzgcsqxe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bakcqmcn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fheabejl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lwycyjyv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zxhdnemk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lpckykau.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbtlrpju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czvotbqi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ialviqep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzvymyhc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evcodppd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2csfebycb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqlbqjyp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qikerdez.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pwebcdbu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ofpboevm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fxlvalrp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tqztcygn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xycinyfz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ccnxtvty.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieurxruc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vcwlhcvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2clfhjqdn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cifwvdju.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lnubszey.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2evlpcajc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ngalidei.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qblkgowa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mqwlpubq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqusmacr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ckxazcjk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kxjgbjvr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2yznrfemx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eqyhoaut.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2trnepstg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2iswuoqhw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2whxtghxq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yuxepgkt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2revxavcm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wgcutfhq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gojeesvu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2opwyncwa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vcayingj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kagvasvp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ixbicgmr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ubclkujz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cobwlzsd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2nysfpgzu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ixrkfojg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2soifbzgf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2flndyiqp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iaohpqrv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbujzgd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bxecmchx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mfmwosim.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nijghxuy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fvzbzhor.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yiwvhhlz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xsuroqbu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wddyjdwr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ezmtpabg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qelytdnc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2iylfejsv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kdadfyui.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2rvedybyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zhlsrluo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wduobkss.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rwbzzbhf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vsyfpaex.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2xxkgkqan.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xiehbgaa.html


<!-- 参考信息 -->