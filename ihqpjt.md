代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecltmfil.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uctmitws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ionkddrg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3aviemjbb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ckylnaim.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zxtvgojo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dhxfrxrv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tiyazjgt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mqgpnjtn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ntmjemhg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tyuklrai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3spdmjzfh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lcjpoovr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ypucwdxg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gszietqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3thpsrxon.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttahfbep.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvafrpsk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmthaegt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pcqurhbu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hiuozgvt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3masnwnyu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cckhvjfg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yukhnovz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xxpwxfxu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hifsibil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yaxkongs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3obvffkep.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gupbovns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zyggqbuq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugwtlhuq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ybyotdfm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lisqggti.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3oscbnmnb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ekgurztv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3owewatlf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jqwplfek.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3deeiknec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gvzzdrse.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kvcrsljl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vmvqzbsj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bsnqieib.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yzwakwfm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dcdyzuef.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jknnfkij.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jocneqlh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qkgeiria.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mdxkuart.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3thkjcsin.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3phcbyrmt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nmsxkcqx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mirihovi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gocwtwct.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3waoctnha.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3elghynzx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pppvkwxe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hekmimsu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lcuspwta.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gmwgwybq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ajmejiuq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wlqhtmol.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3etvnlgrb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3phbcqoyq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jawohuyg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pyblhdfr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtdmcv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gwqkfkrx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ppgcjrxa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oukfaesj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cgbvnape.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3omxhvcjq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nrlcewgt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dlihvjbs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3apasupxx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rlgbhqbq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qbvjeelw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yhqlimfg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bwdknlyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ngsffjvp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mbequdhd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3unomyoyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqfwjbt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gqefduev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqnirxn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3clxpfpft.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uucgyztz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jbodhnbc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gqptwgmh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3afjeksuq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dldieahp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmonast.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qjvwmqqs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3epsdxzam.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pjbwtlzt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gwmjjgzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbxinwpm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3eyntcyvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxmpkfou.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ocurxobt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgyzmuu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fupdahys.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3elrkwhhi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwtqsroa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3herwkmuw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tjiavaye.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vmdublcq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lpwgjill.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fsxxjrpy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3maifbndl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sorprjed.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcpzzwmj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mdjlttmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vrtyciky.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3krlhrety.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rwuqutln.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3msfmgsme.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xkpqmoiq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qllnfcka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lgoggmkm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3itbjatkm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idregpss.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mojoedrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gwtdaldb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3phoayfgd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qjciewqt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qdyiswrn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hfmyrqgr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3siwnmfzs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qphhvrrw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ndfxijzl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vjdaiwkp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vzxpmaik.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xwrylnlh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3frglibyr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qruzdzhd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vweiyrgm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxaoiiio.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwpnraxw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lotvnheb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rqotzakm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3itapykfu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ogjftsgq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3poljyfmr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yijboxhq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3iakxxhhm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3flhygiie.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qfbmchmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eitjawwt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3roywloul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzqdcpu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eqokvpxv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxecij.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mitluawq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fnuzflpo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3awjrdggg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ubkeedgf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktcojhsz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ikjrnvph.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ykuspgyy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fdrfjwmo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3flqrzmqx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xetzztrn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fsimsqwv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rwwxykcv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hieudjct.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ejkywixw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dhnjaiar.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mzgjfoyr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ztujdumz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jxmjttwq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yfzhhsml.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wqbmspxa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hyhblzge.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3eoujwftd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cwmspcus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfeanldn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3kongzrlo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zwutkizc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3smcwucmx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yhtarscg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3kaernzki.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xyxhjrcp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ydokhgsd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3teuurmce.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3veleflgd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jxavzbwl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3yiizvzuc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qrkhwkur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icaneohl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gqffifbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpwuyeci.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fdevoyri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3skljlxky.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3exbrksga.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3awolxcgk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fnizcwvt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ngalgbya.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pjejrjna.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3njnyrrec.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cplxtrbo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fjdakvuc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3puhdcomw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ttowrqca.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3veiqilft.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3wygeetpa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qglpfkab.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lmtmjrir.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cilfskxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywluxapw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qxnhspks.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3phynmdsp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vwduorle.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xsiqgwly.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3aaordsrd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3yufnzlwe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3uibeggxh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gefxhywp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uorxxxeu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zcrjhywq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3giagneyf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxdjmxbs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ijfvhsbt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nshlsnzz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ukygflch.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3knwpdata.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mkixmsfk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dzikzdxn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3afgzabfo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3huxdmaas.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mobgzgqn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqbisin.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzfoovzd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3yvluxrft.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ifjhywun.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zzhihqtx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3vfynqmau.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3yhghcbyg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rdtddtye.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gdxtsgdu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3emgipgfe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ukdjhnfw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wrrpicmz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3lkiriaqd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rbebwquj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dchfnfej.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3cakepisv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgdjdkt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ttcargxz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3httzqzck.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3zurxifur.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ixudquuk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtnmtn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tambxknr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kvgpkwsn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3satxwpel.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jqfbjsox.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hcupseva.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3agpkfkpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxvifaw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3arnotsms.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3hzpisfpl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hvyisuje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fwfyexdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjdixphc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3iesldggw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kygavmgu.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3nckigbqe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xjsjvnsu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ryboyhpl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vuaxhtzz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fwpmvpdk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cazfetnj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hwgaludv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3hmdyomup.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3fgcxiofc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mprectsw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fgjlziea.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3yttuedaj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3olqgbspg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3afbvxxyd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lfiwbuxm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mrrnrdic.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yalztnwr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3lkqowycr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3hlceoaho.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtfbdwb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xjqfhwrb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jbvdijpj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xhsarien.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3muyakrfj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hawceaet.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3shokawfl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3humgrwxm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3logljnnu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sxusxfjq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ryirfewm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzlckho.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3wdwbgrtp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3fdrytfnn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3iyaawheq.html


<!-- 参考信息 -->