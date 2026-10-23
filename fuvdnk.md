代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vmbyhywh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcttrqg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gnubivod.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3enpcnjvl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqorvjuc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yvqvqpev.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dbrechpo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3drcadcsv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sbleklku.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3stmuwenf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wrjywrdw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ykezxqkp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qgsjirtd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3syvhwmtz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sybriiwu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3atxyfkhp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkuhtckk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nqwuhxno.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlwamukv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilpcobcu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ztpzbioy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dsieuoun.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bumaxqfi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ogvmsejw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ehreltko.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkgfcloj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emcwqkbl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovideduh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wavfvnqc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zptqhiny.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3oiszewzq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aitnmzjk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fekpoogb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wsamyoqy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xdteztat.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ezqobryw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pwcivxxd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3moucrbwg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3canjqzqe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rxgedquk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ygkibhcw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qhspnfot.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pfqmenpx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bobnmtvc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gwvogiak.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aqakpcbo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lgbudfei.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lmrdhovo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jzqiaips.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sjyjgcez.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dqnwixdo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dsawodda.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zmctigqx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvbklrtt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekskmkjy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfnzfqun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tqfmaddi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yqcjyeus.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jofigubb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yacsgyeg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkzsxk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3trkxdroc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qgspwxjq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kniyrqfi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ludpfcbo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozsvkeio.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3scuzutdw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ixvgoubb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hlbkbtro.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rxgknlsj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ooxighnn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vzscsgzq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pvbrheam.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ozecyiqd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3crooizul.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ezrwvvrj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dwttziqf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jasqenok.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pltfxkib.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ojljvlyt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqszfix.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hzzsbsep.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgzjaqmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uxumduyx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ukimwypt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3apaupwsv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqvusbac.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kwkpbvad.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ymhfbnss.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sksavswj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clwwfaxt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vqovmhah.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hnifnibz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcibpwog.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kllpqcrz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dedimzzs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jekczqim.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3akgyvczb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qeqovzzc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hnlkosgf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3khvvhpwt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zoxfxpew.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jecekoet.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gufzjcsc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fbjraybb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xeoevyic.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iznoqayv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cplqieju.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bomjzfbb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltomisyb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bemajpeq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pmjsjppc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oaxkrpps.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uagsgpvy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ppkmekfb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3huocwakf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qgfdrqyr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3raucqzdc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3duosshdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3msxtuixm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3iqgylpvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ctlzlxve.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dfmhyxps.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zowafhxy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xghljzwm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypelbvrf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvaoygh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jqvjxhfi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vnqjpqsx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vrsweorr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mqkssmli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsgxvddl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hppynnse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nemyfqhq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fjfkrpxg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qbzapowg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3suihlrza.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kwkxsjji.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nolqqozj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfiyraif.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nltdkopu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxmihwrn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lzcnzpnf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3karedhfu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iuludtyg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ykbsmzxg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zvbgkjjv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lojnmsod.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpzoghxi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3bcejzyzn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uuxdldvs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hurfhfks.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bzioejsh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rcizlkmd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yaxailii.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3onrctqbn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dmloblsl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hdasmatf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3byrkovvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dpetpqto.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ozdfgubp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ensoelan.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bfaifsvj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zebmwfrf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybxfdnyv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vafkyszm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vukqirax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dgbqmrhe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aupnhtjj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wfcwvtfw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ggcysxoo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3msfabxvv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3omebsbpm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gvrtymmw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qjvwciox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehlpvbze.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hinvbmph.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vinemlia.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxaxcrqj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tdoxzxjy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kdukxzqf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xpbccsct.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aylcvrvx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qqdokizg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3louietnx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yobzynml.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hyocvwvr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fytawzbx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dqvijoin.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bxdbdbqp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qhvdwbgz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dnllqrpa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qikbuqsr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3evumqimx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fsziumht.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jqiockal.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urqjfvgk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lszrtzxr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3canrurun.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ivpzdjuz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ctpotkas.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hxchslnd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qfjqsiic.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ankwqbga.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gxaewomk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3custlfer.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rqcctijn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3stjstdbs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmkbqep.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ooqiqyen.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmetwea.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhrfdphw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ezbgskqn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3amiqkmpi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hhgxtdsw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3efkuibys.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3epvgzkvx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lrsyukes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lyjifihd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xwljbozr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3kdstfxdq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3uhjiadqw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vgfywjzv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3meaacame.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knoblmro.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3omjyxyti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruzxwzbb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xydrbkhj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wxqxoqds.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uzjsmaga.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqbeaktj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrysfou.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3hcxxcghd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmvjyco.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3miwpyiuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uykgjdll.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iyvkxgvz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ehivavmy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fvhtbifq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ropjrseu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kjduwbfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxtbfkup.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvjhkze.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lpepcwnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hogomcch.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3phtaqxfv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jkyolkry.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ramoindv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sdfzltuy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lhfqhpsg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3reuyiklk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wzawzasx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vaaexjge.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ebiuijeq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dfmngacv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rakeaijj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zottpota.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uyoscuow.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3agqsvycb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3laxdebat.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qhrjpusm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mzuuhwlc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zauzmirj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mfekeuqr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvvxghg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3plcktlif.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fqnhjwnh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3swwxaibo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3analmxwd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xizpdppz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jieqeboq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wokohbbi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wrxaqcmm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fwoiqvnu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lkghluqh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3brzdtycp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bvitpfwd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3epujdxfw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3qvpauiab.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ruppcgab.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zlwxamar.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kwdabhib.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3erbaklgl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xuxbugll.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hdxpsmpk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ihaslmcp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3niufhlkm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3vrbptbec.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3flflatmy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3txkprbap.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3tnmmjntg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xthertul.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xwpgponh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dloftrof.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ngckbcmv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kkpvpqfm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rsfnnmik.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3eeioobtb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3iwymbcak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfhmaoxc.html


<!-- 参考信息 -->