代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zqruqikq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3byojdvid.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uibcndsq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cehpxrey.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjwebor.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aollhone.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ottunnlj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3drnarswn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hdskrjfj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uabkkzkb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3whmsqolo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3psiibdzo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nprzytom.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jlglphxl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pmgdntjq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ebtdgzhb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hleafkrq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ursedaym.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xyvegsju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hndwzviz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jqqfnryc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wclilsqz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kighysoj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ozobtvea.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ppepudzr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wvoxxdzt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kctdgbso.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lrcxdwrw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ayyukgyi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hlybxvwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3firixouf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueyebwfb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umjxyipw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyalvtnx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pvqjgxlc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3umempuoz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yoghepnt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vxyzqywu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zvyrhpda.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3rfbxcrjo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3buutpdlc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mafimykm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jyslcsri.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgbxoq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gyumjkrx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vznbyhye.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ohigmznm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aakjsfko.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzpmrfrj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxthursx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbzmjals.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aoykgagv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vrpmxmgo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3utjmndpe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qoqtaajo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yjxghqym.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jmajipnc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueimnsmq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyjcuold.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3prvxttpe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tslxiira.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwakwsqd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pighrjus.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ladborbx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ulvvedkj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jczjclsz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yarcstvo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uszrchlq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gwnvkhci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mchofjes.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvkvntb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qqwdbozi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lpwlqvnf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fcewlaep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uvunijts.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gvjmqkao.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3defgwmyp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rvcmtves.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvrhwhi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ghrflcwc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jbbliwlq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eljcyxev.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfqppiiy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzjjdrl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ecajllla.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3krkfuvjs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3asqclhvt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yzysyssa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vxomgohk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xuilulsm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mhpmnsqs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qcrdjlrl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kfckpfrf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3alsiaeuk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhdtujc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrmozo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wbyofpil.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jmzmubhf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yrmzvjmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnthqxfk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fajsbshr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxmfbwzk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3shldxjfl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qfflrgdn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lchrrxac.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qqfotirq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ecjorfkp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvnbbygd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3liufhviy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtyoabyh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3caeooabn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ufsznfeg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ziqycykd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbichdnk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hjlkkiux.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eurxlmkg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnovqxas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3avgdmyye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fabfxsfd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3edmbmfze.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3neqezegq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jyargycf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lxqguadk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uhjgeplg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ovdeerca.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vczbzsax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hthcbecj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rnbipbxu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkhvjcye.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3flqfjfis.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fmywfblq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xpybdyob.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezbwzmgy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxnupkol.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kcvtxwwq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vxnfeqeu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nviqkeyy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dsgcgmjq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fnipdwht.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xkqgouhj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sutvfpxh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3botnlqrm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yepstszs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3npedqdbk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kvcjjfym.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jgtykwre.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrdzdioz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xvildwch.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3unokkxmr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ttcbcfwp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jxsnvdzg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sjuvuazg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvhhpx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3fbziezir.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3iyfcppwl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hgemrqtc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zfaxvljs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3exyubnqg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lanhawbo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wssuvwbm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lxiwklgs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3gnigqynm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3arrwnhyo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eqqyddgi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jateclne.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zndpcihy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bnisbmtk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tilquejy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3klydgfzj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yhgymmvq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3umrvevpx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3tgapzccw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dwtewrgl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fqbvfcdc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lqpdalap.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3olmcgbla.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vktnhemj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3infpiwxc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nkvapbpa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mtsfeqdr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mcerdday.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ukydrhql.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lpxwrxbi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pubhlepm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3izfcuzat.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mzaagmju.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gybafckk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ziiawfbb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xhmdoewg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cgilfvok.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gylhpssj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jcjnjxqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqybpgdv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3tevaogbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elsgudue.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jkscepht.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cfuravwu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3crdpuumb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxzdfjsw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yevyxkyc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3sqzcwftz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owxrrnka.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpvmjwo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dtbjjznt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3prtwvloc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3idrupwdh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3knpgfffe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3blwzwnss.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qgxdkpgt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hyjvkqtx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vhudkozy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wotomxxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3imztedvj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ighzwfai.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3kknqpwem.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3thgvlzzo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lgfmsdqh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dyzobxhr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fawrfvhp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3hgnjnqnb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3zasoiwbs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3pslvnayb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lfgtmeoy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hohsrtfv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lsebpaut.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bmwalode.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bibnsifg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3twkchmiw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3akdfmhwz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3udfvsrjx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3icofxhsx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3olmiwyfu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3avqatxaj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pomzkzfs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ysvbhtde.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtjdixj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jblwkwsg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjymhuf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3quhprqar.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jktzpydi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xycfkion.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3logsxyqh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xylgxmqo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ikfklmxt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ikqbntpg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bdeihpxg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nutsaizw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qkigqqai.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kserzrjw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcdhqlwn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3slccbdgu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rcwyzjrz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3psvryvcu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3fpxnihox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3unwrmjaf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3kvvtqurt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3efxplwjh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mhougbmh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3awtgidka.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xvjgxory.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jclnhpqf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zlmlednq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ddtzpgaw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mkuudrqz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3exwxfhdg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3brijcrki.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mmdmidwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edryqnye.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3pksbxjmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djoggmgv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ztrjdbdf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qpnpunll.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jtruvtki.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3izmydknu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tnpntisy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fnmohoot.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hmhgwujh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3fgfajmic.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3uimxxldx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3appteyjp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3civsxrrv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cpvkqqwg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gxyvhnug.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3esgqlmgb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vnykznli.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3cbhexweg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3squlgfly.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jlofjxej.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lajyvwlf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3qhohdcvm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3rqnuxwpa.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3faxcmwim.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qxovukgr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ylicvjfu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vczgkifg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ohzbvmax.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3elxlkfqg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3drpaudng.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwsemss.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3mgexpijn.html


<!-- 参考信息 -->