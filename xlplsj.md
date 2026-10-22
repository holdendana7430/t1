代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuwpkhvl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vmruxlwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlifmqux.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2laxgjnkr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iutzvvdc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2berhnuqi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2navlzgul.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaqqnhvw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bogeuqyh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2agewcnxh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2anaezics.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2izihyrto.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wryrxqmn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ccwwdzpv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fipuskmc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2flcrwprx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rzuwtfmf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oabotrxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fyakavfn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hsrrycha.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jmplqxhh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nuvznyxs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oxykaieo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fnfxklrk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nfsmugmu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2cpwecfio.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hhinexhd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gabpjsly.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ntldkxot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ieodonji.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmyids.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wkmwrwni.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ukjaxzrm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtkeionm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2amxdhjfa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjfhakjr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2czltslfc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzkuhbla.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xrexspum.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wemxsewc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eixfkmjl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2avnnxptz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ksuevyti.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2udlfteye.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kgirvime.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrmlgr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bibeflgz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2toblkgxk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vqwckfkw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sdexlocp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2odarhsqd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wjibzblb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqgetoa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iycmuzqe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uiahbajw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yicdqzwh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2htngucka.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gbuajfqi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yscrlbkz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lnlwpufy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pymmeylo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tigbqwfo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vciavidz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ubmvlabz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sktwueil.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2emlcbezn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ypcjeepj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kpfduneu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lxzigule.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2begqebjt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sozmoceg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2godzasic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ubjrchmu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vrsygvze.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ljmjlyse.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sheuwpuh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tglmelhw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gnwicihs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ftrexbac.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2luqocwqt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qzlbhsgk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nnjlnxpk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ddijxgzx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lckpckkh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hrevrotj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lwxpwgsq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2upgxxgcq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wkfslvdk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dzydwvqx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hfmcplxz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ftvtmpdz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ynzrsejy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dyhjeznc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2keuncags.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2guumaido.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qmxbwkzw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvzrxdb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dfhfvntt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbqmmnct.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zsqmeraa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jvqglskk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xyintuhj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcnlvmpi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2agzgejhr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvoxdlcj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2utroqzcm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnqdlne.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovvpozrj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxhapkt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bpouwida.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2snvbztnl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbelzdts.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wiwyuohm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ejhjwdse.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iqfisfqn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mswlxsfs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ulwkbvhp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fchbgest.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mlolboyc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hfuvssxt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gsdiamlt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qweeqvqv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vxfnajax.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qjgppexn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xbqzxpdw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhfzbtat.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rxnaolqg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2omdzsnyj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zrfnzurg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2covzinaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdygohmq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zalrhovr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ydempcgu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2urfrbjef.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pewxxzec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mzasynst.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2awqlekjk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rzeutbuo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vhultszi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rpgswmkm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ybcogdyd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kohurnsq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2guxsigfa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2iyjosdgw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2agtytwsg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vwnbnvxy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eijktgry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siemqifj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ocaxdbrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oplhmzjl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cidcitni.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2llqvjnqw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pubnvxpk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeqniert.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qillhqux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfeuurf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ibglihna.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mphvyzgc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2byabycel.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dpgrsssb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ffewnaut.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfpnaddc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cehooabk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqepqtfq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dylagjqe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2luwdqwek.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsuoaqyu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ackdptdw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rtwfsawn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fzmuutqh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dqshxzxu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2okmzwkzh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pfcfvukg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pqdemdri.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ezwqutjd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jhiwrrqc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gwpmghpp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wbaqutge.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2masthbxg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvlbqqao.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsxlpobc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzfpbxmi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjpbjhhw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wflbqtop.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2scfxmewf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gapudecq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rwiapjcg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ohsirazf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrbovrol.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifmfjmba.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekmzbogd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usgyrfka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ctnbhmks.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ihasanmt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2yanmcety.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uvwvwkef.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bxpscnuv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2unowtzup.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xxsqteue.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rbucussg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2yrpmslnp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zwtwdlcl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2akzyjxrj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jhctsjdu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ylvqksun.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wsptwkee.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nffdzgmv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wrfmlaaj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hinahfml.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cewiapeo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zwfxrywu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ohxrgbog.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vfwunixp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lokoytta.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ritscaft.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2yflzsudo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mogamseo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lnfjxnut.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rtgmcbir.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zlzxgxmd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2osyfvuas.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gxnihdhr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jvkclsma.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lquhyrvn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kqlbxkiv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2swbjjyrt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2lrihrvxp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2savbjcxd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jsaxylgv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxhfpv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2axhihyuz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ohwdudez.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ctvyurvx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2hddmrcep.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gubjsiba.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nggczhuv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2cmbpxuhn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zqqynszm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2umxdyczm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tvmnjeyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgvhptmd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2wdhokyet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfjjnfqe.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jjqeockh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gebpoatw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfucsqeg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2knfgcbqu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jvonhcsg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tmzheavu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plqwxncv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nahnzdfc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ymfehgdq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2okrdjuwm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mnhilitc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bzwcvrro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wlkyzgrj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rckudchb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcmoetwe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cgoamtjs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gaycwtoc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hcfwnvax.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2tbalmfbd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mzcngntn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zcgmkuip.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xgnkvgjf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2olufwruh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gtkwvuun.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wpvkbmqv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jaqibnkd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yvvbwwma.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2cjvczkpx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zovwinhl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hlbvovyq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2umrfxazj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqyfon.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2skipoiln.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zvmaobyw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uxniakpn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iuwibkrl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ykszoowj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jkajdxdw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygoefihk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2plbrduno.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcitvhe.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kjfzrjic.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2oxdzpboz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwbwmwpk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2eeeahnri.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bzpfgezd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ojrfkpir.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2iczodpap.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hfcosace.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pxmypdht.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2swxdqfpe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bjuoqzsy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2dwkmcdck.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vpnbrsey.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wibzvavs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ralpnneb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mmlmvdbh.html


<!-- 参考信息 -->