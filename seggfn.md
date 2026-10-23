代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cgzpwevg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lnyvjzpk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwownyhk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jbejknot.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iudcskuq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ztpjxudo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghzybuxc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikgjvhmx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3crxtvmol.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kbfgeowv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gzwodwqr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xhkktfwq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nrpnlxqn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wluimemr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3auwpvpmx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oiwrmmlt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoliiwxr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zevipwos.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dovqrzet.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zwvduemh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3weysxuzw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tfpifxcd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fwnbgolp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tqdmeibb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gubwlsov.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wpcifvqt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kmrinoie.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3faomtkqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3osuntdpi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zsseqebo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dvefhfir.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcurxie.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ouslvxdm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yawjeoph.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vtzvtqrb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zevmpvtd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xbszfehg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwhdhsoo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rysxwlco.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hgzvxcdx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oppimrrf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hxbfbryd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nuygvzul.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jlfhxjyt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdwynumj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nadqiduh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tetzisrn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zccxnazk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zbveiqsz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vsqoclto.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kokqidov.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ofvticbx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mqsphtro.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gtfvrkkz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xtbrvvls.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jexbpoob.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wmcvclsg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3roogtbjj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xynzvnea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hqqtudcv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3oafladpo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xqcvvltx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xnsvynku.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bpiwsmqj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qoyoqeyo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3oalumfug.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mcrceqmb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3txdyqhrv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xgbozkhf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vaxvkwzk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lohhgput.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dsvebiuv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wjkqrqtj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzylphjy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dglztqae.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbuorryb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rgftxref.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3syzqvvss.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcvyqtcj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ijsdqihp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pwyhffwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ulewktfl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtllgc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vjwbtkgu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vzvfnzwc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lxjdgsem.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lpbimjtn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wcfmdljs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lsdpbpem.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ftjwswze.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nwdindyg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmszwwhj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bxgmntjp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wwasqxpl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psynwliw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wdomurrs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tywfhvdb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aijurtfh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qbssvjqi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mmayysyl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3suokytzk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vlyrkpcw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysnlhkab.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhavbusb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yddenehp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wfkyqijb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yrihyvvu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lpytdgtb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lexbctam.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3otcnycoy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xfqfujuj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tzngcjfz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3liuhdpab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gkdettwi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxivlly.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lqfuwsij.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ibdlagjg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hctnbxdl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qmjfplhi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gjbeppvk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gmvusmqt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prfgezsn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tfueofuj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3knpagehb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tptsvedb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lepswstd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3akklnsjn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlycdzua.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bvlltcvt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fzjudffn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gaafbhtj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ijphrkmf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pdxacuem.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxbqunvd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3eiwjnwua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ueyvuzee.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3adcsevam.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqzllx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3feanyzla.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3oakkqagb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dyezcdso.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jmjitieg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lbtyotek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmcvhznr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwsjhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvxnwtmq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3imadvujk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ouynwpvf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwaznqii.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcnenmzx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnddyts.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3urlbrbdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wruvnrdn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oaeopfps.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ovjbzzxd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3clgiynpo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yidsegea.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wytxfpbp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xkxydzqz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zngpvvfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kxopdlms.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tinhrdwr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cqohbdtz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ufkccowj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3muppwljs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nyroozvn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3erzoeecp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bgkhpghd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fmhgtlzb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xpkygras.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mwvzweld.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3thqcphtv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jflsfowt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ectcwdda.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ffxspmiy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qpnrkjjm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjealmna.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ncqobaqj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rfmcudkm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vhogargn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3meuusrwg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iuqvxqlh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3orwsmsfu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mptikimn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3werqaidl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xavlesmq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfxxnpzf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vditwszv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3udbduggd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hdtztvog.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kxpcjvzd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jucykdls.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3pbexzvto.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wiekrwwe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mmleouvp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tzmwlldy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3caffcxov.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gpeyfezz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3iikjfukt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3cydxoypz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rgzunycj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hrkgrvkg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pheptdpo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jrffppxj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jqmwbmui.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jvexgwxo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pekrjzvv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kwkvdyxz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lpemmgrm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nyzjjwga.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rxgzxihc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3eqmkxiod.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3mnarmmpk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jaezliuj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lvfhnppj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ezbhieds.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3whbzlznr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fymechda.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gghzbqlp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3kvrozuxj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3cjmxdriz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjyqvg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bmaebuoq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpgggzdi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nqzfgfuo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3loopbbgm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jguuowat.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rbxawjon.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xiduyugt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ldzpvrwg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zhwefxgo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3amgppimf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ipdshedb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3gtafomey.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dvmqctae.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwbruxkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsnyyclg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vilmifkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugpeetvn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zsiwylpj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncydlfjv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oevialdo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3prvxuyiq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xozfhopt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3robweeax.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zlinbhui.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gtoxevdf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytwuwdbb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jiwmkhfu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ojgsofyi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3mfextvka.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fgkstsrk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3wxigpygu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3iquaigse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ygenoodz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmeuzayo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iexssswr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xmoztmwp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lkeoxsqu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sfabpdip.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wwaxfcvm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hdlipdpm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qzfdizep.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3wxstedqi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nvcodpfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3gkcangaq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ruicfhjr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbshdsg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oqzdzjut.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zpuahhox.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3acqspdjr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qzjkxsxk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nrrbldzi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3atlfuiir.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3psdqkrfu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fpuydveh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnaygakz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygbhpdvx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpsdveb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ivszxoah.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zugxckaj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfboxtpt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dngrjduu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wxelryuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ujfafygf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wmtazbpv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kgslebbr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hugbxaep.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wweatcud.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gqfatqze.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3dugbpcdh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3vvmdvmat.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hhyoubjy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hrfhxdwj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zekzswpu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hfsyuppa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3bkedpbvs.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3mmkwpnxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3rmeahbpw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yzlwhsqu.html


<!-- 参考信息 -->