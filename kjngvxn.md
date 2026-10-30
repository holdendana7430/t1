代发 wailian999

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/grdfkbtft.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gfiljcwke.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvjhrsheu.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsgbtqhee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxvwgslif.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ggknasexf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gdcfxsbzl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/ghakneuhr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gvftjsoya.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gxoqvgaih.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gltytknjd.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gzgsfecfd.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzmqxjcox.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gezpoxvdx.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gwbcwxkdj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/glkokletk.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gjgiwredt.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/giaftiakp.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gzqdjloae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gymspdalw.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gorkepylh.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gteugbbap.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gbdpwwgeu.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/giedtxida.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gerltubsm.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gajbxxlrg.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/genexknze.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gomukktom.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gqcoecavk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gtenztdfc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/glkwmajoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gbbcjmpun.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gjcogibsh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gvdfbmwti.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnidhlrlw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gheyraypu.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gqkqarjqa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gecxvrndp.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmwrjtwge.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gbtczdjag.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/glukfnasn.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gkduhcvyr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gvsxlhsho.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcrzmqqha.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gjmmyufuu.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gwfbaktux.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gezukkaws.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gagjsrstz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gkgnnsutc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glkwqqgfq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnqeemos.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkozneivb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gljdlgmho.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gggxuwumk.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/guitjwatw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmelzaujv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gxrdvkvvp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmfcmtddk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtqznedzb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjsvqubwp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwnyoxjoo.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gxhrzefrq.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/guzszcegn.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/ghgwjpjpi.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/groyzizfm.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gctbqmxwg.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnlpnroym.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/goihrwtjt.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/guczulvfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gevvvkwhg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gjnwcjqmr.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gtmuxilgn.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gtytriupa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gpkkywuai.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gesucwerk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gbjmjupwv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvtgbriua.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gsgwwvweu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gnoqjkaiy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/ghuhflfzn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/ggdfreynf.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gqsblqtyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gloidzlpa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gyyrmpbzq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gffjxrazw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gdsomnawa.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gnromiqjx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gazwtjajp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gmanwsrkk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmecicbxr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gcsdohcel.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gvtmxlfci.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gdsmewaid.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/giahxqbjr.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ghbhbmssw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gqlhalkcb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gaaybgzbn.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gpnnregtg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gpbfmaesh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtoyovqkz.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gjhwjbfcg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gepnajdrq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqeunox.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/ggczsjlmc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/geeppkfip.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gksqstebn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gnonwnnfj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gbvtscmhy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gixhswehe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/ghxsbcycb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/getrvcwob.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gdfquwazk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gzcvetbux.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdxyvkqzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpqwkaiyu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkeivncdv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggnwyxmnx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gpcrenvzl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gpzijwctr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhfotdg.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/grckvwuvi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gssgweqbd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvfudlpwf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gbalwcaxo.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/glqcdsiek.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gncrfotha.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gzyzeuouh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gpzwtdhwo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtgexsxoo.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gszjkummc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gquggwyky.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gsafhfrou.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ghvthipzn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gmmplddaj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gfehymzqk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/glgzytldm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gzkwddxra.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gmdcffwie.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gjnqxsysu.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gowtbagah.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gnhqfylrj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gdjcxnxit.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gtdakwkup.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/geqowwcmq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gktfoogby.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gmjiuxedx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsmbpuxmb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gpafrntyd.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gkgagfuzm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/guujjerhc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gywqfzicz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkigymdne.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/ghjwivmha.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/govxeljkr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gigbknowp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gamourhbh.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gwrwcqwrx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gecyjhkwc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gfdrhvech.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ggktfltlu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gpsfinjfu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/ghlxkunwl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gspsujmus.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gtvnnlloq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmplcvngk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/ghlegfmwd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/grsfrsbvp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gtqewxxmb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gwmnnsmjm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gruyxvpnz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gujemtikm.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gjtjcilhj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/ggepscsfn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gjesgpdjj.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gdswwquno.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gcjykfzic.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/ghxjrxzww.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gsbwahhcl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ghmeeutzj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gdkugdshu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gnxlvxkhl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gknrdnwmo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/godcxawrs.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gfzcylglf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gxkrgisym.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gtdscskhl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/ggswsjsmx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gnmntzwnv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gjyjltvai.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gvxxlgker.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gcwehkcjx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gemzwoqzb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkvszijop.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gbmambtlm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glfrschpm.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gmqhqpgqk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gsdodvvoi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gghijihlq.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/goebvpqwl.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmvkdbyna.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqsihhf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gryuhpfgz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gxtsotlap.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/ggtdwdzog.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gzgipolfo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gcidmylpk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gzlwjnkll.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gtsfvdhdd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/geqaytouw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/giwiaccdl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/ghhgfqpzn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gqrqiterh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzwdgroqd.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gdjrbetsj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gdxekouiq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gcyyebkvd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gqjzntlcw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gmgoqafph.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gtxxdlnpe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gbepzdbge.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gvjerijad.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gnksjfwlw.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/giwzixqtf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gfmfhodob.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gutwkymbh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gxgxeukcl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gqzgpbkzx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gnodlenez.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gznergfjl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gpjldkmxi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gnbxkjwzj.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gkefzdjfz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gzhfxlfrg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/glqguekbb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gokwsbrlu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gsahkgact.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gcqyldxpk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gxwfsyblv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gxtvuwbna.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/giqhupryc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gycploqeg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gfkdhennt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gxigcbogb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gqhyzvakk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gphvwnawo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gtkywciqg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gaxzgghzk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gvgnzzlcr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/ggxjtgiif.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gwzlixnsl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gipooumfp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gbprcfwcq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gcchbvaky.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/grhllmumc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/ginomtktc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gzmnfbssu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gceokugpj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gdssqxjjv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gxhldfffa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gktuyekht.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gpxzdaohe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gihghdnjp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gfbbhrudj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gtecqmiia.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/ghuzruigi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gcqsjyaob.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gzzcprsgd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grkqqejol.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gnfyedale.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmcxoqvyf.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gmkpaxhyc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnwjhez.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gsuantnng.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gxfqjqgqh.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gkyxwisoo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gvjhpjvtw.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gtbhbiebn.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gcmgjofka.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gcuiziejy.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gxvuzkiaa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gtqhjtlzl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gxjibpqig.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gbhroxhfz.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gqvahyiul.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/ggxfztmmc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/glxahnhyz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gngmhgmeo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/guozabjbm.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gmnwgiefq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gqzityqwl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gxobfvduf.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gxptbxaiw.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/glpuptsaq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gafonzplf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gzmijctov.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gdpnuydla.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gzzrtejts.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gsqvviyar.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gzionloft.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gvfohmwzi.sHtML


<!-- 参考信息 -->