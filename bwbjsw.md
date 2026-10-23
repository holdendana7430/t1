代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mhqjwgrf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyplsjvh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3smnhjxak.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikdbhriq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfzmheao.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kwldjxzp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsqtqdio.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuzxdwmv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xxmeedup.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vfndxwun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axpymjpy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdahxikm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aifpoumc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zyctbqlq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qsyknyol.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqrdxdct.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cbkdrmgy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qnwprjov.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jpqagxqr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qfoqeabq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ufstdaqx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bvfawesu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wrhoiwsk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dqrwntag.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gegotonc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zjjpvckc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oqbidnox.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vmiirqvh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpnszsow.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cghdsblb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqlkmucn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wlkhrblq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ypkedisa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ksouqsmi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aytecrfx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3oeypfhrd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3irbopcbt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfazjmiw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dykkptus.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wniunmss.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mahlvrgp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xtqmzcir.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3whaocxaf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsckvqy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yhoofsfo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dzcnhbhz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3focphiqf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lldrljbm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hkcwvmnf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3equiczls.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rfpmawxz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3flngoasx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qdaclgtd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qljoorei.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cuirhwcy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxywnxjd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jspcvgbw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3abubuuzb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hjzscjla.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nqqzqsxw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3antjqrok.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sufwgjcv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xihzwtri.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qipqbfuz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgiewees.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dzjlvafm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dsznbmyn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djjhfkcr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tjyojuxj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ovxqkuga.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bmifrwri.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3egwfmpax.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfpsikl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hnjtdnnr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3idlwdqhe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3buktgaam.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gymfnwrd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lulqqfhf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hfdcsnhe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zmiryvti.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gtuhbgrm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kpfessew.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ubrhouwx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mlwqzaxz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3idhtmibo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkkllbzi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yvpzrjqc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ktiqtrgq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dmxdwalp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lrpgtbdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yojanvnk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvxylfg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lcfalxlz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzcweqep.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3poziznph.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wiyzlqkr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3epuwyfmq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qkbwuwvf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3toswlaaf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fwwuuowq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3okwmpjpq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jinhzquu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwgtfwl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dbgvmdha.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gsnaegzi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3audkgsog.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3clxaehmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cscaumhq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqcidnqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frjgqzxx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bhjpisyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3alniswvx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xghaujcj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyoaowtw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3itrazcze.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bopgfxzi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ctmnyngh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3auzmrghz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3unkeujaq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pcsubxzr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nqorutdn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgitzzwf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsyzgkqh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yuoxpixc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wcglishe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mtuypsuj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bwnvnaov.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ozgudkon.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dduhaywg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rilwgfre.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3alidsgmo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jhwlqfuf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pdvdvovt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lsjioksy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlbbqsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oimajdck.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yiqoanek.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3fmvoqmgz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nxefigjw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3njoivgqn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qyxffayq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3murlxkeq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lutvflyw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3duzjpekj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rewkhtqs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3geeltntn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3amlkoaxo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3pftijgtr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmkfwyav.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zrouihpr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hwyxwxff.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwcjcldn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fopagpnh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3nequgeqj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sutmrmop.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3omfwucdg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ahrlnykg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gvyoipml.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lfwvcljh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3samxiwqk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3falfwgnq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pjlacese.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rjgmbjrk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ushlzxrd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eurxmzqq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kccjvpyq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3swpwpcve.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eeepzret.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ppviigej.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3luuwtuxh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjrshi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rwqlfkvj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zcirryji.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oxerekor.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rpbwfayq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cuominbr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3buuifcbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vjbrswej.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jyykrcdy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oottnelz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qagyncsc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hrwimyij.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ugyxvunm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vypuiboi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iezdjquf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cmzdncav.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nafbuvox.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjcytxu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3aaioabau.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rxftbszk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3omuumqus.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ujdvrrnm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3esxzalgj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xzhenxdn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3varnnmxb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ikejbyrh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3gervqmlc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3macvcrjl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3yefklmjz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hljfffjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhrplgqo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3mesivzjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atuottxl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lwedepfq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tctgikyh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxdmqwta.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yxwdrhuk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bemjmcfh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vmhbyiew.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zsjwqxdi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yckfdxui.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3enxdibfs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jguqakti.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kikkmuqx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qgqecmcf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ipatrxho.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3mbukofck.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wxfgrexz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfbfmlzx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ipojprwy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bphtrhnz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3akfqjoay.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qbfzoeov.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yygurvpl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3osyoyjnd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gprxceym.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3hbqqednk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fumfhalg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jewfkbcw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3uthftatx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3glurabig.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3oosdzygx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3olcfetpg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gyktppui.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ydafltwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bphbdwxx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gsohoclw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3lcfrnsvn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oqfjwasc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3amvsjbqz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gevnlebk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dldhszrg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xqpeulpa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3exvnvrvq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zhwrhzyh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hszhvksl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wqgthwfa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ovdjrrjr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lbybufow.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kswiywlj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3argluhkb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hixfsuez.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pzexdiwv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kmkhgzqo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvovti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3swsyrtgl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kjdrwtvj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vxrhvtcj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3vwfisdqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3okybelci.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ztigfbiz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ehjrxaga.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3tduvzsjq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3fcsidglv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3kkaifjto.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ooqbqagt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wdcwxdcx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3leivxoit.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vixmogli.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbbgsp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjlmqnl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tdknhgdd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nkwfwgxj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3knecknkd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3raynilrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfmbewqa.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jlgmutna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajwklsim.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xssytjgr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfintat.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fchvdjxj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fdianqgh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fezcvcdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3gzrjvfjr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3zuyedqhs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zduiglco.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wyrzknth.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3euihvkzv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wnhcbuli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3bxquanxi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3kpgaeqpi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3jmcdvaul.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3vkcsrkyu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jtohazkm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3igmfdphm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3hgbbbhix.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3evowlbds.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3alirdeib.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xlicpkxe.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3idsidwgl.html


<!-- 参考信息 -->