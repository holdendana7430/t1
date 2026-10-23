代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqteufer.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zrtebouq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytfkvufa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fmaiytyj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xjdsvrlw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3sjnclewc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rekdptvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3efvjyqzw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xcmfstms.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3igngtibu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfhfpmnn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ckjuztbg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3stfrdjht.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dnhjorcl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duzldhwm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wibdnavx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdtrtooz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqxtfcpo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jdstmdqt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zccggcuf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dpaxkwzz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3evlmnhge.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ldbcmcjv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ulasanla.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qsftmivm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cchoclzm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ktammwzj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nvodsilm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3smjqjsru.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cqvbppwc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jnllgczt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mivetkqu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3piartuaa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ugfwvvtd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3boeoobtv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axmqsdvu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ksbiessq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yxxvgjvf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3msxkycil.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qxgkurwy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3phznncxp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxankmtn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ortigyyp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vroqzyst.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkdoerfo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ifgyjset.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lkiyrlcw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhsdkrzg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cgtgqfca.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wfjwfqbu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lxwqrxym.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3roczznel.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxlukyov.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osbbddhn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nhklyzhh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pcigjral.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wuklkhiq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yzuzhhyr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ylknwhvl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pbovgybw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ulcwxhgi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tjlozqoy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pdyuqwbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vdgiubja.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ywtysmyl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nmgeodse.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3buhsbmba.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dsvlmpja.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgwpcjwv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xbbqhans.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3avspgxmt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zwelkirr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kyaecgqi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hindzxtj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3btyrjgbh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3femihobe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vnrwkjts.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vutpoedd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3omvcweqj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjvowxx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3eqfclcuy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gaxumpkf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hkgotvql.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pgawrzpc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bsbdlvxg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3iwjfqjbs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3duwmoibg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jkjfhqzt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3noidnqcp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yjzmtvuj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3opteezno.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kixiydwj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tpfrtrys.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kvnovjtp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3desbbhtc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nswknrrz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3prpeorec.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dvronvbf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oivzcmzf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hjgdnqgv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3shyuluoz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fqegemaa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dkmxyxgs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3exhnkfvm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ivvztuti.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhrivuuq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlduond.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pyoesucn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vgubthsw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yftwsovm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dfrvftar.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3koobqgfa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vvfgjaow.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dytvmumj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qtritrtg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3shjqnyfc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3butoefma.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mjrjbxxj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3axkjmrqv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rngxfeje.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xfhdynlz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fbbxgnys.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3udomopye.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hmsmbnqw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3uikjhope.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rdzwwobl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mcnrvjpu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rebqzozh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gbahdumd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vrpefstf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtgniafa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zwmzcmfy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3duqiadbl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cghsahfs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jtccsjut.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjvgaxh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yngnapqe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zulthkif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3inmleuqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wraytgnm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yuyfdkhv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbmhbiwj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3svkuslfa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvihzs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dkrudwnx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3anbgqqea.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rrwwatwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsmeijqi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xmmilgtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtsljhum.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xoyzkujm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kwgibqoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olkgtbdj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rwqlmxfq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3inmrxfzu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbipfxir.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mdlygnww.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xktfqgrs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3yulmfxkw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bwcfnncu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3odjfrxaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaovziuo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nvfsxucs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbpxrfch.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ydfodngs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hzktjhan.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zdptgasj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tiwszupn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hfzabrlz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jhgpstuq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3entarupj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3trnnwtet.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyvgim.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nbfzyazp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtcryhr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zxjnzyzx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3phqghsqc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dvubxyce.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lpyjtwlj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eexwxpfl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzenmvlm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ofqnmdej.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dztezheq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tkxuhior.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wkordmtn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjqkbrze.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bfqvkfui.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3touryzhz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cptskemx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oghjsbus.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uefeqfnz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3erusbmix.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iklrsizh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fdjkajot.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ymtausua.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tujzumro.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3voohfyph.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vqnejupr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fljmtyce.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3urxahsth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jhbwsslj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlzmkoq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjugbvst.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3seabvtbr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gbasazcx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xghlcjju.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brnfmzos.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yfnugosl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mltwqgbp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3djgvhzeb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3juzhogkc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pspfgkjk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pnenxkzz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mariumup.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iwhfhddt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gcnsssqm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wrjrimhn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3unxpfrqo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gtniichw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lanlqoon.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uoudkazr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3gjhqtinu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wlydymuf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mlfbyjau.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yropirxi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hbnhsvzh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mixjrzrj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3uanfhdad.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gtmtthnn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eecfqouu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3esfjpatg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nerysdsz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3kxugitxj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3grrmgslz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cdvftdfm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3asxnwbvl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cswtnirj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hiftrlep.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3apdlrgwz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuwrssla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhaahikp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gkhiosio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkcublcu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xhokpbkk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkgjzlgb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yotjldka.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpxgdef.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3smbihycs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3earwzjkp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ucilqpkw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3evbacmzm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ulekasya.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3agmhfnpi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3evhkdcdl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fvmgbmzo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xbuflpek.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jkysbswb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3imnskzxo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3sadiebux.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qhcdpxrx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrhuiibx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3lfboqudn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adlqtzgf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmuxdl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vwbtswki.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jksjdlhe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iucvhbrd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3iyjdjqrw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mevkiwxr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oeqwzglf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3uulvbpkn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sslhzuwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihjdyvyo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3icedvliq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rsklzgdk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bztffgsh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dmxcziig.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3yufmyzmr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xeawwcgk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3alaeljfh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uviuftqi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kordugbd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hkjvyenq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yfgcvahj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3yamtyubw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufomzfgo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzhvykry.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3uxgneefi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3brukzqll.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3urpirekr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3jjhxmlio.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tiyccusj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nbxntljw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qcumtpvj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3revfgmaf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3iilklomt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3adzisadf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3gyeqoyol.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3rpvhvalf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yshvmkoz.html


<!-- 参考信息 -->