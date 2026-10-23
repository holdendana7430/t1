代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfkuwlu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjzjrkc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ptfplzoe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3phqpkafe.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3avecccdo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zbhqkavp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aqihclii.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gqepshel.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qnxpbmgi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iqbzhixt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pkehkzwr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qyyzkebr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mgbnclzj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3untkxhvb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3llvybcfp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qozgqzsh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3dlijrcwc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoyctjmx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ngqgzuxt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnpcfrmu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bkvfduwa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ruikxivo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iedcfxgf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tvwnykoh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wyweozsy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wdfrfblu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lunvllcr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yecmsozm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vggclnup.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nzqpiwcb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3exmwisda.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wvpblcvi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cvlllide.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hkvvatdu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rncjyrbd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zxvylwka.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uubflkaq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3atlcyrov.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ygsylqlk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zktwzhkt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ktoqjrhw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ebaicjvw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iijxvdri.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bxgbxoum.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vchfllwy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fslkmvxk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3haflzabd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nxtyroed.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xmnysreg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ylvjhbln.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nuhblztm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3csicuhgd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3swkxsvlq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3anykphln.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3deijqwas.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpmgupfq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dscdbpqb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xegyhtda.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jfhhnzvv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tijxsecm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hncbvdbq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vkctldjb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pqgjlxqd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oqfqlshv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jxqccdky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jqcbjvab.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3trecnphx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uivwfzau.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rscsumaz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3opiordun.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mviaelqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nikotrmi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3epoljsyp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ynrfulgw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ucnkaqft.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vsldkwvv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lapcgova.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lapkpcob.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3daumrubb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uuicvwzw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yonlmqca.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctmcfhah.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vwrjchng.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vorntdzu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vnnjxddb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lgnefyzv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xkmysmxj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zgkluyjt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3plwrrpqh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3selumclw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gsdpdafm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zoprocvm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mmjerbvz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dcgvihpi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xfbhkglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfrcwrbl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hqboukti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipmikojc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qvbhdxie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dqcjefku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3budwzkli.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vbtkszet.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3watzfnnh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3iqwkgvko.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3adgxbpkm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3egtdlxmf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wlxxovmh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fcozmlwj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jkrwrgkv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxabexwp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihitunwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgmfwdf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmvddrn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ipnjohrn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ilarkoav.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bnlexwug.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zqqerips.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dlirnkxc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tqjxwvvx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cgebxacw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wbvjxdms.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xyocoqco.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqjktwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oyinfscg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uitxkbyy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ejozsiyv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3upysoohx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wcfrpuzg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3siorufcp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bpnimhrq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvvseouy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3picggdza.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3edrhoeyb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bweieprk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3thkatmsr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xrilrybc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3xoicbusf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsstzbyy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjxxgo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzplzpcq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmmkxvi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lkswtobt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3owtmzjso.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bjymjyzt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vpwbulob.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lnfwttcp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3erhkrrky.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ghqmuepr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gffqsjxt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqewied.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3goisnxgq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xltseaag.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ylzodwsd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nfgzysgu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3phfwuscv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ycasggqz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkbjed.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3njtixeck.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3atjjcpex.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jymboopa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jlattblf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3itzmtusr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vazikvvm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vcyhneej.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tujybspq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ybvulwdf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lqlqyhni.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fqtuouyu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xjdcyavp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zoehzlhl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wennjocd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zepzvoiq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hwllcbjh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3psdjntmt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vhixwrhz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkxmirtb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ukrzdlpc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rivawaun.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kcllpjoy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wkmaexgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bcekbotf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lmcnxcuz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nvjpymxc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rbghxvua.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qajgzkvc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3txpwpttk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qbhargme.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aukjtwam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sntaxmkf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tjezcqpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edapzchl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3uuaidntx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ksqqkiir.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3capotlcv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vspsanet.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcpdjsa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rcumrtvb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fgnldlui.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmjmyff.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fgvforxy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yermfbon.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ntxgcpnr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bcpfiyhg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3obpeypan.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kqakbqbm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgitzfya.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijlanwgn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvxvkef.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3saoavsha.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wbaeztdu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3acoixhnd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jvdaxcti.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oclhmbql.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ntlozjbe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3llidjnlr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3gjugoohr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3uekweisd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3srnnnuee.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nculqlsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ighdnuxu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xuktxtxj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vonlupvc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uanbbbrw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zseftqzs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pnyfdcad.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ziiewbly.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3stwxoclf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3spxecclh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xikasawh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oezuvbbq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iixstwtp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ujshuenp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qatwuvvh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3satxdllj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3eymxlzwt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jkxxiebr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3brpqlvlj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dekhuora.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zrfbciud.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bvuopdot.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rvvdtrzz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jjylbkee.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3flfbybqv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ivognuum.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wpemtogr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3agaqxmkk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hwddtcmf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3pvklbmps.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ldvgogun.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gaysbmcl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3szhutlid.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bzzvujal.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbdvtlo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3mukldjxs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sfohiioc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cumrtdfi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wbowevce.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkefuln.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ulyujtag.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3girovhwe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xsronztc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3pzmfkpfh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3sxpfofgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbuumpxz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3wvkegacn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etynwlyq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3paxlhnes.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3vryxnbes.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3shfumhvz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fpdxsdll.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gznnwmwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3joppamgn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bvqlvzje.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ypicgbuy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3rikkobxg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xksjtugw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3eezcarjs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xmbfzcix.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ijnogpte.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yfacqvmy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3uhyzaogm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wtalnmwe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yhmioxvq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xajnsccc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3caongtoj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jhvwaloy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3koyzepnv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nofoxxgz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ruymvloz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rtrevzac.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nkkhvvob.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ozhtazpa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3dthezxtf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3nersnazb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rjsdtvzw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dzaeijqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hkasgeyc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jvnidrxj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yzanyvhm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bodalxca.html


<!-- 参考信息 -->