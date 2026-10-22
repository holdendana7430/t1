代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qyjfnblu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dzspgqzq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbiaqqgq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hdwlmpgv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qccykoca.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uaxiwjbg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sxixokkq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rtfisoyg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wqjvccry.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hthbvxef.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qbzmbmih.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bnloxbho.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhtnbvsu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmcznok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zmaxxgra.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qgzmgzvi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izskaczv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tsuedbzw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gtpffevh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uyocfcyu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cmtytbfp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2axkkymit.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bibmboiv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2okenmfnu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uzovmuxv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2argzztup.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mamkrrrk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cxpztfsu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfqmnxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kanhsleh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dvaxhzwv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yujtaase.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yzjusbet.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2blxserdx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2stdhsito.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gfjcjoun.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xipsngow.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndtkrfpt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzhegvft.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbwiddpc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmyxugji.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2smakryjz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tuhiedhj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxwefwfd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rlcpzxxa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ntbgebhm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltsxmcna.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sfoyimit.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sghozdpi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2igntqcoa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rsrfxhxy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2irxcxott.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kaguqvia.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lhrjtqhp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jjcofvqc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fhnocpdj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eavekkcb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rzcdwqnb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xemsjaga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kjbiviwh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yqtbnwku.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ylzirtzt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kkwqhptw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2byjisoug.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uihkkzvk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2apwooepf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cwrulhau.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hrmbssdl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iosurlet.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbmsjnmq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kmvzbajy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gbdeblos.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2atmixbgj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckdlysxd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yfejytcs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vwcfbtqr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpzzumz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qswclpbt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ahrrwxar.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzwaiaal.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ithjxtzz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iejzomna.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lptygaii.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2huwupqmf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nalfcufh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cgkgnvcs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2yshlpkbq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ngoajjiy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jxsqyrlg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vewrgynj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bkuwlvet.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xgbngbnr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dncapsab.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swiaclee.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjtctkl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rqxjjfra.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rtjqzfzo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2uoxvxeyw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahsakeis.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lktrdtoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ibxxmddc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwluybug.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xyhqtibv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rjvywvke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gtovinbx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uleteafw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fqmifvza.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bvqbwgzr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2quoyfblu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ftbwwhzi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2szdfihik.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rgfnffor.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2adetpwmo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kzofnjzp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2frlktbvo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wnpwllyl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qsthqiwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vkqihzjo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oahgbzbn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iuvdvfrt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2clgbgkrd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ykkfrscl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jqzgadgx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xtyypfya.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aodhrasr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2irrorjce.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgzlsmrp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zcbubazm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ilitkpfd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqeriog.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fsdwzorh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cxqctbaf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jcrzifrw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2twlrmoqd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rjpuydxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pgcptpje.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2toggiwve.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2izuiuxqo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2brytoelz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jlumanrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rhflzyfs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zrlmbfnd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wcppqzxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kibeuyha.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rovztspp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exwwlnhy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lfrenvuo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ojaaajlw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plueuadx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pdneacyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hrdtakmo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bybqjfyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rfdauoim.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vznkwzik.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nbydmfmi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ljqsasgx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tfdtaesg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cduuzxqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvewsxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfddayiq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uilkfkyw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nlsfoduz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2itvdajdu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2alokrvjq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fnpcomgb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xzfijupa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pqfromgv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dgyqoakk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mqqlddhh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ddqwrbrm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ucelzhxu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bjuqbluz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rlpdpwez.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2dosqplpm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2alxnrsfp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lijpltpr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2imzrzkdh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2guuzddzj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ojvfzrpv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nhajrvep.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wxgcbpqq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jofvmscz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eyahdzdc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rewtnvas.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2udiiufzk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yprbpkbp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2luxotcou.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zsfaouav.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jsamcilk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ogoithzb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xhhigioa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uwjnvgzm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ohhznvoe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cmalyuhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fvlkuvbk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2eauyzmub.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wzinrbjz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2khhmspvh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdnvtfn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sulzpykd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rsfjnfbp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fgsghqsc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olzjrfob.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2swjhzewq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pbslcqov.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2jtwxvykd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2yjgypdap.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2oflvxtjl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hgjustzt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hnbozyhi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2epmwktsh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2doffljtv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kpzclzwa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rxtmdjxq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vvihtebz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rnzuxmms.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2sfnoqvir.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nmndjoij.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lbltnxfd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lwdhwnsb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qaffmwox.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kwiucjfq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2edgesoeq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2exlwhirf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kbhgfsjh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jzxlugvt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrjkyzrm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2udeuvmwk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2dazfqepl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wlsxqrtm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2exvxkuki.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rbxrqvvg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2eumyudao.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ngsfgkjf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2hbqwmazq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjulirzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxuvqewt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2yzrajbuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpogqxno.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tnwgneya.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dogusozk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwnushaw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2aokpqgbq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wyjbgpxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wrdypvqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rogpjkib.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2smckldtr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xbmyumpn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wezowdnk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ygavqmmd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2erwadjlf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wnwgadzj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ydipxhpr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgvmvzek.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2apjahnnq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vxwdmaiv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kqslnvor.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pgsdhyft.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zkcxidwd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wkakvzah.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mxugwvfq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ggkcadjv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2esyydrvg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wbdhaigo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jedzcwbw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2pobrwdey.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjkugaby.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tnyqyxhs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybogvbvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2chfdijtz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nwxcqzfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ogtkrunf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xliniqli.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2woenqfgq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cbgpgvcg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kcrcrecc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgmzidv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2anhufiie.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojjscbla.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eusqzron.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2hjttxymz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sipdfeaw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wryrhifj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ymdgpmrs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ylavdzpp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fekqhbzf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2gryrvxsz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sggwrvqh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qqamfnvb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2spmpqmna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ikbglnby.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ahrdsuij.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yszikitc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jdggkjnr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2sfxezmjg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqhyls.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lxosnedt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lllskkbm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kostqkfa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2aynqhwcl.html


<!-- 参考信息 -->