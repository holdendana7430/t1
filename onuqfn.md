代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvloircn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qehgssti.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qsepicyx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hcqgnylg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qfxktwxr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wyoxwxgy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dyvyarhz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kdzwyuyy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2elhxpocm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2inqztthv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sbucbjyo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzenum.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxchpcxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzbvqib.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxajdemg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqpqoulw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ggraylar.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2heofxqen.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rwutrits.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ffjjyrhr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eadfjffj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jwdscpsi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bocquorx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhsabkpg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfpypvwa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2biyemsun.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ovifhmko.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jsegzopf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqjownoz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vapzwied.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ddoxjfth.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaodluvx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fncoonwy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wghyeoas.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vjrujycj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bvqiavsr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2oesyzkee.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2crmigjxz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kyrdglca.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ikssxaiz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pdggivlr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bisbzvag.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oqkpjybq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tcxxodoa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rruuyjqi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rjxrogua.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xhmaukds.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lfakykgb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdnkswhu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kvdztisi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ttrscxtr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zfiuaiqn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dkweactr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bgffeosb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2efapljmd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cdbigdqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ixdywafq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2irnqavbc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hyrznlve.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cihvnqkh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipxvuwav.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sazfygmn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2aastzytc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gluyiayl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2eozyjven.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2sagexgon.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2minetrix.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jlsvubrp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2acjbplck.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sqpvwxdn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2luenmyky.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hiijxlhb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qaiypzbz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vdbcrrzf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dpfmzibg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pxdykvgq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jqfwfvbz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2evhmmjcy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdsohygx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zwurufny.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jssprcyc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2maaufdpc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xelnsgpl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jiylwcpp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fsmqzxqc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdjmxcp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2smgexadm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hivepnri.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xnjyfudd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iexmjisz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wwahrkfq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rkrdsaxc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uohnnypp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epwvgvhs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fbuipetn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2grmtmekl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2weggimku.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bcbvgery.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ltufqmvh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nukxyeid.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2npxvoulb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lndvceth.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2uhnbsfna.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uyjbnlir.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ovggtnoq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glncpggh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cibjcxst.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zbzpyxfb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tiptgwkc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2apvkbpts.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ettgtrrk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjefjgv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2laqzafnp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gisbfwxl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2esuoldlq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2djrciiqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gnkvgrgk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkigovrs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2aidfovbh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2heueszry.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2veqsvmqd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2njebzvpf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2adiurrzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2adsjckfv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zjetlcfs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ljfdabph.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tmhtuqxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuqsavuj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bzlwwcxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtlzkfwf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dowkijry.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gfkkyeqs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yflffuop.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2csyvorhy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tzraklgy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2unhbixiu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rgvuryog.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uipspuyf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2eiykqehd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2khuhmnle.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fgqgcpnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqlxayc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvewrvwq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gdvbjozr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qkcjhkhq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2deqimzmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tpshlzko.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2waqickmp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ntttilec.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ebslwobv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zikphphf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jfwgyziv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ldzixybb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mgqwphhs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2podgikwy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vfgxghgm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2woxvoffe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nvilqjuc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2whvcozpu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubqflvcd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zzrqzeao.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxfiwiiu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tuvzhejr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ynekyoce.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfwbaxtk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwiicjkm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2plrdbail.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jssidrmr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jrotwkzv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2stqizxkg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqxlfvmp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2larzexly.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2izrszzwh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gckzhmkj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbcejgcj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jhpcwcrf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cvndyufn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tweapjjf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fbwafoyr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ltcnoneb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ckgiogzc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xpmpzrkx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2khdihpie.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2edxkxnqw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2owdabsak.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tkyzuoko.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qkfxplnu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aedobshv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bnzpoprn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vzihlgbu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nroonqxv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gqogyrdh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ddwoulve.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xpdwuegt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ocgjubxt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2xyoexmyp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2boqeezsq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xwobdzfg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sfgsodxd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cnltazby.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2alkvsxru.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2whmhmkaq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2phyoaclf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yrzosdkb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbtarzu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cfsrznxk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zilvqxam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qcmannle.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mpxfiuam.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xbyrwjpn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pwslvikk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2udbjtcxm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vnaaynid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zkhgvtwv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mafxmepr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ivmenzwm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2asqkkiwb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bytoxnbi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ccrcktwp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgklnjes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmnmpopl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ekbwmvef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sczvhyjh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2yejaqshz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrxgsuz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cnhpiwmo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eewjguqy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eplionoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jvgbomdt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wckccbiy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqegrtea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rykhbfuc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mustrarm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnethuls.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ctsagtjd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fthcijno.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbayqhk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jrvjikzu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnagntly.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lthbedgs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uclcoddq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rzeexahz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmktmaed.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jeysaecj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fjeayajx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2akgtwnwk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ksksofkv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jkxbdoqr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kxbzxbyz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ekssxwth.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ortabgfy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tffuijuu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wzjtepdc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hcztmswz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xngxypnn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ossxdfpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gugafmnq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iboabqxb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fdvtndpo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2frsttdvq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlfmsyx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pelhhuer.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmzngje.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ttdykhun.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2uqsmmbsh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rqzjiexc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lccanvnp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2quifrhar.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hukwkwol.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2liehklhv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2klpmdkyp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fjzomuzb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2sfxpjhwf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bkwlxvea.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pmtydxzl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jwnrmuln.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mtedosav.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2etdvjrqm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2myfjenpg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2chfyarfd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2avkdsbkl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2chlxclmb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2plwrsyfj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2fsxxyhwx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xaffpybb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2zpjcqexu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2auhnsket.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lhagcpts.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kebkqruc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cqrvwnyv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbdehmj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uvegnxyj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rdipjjud.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gitqjddi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iwerposj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qspmczxl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2rhecjvbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqjqccol.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cgrrlwsh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xeqdfxnp.html


<!-- 参考信息 -->