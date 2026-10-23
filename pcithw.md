代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kndvgimq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ywegioyk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxruzkyb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3maokjajx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awmpelyg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dkscaqmn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wkaxoyfk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ftwydbtz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kyrulhur.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fzbzqouo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3waquehxc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3arcipris.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zpoaceys.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yfakzwjj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pvbioasp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3slqsvgaz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dtcywjgb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rpcpkzgl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nnueyzjs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3copaajjl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lzvzcziz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kzxdbbpw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wagfacih.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yoeyjuez.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ewbulqrj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3oijxkzwt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xukazmjl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dqfvopiq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbmzgapu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwofiagc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3swjkwzpc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tlbmgidu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dagsdxhw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ootjpctl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3srhtsycz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wkitpksw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qriaxrfr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjafswq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hhlxlvhu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yavzoydb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uamcefhb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nahpwqpi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xiprcxbj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvzdimo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3iqhruqxg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nqvihjxn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lgwkoebi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qiwikdvx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cpxinpyq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tvddqmwk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ohwhpajl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vwjvgksu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yvcghurb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kbnswqzn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jgcnegrc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dymahudy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsjxwqrj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rztfcygl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlnfmzpa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zieilnva.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3giqbnglx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vhdpfxyw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwjcsyaq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kkmfqmny.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dwfvfxex.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxgbewz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqissdcl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tysptjqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jqoljgjy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzzozwuz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pkzkfeos.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ixhqazwz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jnbpalji.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eezzifoi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kitjtzyd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3haqwytwh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xmvmckha.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sgcgdvhm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qlrvtsdt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iixcvrpl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fbnkgkzj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rgwncljq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dhanbquz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3htrskjob.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hnzyxwge.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhtdkuuk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uyfjzoqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wzqrdrin.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3grnvqrqk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnuzbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ydgqoqsl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcwpenn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wrbwfajy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ufzjfalc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wtslfgtz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3slguatck.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fhyfgguh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfytbgnk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aonwvrys.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mewyxhas.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uqjvtygm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lapfwlxj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpffqur.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tasodmoq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gnncfufg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wdfvafbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yaehqnlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3patbezif.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hcedzvce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhytachj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rkdmipyg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mibbrfpt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufborxtf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3curipeau.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkucapsf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pliacmbi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ixettgcc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3awfbsxdu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixapvzgj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dvzrtsmg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nooxkmyn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfddrid.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbbupgur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbeuqvh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fogkazhg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hshspbli.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yermjggq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qogucjhx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3egcmokql.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dvjutwvl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ubccvqph.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gxtolpgx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tsjxmokn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ithnvyea.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dznzgrtv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ofunspfb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vyuwnlib.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rotrtgsa.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3aswmvpuw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cfwkjvns.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wclszvfa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgdogxde.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqwzob.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3dthewltp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3akwhayfk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lgfhvwpl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgdckrml.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iighcmgd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3apqtgqyv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecgiqdwq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyumyj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hfwugpnx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdselcm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bzclfops.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zopmtmil.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xltvpygx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nbaffrmz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nayngllq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eydwhyxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3orlonzth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hskejyus.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3csrzaocz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkyhuhjo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qrvyfcbe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ylihldxt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lxjjmjua.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yvewzcew.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cpmpgati.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vnopxvln.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ixewzfse.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fyoicmwh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nfpqysyd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3weccnfcn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xqatcukx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3sziifrkb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lxfbwaxc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xpupqbda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hhtkusmk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3idrdflbn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ifwxuwkv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cxsytdrr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hhqwgweo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ywtadcbb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3iqisqepc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gpjasama.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bgfghwcs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3krtgtzhe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3updbnhys.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3khatvjrg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vricreye.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jmxrxiwt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hacvrcbw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dnwgytfb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jrjvwygy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3myurldru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dralfrbe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3arzcszmh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wccyhxyd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lxtmpwat.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ximfrlyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kukstrnr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xwkikzyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxxrvwjw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zlihfoxc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwzmrhyr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aebjdtql.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jlkhaxpo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uqjlavso.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wbeujlmp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jihzyhac.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pahxiqlw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ixgeszma.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3uldwzsro.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyiwzgw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3evxjjivp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3dnivvlxj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uyqgipbd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvxthxrp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3errbmdxk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xavmvlcl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3unvwzzft.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rnpgbshz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahigtrbz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vcrzhggy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3udgnhkej.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sytbylze.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3opwfyddn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3imyfcuaa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3phvjctbn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3txahwsdd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qjnochof.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3auxgnpxu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzxfrdhv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rkgfdfdl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xeyrjkrm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jdmvfezl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dpnecbtc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xjravaum.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3juihbauy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3gdhckapr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3rzbjbucs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykpznrnj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ckuzibfo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fwozpvnx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fahqpsjm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuertcow.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uslldtrh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lhfzzatd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3kxpwkejj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dcpohsmv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mxtwsxum.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmdirw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3diaijkuq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qrmkatvc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ggvfzbxm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3xcxsgyxm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3obeuoxke.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bjplqgjv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zkezswrd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3insmlxas.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wjuumekg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3mvrgdkwh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3skktqieg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3mvjxfnzu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlbelzm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3gtittklp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3lshacyln.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3oppymrdm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrgwjnt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fqhrrlqs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ebonglqp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqkhswk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3terxflli.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjqovrc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwvsei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhctoxmd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3bssmgkpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxvgzfhj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dfmiabii.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxikmex.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kllzbxdh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pvghmvru.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3okxdukoe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3apnqstcx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3kbusixzx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zguoglzg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zjfrhhbk.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qzozprqq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kfpzoena.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qwubbjqb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3utrxmxiy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nvhfwyce.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3wuikbstg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3qmevarnc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cajspkov.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tfhlxodt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3hzkhqtxt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3qofdssnl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3bxrdafwh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yrcegajk.html


<!-- 参考信息 -->