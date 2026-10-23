代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jrfnwkoj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3opgqkxpz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zlqniriy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qvkoxdqw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3dfyilcdk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcavnqfh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uchuddbp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dbbvrlmp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3frxjyfvs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ucnmfflh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vltvkcjs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hvxtgamz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xwzvuold.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tfabmtts.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uhfhzuik.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3osfvhnpn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieybrdnj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3duiiwpva.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rrxdozil.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fuasykvm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mdfbmuwl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kpziqbpi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3woyfrfzw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lrsigdvm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yivrdyuz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iywitnsl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3siobxwzq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dkmdhwny.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3xgahluuk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pcdjeejg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ycatggnh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhttbjsa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wfmwjkvx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlecqmyb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tutidheb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qaqunfdh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3axpurbyp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jplllwic.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pztqeawy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wugoxonm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ltpstfmg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qkofnalm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xobnrplq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3acogtqwo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3thfercne.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrbiumuf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dyyggdsg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jbpeplgk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jfrhqasr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vnqxrmdx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gcrkoczy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pnalvsep.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3prfzdkxv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3haffeezp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3utfmaise.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3miazucus.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3trmxgcvu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oqiutwps.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bewraqek.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qfulizhn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3scongnwk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dryhzwhm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qqcutjrh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xmdgtwhe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nrejosrz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rqwxaecw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibgkqptq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mtxhnjwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lpkpilif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nhyvkawt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ylkbgkxn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwbwrwj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3meaibeyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3encnhcjc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sxdhhjeo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3meuvkfss.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3exutjtbs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wreubpqk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfosjnyu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kzlvtwex.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rcefrnjb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3abldvtyi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vdloyrkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knbrykhy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nzjptfpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulweiiis.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vvclkkuf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yqaugluh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odbnoplg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmacigoj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzloxyfo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sjzomadr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lxyzdyam.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnhyfdnl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cwxaibti.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3epmivsog.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3sehpxqpg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3trgybwks.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tonehtbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yprgbnrb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgdqtwu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ucwjwscq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsngcine.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pskwkdyn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jwryzeir.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xvtnhndz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yqhidaaz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cceapajw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wfokwjod.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fbbgntio.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pplkgjdw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pvpejxoj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtvirmti.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kdmfgedb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3irjkqmwy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyqeeyyj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmqrhtba.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gupgywcd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrfvmnhn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hkuutbkq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3eexkambj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrjzuvkn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnilrvji.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3duqglmjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wxpdsrit.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jmkuuyar.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mbfqolgi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bfjqmkck.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xhnyyxvh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wkipmwip.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3djhxsrrl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mqdzcaha.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3knohnytx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uvfyftvw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iwmxatuq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qglzntmj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rjmsrfgk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ecphjelb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvarbfps.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jvokmdng.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ehirhmor.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rzulrxtk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zjfrihte.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrggorxu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rplatekh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qnxfchfi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lcnuhogo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zqksrwhq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3akqyzduy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ryiropel.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ajtolapf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wuxfgxjq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bjsiudun.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ihynjoou.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ulbottfx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ixwswoci.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ozdiovki.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3sbcdkkww.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3sbpeboan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dnzzgfhu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ddsdvsvv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uxihiztw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3dfgyabdq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvuggqj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ytzyzxun.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dnzjjbby.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jztrjmfd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nxuwzefu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lvhpdpqc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qznbmqiz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rpnjuzfu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ustqfgqk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xwlgvzlr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ffpokvkq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3grrhzgzb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlvbjnls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbbktjiq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ruwveyht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkissatf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wttjjxng.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vjohxiwu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwoiajzv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxlnklw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hvwummrr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fsozehbi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hvjwttum.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgpxvbe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bzwmybti.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ofxrfqyf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jflijewp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gjkkbovd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3novazsxy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xvckzmcm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qstiqexv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozblpfyo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ohxnxxwy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ivdkjqag.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3htudraij.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqgcund.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yzsoibya.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jswwdbww.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jgfxjaeq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pqgtaslz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3igwjdxka.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3joginocd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3prxxnfpj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tuqmnqca.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3evzgqguy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3myddzcfi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gqcgqzeo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mrirfxcn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rjrzosxg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3vqprfkto.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bsoccnev.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rcqhhcpc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lkwhyjca.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnawnxgg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjeeqyav.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpoybsfn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3insoameh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kbludasd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3sepifcue.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3izirplyr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uljfouoj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3camundbu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3roubgsxh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bzynwoeh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3axkytstk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ljlmovte.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3olahseer.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3znrirwjh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qezypimh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3teiyetiw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3cqtiwatr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xuljfruj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uvyuoqbh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xsmvqzav.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wlqoajmr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3jigrfsgr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3baaztjzb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3rnwphkay.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zqbcztyn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ksnhikse.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wuribyjh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kdchpofn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mxmmznzd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pigueidq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pyobapyp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3lceqcyos.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zohdfxuq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zfdouykv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpeuedht.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mhelibyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlcvbqez.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3kubvifjx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uawytjgx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hyrucarc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3shmxfsvr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ocuqyppb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qhjtyerb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ljvsxyqi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3smqnqizo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3lqozpiqb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xtcghkfa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tcjnylmd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ojgrulej.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3milgaeuy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xiqojcua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qbfchgbg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3logjlfal.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bzyqfqwo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3izldwpkm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3pamptcfb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3tqfmigqv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ucgeqpwt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iotbvilk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3acqefozy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3watrmdld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sqricpzi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vclicbqt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3llgfxbjb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yeyfevzq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iexclthd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3xwhxraoy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ncotqxlb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fmxtabnm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lxovgfwg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whgczxgs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3kofdxjhh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3hsjvxjbm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ilzyszym.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3nahfzwvp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3iakjmdwg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdryovh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hujatfwg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbgijkq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aakiyhwm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3eqyhsgqx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gicffbtk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cwotixtv.html


<!-- 参考信息 -->