代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyuqftam.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3feypbvzl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rhujgywu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ueggdppo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ffpsjxbz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fasdapla.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xucttavn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zrphhtkd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iecrezxe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pobpybsk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qbgtfhnd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mowjoaks.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3baddeibu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vfemwdfy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rcfzlptk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qxhesjct.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cremuxuq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qspzbjkc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jpszsonl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cvflbcvj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xrozlrxq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fbgkwntn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tidzhvmg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fhbgovwu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkvhamwo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqesbdut.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uxlfhycw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mbsfqdei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3abasrhvr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pthibnzr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndegsgxm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bcdobixc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qncbdjok.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qypkoxjy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmthfx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ussggkbi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twjrfoys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdfzskun.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ffrcuyub.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpiskke.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ikphvfnl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3croikuhj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zdxjxyjr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vuukmett.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ppxqrjdz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jrzuvwyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3trzieynp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ltmjmfhm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iltywcvg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xhpmeqgg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mjmqfalf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xrqskwyg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mfkhsqxt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjizvvas.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtuppxpu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xlmblvlj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3domgijwc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tbdrbdvx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rowspqbm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mblszxzq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvetyrpu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bypotede.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdatxnue.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3znwitgpz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ggihbogu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3blfjhuii.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lrhthwei.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hduhhvdj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3byeqjtbm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndkkptjo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iyznimqb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wczhqmwz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dwdddrlf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sxklyhbb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bzefdiae.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kqrajsgp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3sbittrpb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmljft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3abpbrudt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eljmaird.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ubrwwstp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3okpaxykj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3edykkmby.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mdomqlqk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tynnzrpc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fmvqqmsk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rehpqfym.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rthregtq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3miasebhq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxwpeyrh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gsrmvqts.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gjyvjuaz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vfmckfzm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3atrftrfa.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rqceijyc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vklmbkvm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3emsghtfy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gneawyga.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnopfwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3toexxcaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kvixwkbo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gsjvjuat.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dugbmutw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivpakyqs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jtthbpjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khuhczmv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ylkejwkj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcguoow.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgkrgjkv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3emhkuzlg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkgnzpof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tfatkuvk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vaihqnui.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3aprcgzpi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjtypcxi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kzupbebc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3epcwfqjf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oeergpra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdgwbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwlllrhu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ecxhuvnd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fdciepkr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3swxpamjy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olfqkllr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kzciczax.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dcadffuk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ogjybhde.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qoahszzw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qivaardu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cjofjpjh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmctsne.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bhyujmza.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xdsvhdmo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vgptakgf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ogddsuat.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qpwsufey.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xnavfzxm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uchcloja.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wparumzz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3soelukfn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zazticlc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xvefnosr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcntwffo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wtuxnuro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3srbqxpyb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mfriojdo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bprmnnhf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qsqyrpwv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3srtgzhvt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3sdkviuge.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vprafszy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mpcqnjnh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oskknjjg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fytwnoyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uraamuqx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3umabgomp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3sqwvvfiy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mdctqfka.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3geiufakn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3etnnegdq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3bqjhferj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pdddtrnu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgfwnmla.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gpeddjhl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nsizjwza.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tcrrmnks.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wgsrzitd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ynevvyds.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hutbeynf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jllhsvky.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wwgcozgu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zdaobmbg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3spjorekb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3woziecvf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3eqpfjjpp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wlodvggt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yhpumfpd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fgtgkmaq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dneranzy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3udzvqicm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uqfpwjct.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ibixbkls.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ritattna.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3axrikvkx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3dxixzexv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vnfdabag.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3iwcasghi.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jwkatdds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kwmmcvnv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nnfvotcx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iuzjgohl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kpvyqecm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3owlhjqll.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ewtfuqvy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wpetslkt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gidingln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvzeaqre.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tikvrlye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isxbkhft.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qjzztjhh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsefkpmh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3szxxckbo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsuieok.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abrgmvxa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zrtjjjct.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hbyuldce.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kheglivu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3swoqwkep.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3escpnoyw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lxevjaua.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ivfkhhni.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kpjhxtiq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nlwtcsuq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrmjcpsm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3scaduucu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zeliaszy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3itkyuavm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dbhmuajk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3agahjdkq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jswcaukw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xyqfirgn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3gvqsusfp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgzvsru.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3oaihrokk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3stfjdefq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hamaoecj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bjbjgolk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pywibopi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3edgyyzgr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vjqmozwt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gmdpmxgl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ohvpwnyq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qxjcnxrd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3smidgmen.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3btgiyezu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bqcrwpec.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zksyaqur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ippxwvnp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxpetdl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rigetsjp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cwuidcxq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uflyakrd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3njyuvtip.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cxoyzhek.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3efrvitql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fzbilcnp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3pudcorsv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ayqdgcfn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3smnogonq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mmdptrgs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ateytite.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3gcofbzxq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bgnfnges.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ihekpyyd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3benentkb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ieqihqmu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3uujygerw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwgysk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3soajaxae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3caaexnlz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xunhcvug.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3xedluhtf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qvaglcim.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hcjfitad.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ahqsqoic.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxfjqfo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lodojmpz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qvplxlpw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ntqistgm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3unhkxmcn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nvkunkpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xiledvsx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ssdkssiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xakvjijj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qqlunwbt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3oxghztux.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3seegdboa.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gczgavuw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ltamdzlt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xficvmur.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3txaaemil.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vftsnkbd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3utmlwpgh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nhxyuyhz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zegzuaze.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qfazqhwl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tphqclla.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3jdftlmqv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3obqkessa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3gizcrzai.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zfbnuhvo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrotqnf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3pqxxdihi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3kvlydtzh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3cvepxubm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dkxxiidb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3eyjcdbgj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ptolgwtd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ifrugcmw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzreovv.html


<!-- 参考信息 -->