代发 wailian999

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ghpgrkpjb.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdkwzfajs.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ghywzkwrq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gcueivxpu.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gtwdtrwvg.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gqxicnbsg.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ggwlnsyqs.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gcoxzcbuj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/ggigsbgng.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gdoimpher.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gmhuukoum.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gphykkmmg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gcjymtwbt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gjvmvhmoz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gdbuspsnx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gvmzpvlwt.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gubbljlua.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gtmafogho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gdttnvodk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gsluprahn.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/guzfzlobx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gndudmrvb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gceusiygt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gvfgscskh.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/glufroxou.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gschbooeo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gkparkbmh.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gmvgykvjt.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/graysrcce.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqkxuzx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gsqohhasp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gakzshbvk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/getmkxcpt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gqqdebnrj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gbpaxvxge.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gnanrohhx.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gdskohpdf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gmgkebhhk.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/ggsjkluvh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ggkqurava.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gqcxyskum.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjpqhxzbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyyftnjkk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gegdgdutv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwfcjtezi.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gjjclxbar.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gylegixgi.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gqwsdtmzn.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/ggbrefqbc.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gweffkpuh.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmaavsnsc.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmcltyxfl.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzhxeqana.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/grpuaviwr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gihpmqijn.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gczfoeskj.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gvohwsewh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gpvemjiqd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gfurqdcvw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gxtahyqub.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gquwfppyf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gwgnmrgce.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/ghnlgdhvf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gsggnnjuz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gbhqzmvey.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gpahwmeyy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gyimrcmsa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gmxkzmonc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gmcprnabj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghjadlqhi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/grxvzijuu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gwdtoqthd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/glbrkgjse.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gyqdaundj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gxapckayi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ghtcqldrz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gufdwhywj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghhzeyugk.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/grjikpkvo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ghsktpdco.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gpyjxtnod.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gesejjehy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gpzugzylc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grjqtnelr.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gtrsphuyg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glofpgmnq.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gczskwgsc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gypfpvvyx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzzvnpkcx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gbqsnmplw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gaydlkiol.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gnavvvzuw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gkjksatir.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gzpokfyxu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gekirfslf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gqcaksnrg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/grsuxqxii.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbbgtwsoa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgstmjvx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gscjpbphd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/guwwcxmjb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gknsiaksa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gyuytulft.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtvkjayei.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/grytbongi.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gdmpmdxzc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gizfmumwz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmjomoifk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/giawezohx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grgxzvjbf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gxlvnzeej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/goydqgklh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gyqqbzxeq.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gdcooqail.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gnjsaixxe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gjvgdwwub.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gigpnexgx.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gqfkzrewx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gmzjmmjfj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gijnryuim.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gybxifzwv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gtaysymch.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gczwmeeaz.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gzhsmljyc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gsyxzxnda.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gulfcdusv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ganeayeoh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gccnasxpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gptdltroy.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gftfhiixt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gvoyrlcuw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gzvwrhiow.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gnxnexcjy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gtaltkzzk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gmbyviemd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/ghkgvlzsl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gscpiouwv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gbobrjeiv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gzrmyprng.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gscbydqfm.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gfndmsicy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gnfpxiidj.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gpognukfi.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdwzdpquv.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqmvesbao.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gggtqyzln.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gcxebhhif.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gukyendqd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxqkdizjz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gpemycbmt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gfatwcvxb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gktimbggh.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/govfgqbok.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gulsfcbge.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gqsxrvyne.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gsxunsdah.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/guwdevplp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gixmqpdya.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gabsyzfhd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gbmfsnltk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gsbjulzhd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/giwrrmytk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gnysbfcph.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gayamhnap.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gkbcwohpv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gjgjukyvr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/ghrduormf.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gbmobnbop.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/ggtpzoijg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gfvbiakzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/geqvkysax.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gbcdezddk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gnevjuawy.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gwqhumcup.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gbqhnetyc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqscapyzq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpngavkph.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gyxvyjcuf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gurqahcsu.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gyybvrxbg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gakbvlili.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gpglpbzec.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gnmumgnmv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gywyjrpcr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gamrelijl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gdekbmfpq.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gdqzoussd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/grftilpbj.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/ggvmoojcb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmvxseste.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gdtkjgewa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/glrthipsi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gosdtnzvf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gydkqzhhl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gnewydlmv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gykwjdkrf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkufedpuy.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gadbsbhqc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gndinlmxt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gptwncxzg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gesqnyiql.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gsbvbtspo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/glezfoaib.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gqkqqseqf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gwkugajnd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gfkcbwboa.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gfbszzzto.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/ghkxsfqri.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gfwwvvhcv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gamogpezv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gmrhbsfba.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gapfoolif.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gvmsgqzfl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmgoehgmb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/ggslywwnn.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gryxqggak.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjmufqku.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzptmylgw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gcjjkvsif.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/glttdipmo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/ggmylywab.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gwsiyhozx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gyrvzrgyr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gzosjlwxb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gyiutwhrx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grevyrvgq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gulmkisth.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gzchrlvpb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gzdruqbxn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gkdguplij.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/ggetmoyvb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/goxkfzhch.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gibapwvrs.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gwrerqejb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gkrdbmflc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gydsvjboa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gcwddpkdh.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gzlxgpihh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gorritrev.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/glbeojupz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gyltsghds.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gplyrxvwy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/ghgbelxlp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gyhngebnc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gvhxmrcqg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gleezmtjs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gxbzlhzeg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gckdzqzgk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gsjtyjujq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gkgjpqgde.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/getuffzmo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxbgjrhme.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/goenhirae.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqywwxkqk.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gxrfhxzxl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gccplcnem.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gpwhnrcfp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gdqbpefvk.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gfcyqulnh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/ghcufvbxx.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/ghifggjpr.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gavriwxhl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gtfcmfbzh.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/grhwbwyqa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gwlfknjok.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gpyzaigxh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gvsueppqr.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gouzdzzbm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gfxjrhckd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gngxdbzfa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gwgodvgef.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/glvdtsmwh.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gdgipwvix.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gqqeflkwz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/grvecjgpi.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/glvbvirjz.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gqqrxdbgh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ggztnptjl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gilvluepc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gonzakdzl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gwlfcpltq.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gvfliirqo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gtwgzdqmo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gacnkrabv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gudttfzwc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gewhhwsqx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gsdndemub.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/goufhkwby.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gzfmlusjo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/glmxigrkk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gtlbwodyv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/guxyehsti.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gvikiifol.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gxrwxawmp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gzblffspv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/grcqnhpob.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgjjxln.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gseuppekk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/ghwwoenhm.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gpqjrxzcf.sHtML


<!-- 参考信息 -->