代发 wailian999

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gqonstjbb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gcqwrohus.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzgbrfkip.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghiydgwla.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gulknstio.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gasfbqotm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gxnwfbvuz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/ggkziwzsf.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gemhrfhpa.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gepdeizyn.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gqnstdwvg.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gbcimgbkd.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grlbdeths.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghfuvymki.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gdkmkogog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gbsgsmvud.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/giuyxqggu.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gmjuhpelm.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/ggotgcxrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gqctbqzkl.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/ghfrrkhcp.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjrblozxg.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gkvvztrni.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/grfgqdjka.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/ghzefdant.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gqecpwkqy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdmxdkgbh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gztqyaazh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gfruuatoa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gpcgugivr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gvvibtptb.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gfaxigbmf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/guewisrhy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwsxtewio.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gdwajitpw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/getnggihl.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/guactjulu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gpqtxojjk.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/geeztfycb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gkajwrjpp.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gmdxjqjlw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gtghqpxbh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gremekmzu.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghjomwtfg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gcmucimyh.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/guzpgjejn.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gqsbtkhij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gpcjyqfja.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnklxfzc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gcsrkevxh.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/giwfmzuen.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gwnasaxab.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gdwzvihun.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/guwgwdaaa.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gxbtlqhbj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghgibqfay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gumkphpvc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grgottvbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grpvsrqze.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gkmgbjsig.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/getdadvpi.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gdhhgpjig.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/goutuwmcl.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gnjfajwof.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/guwauoanh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gjqubwqnj.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gjjjmizhl.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmpqcpcjv.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gqitwmklh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/genxxyktw.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gsyvywltz.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ghlvqwvjs.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/glpitvimq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/glrzbjsvm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gqmudclsq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gfwiuqyjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gluwpzmvu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/geukdwesr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gucckmjid.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gtwesunyg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/giakauxdl.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gocblbadc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/guhefitji.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gpeaosugj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/goepaujza.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gjralvzvc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gayasnflz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gwytxxwwr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gzqsdupyj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gyvhznzbb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gskgwirvj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gbrozvhna.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gifiyrscy.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gscqlmjim.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gbhkyrdud.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/golgzssyf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gfbfmvarl.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gemjnyphv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gblptpjpa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvtorhdbb.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gfimdpfmi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gktqrajpm.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gelexqvfa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gjkgqjzfp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gekchunjm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/grktrrumw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gseibriow.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gkwjjiqus.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gntxpwhbd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gckoeqbej.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/giaoptnbt.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gufkzaemy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gecwvrxqp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gytkgkwml.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmvdscwxx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggjshqhcs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghntcygyi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gcaslgtqg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvvczbjlg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnmsfbgmw.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gqcbdzisp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gvahylrrg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbmmepzta.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwsjrofkq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gohezyajl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/goftngopp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gaefizkme.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/grsodfuom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gtodkmmmf.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/ghgobnaob.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/ggklpbson.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gszbimjzu.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/ggxafxfzi.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/goadqikew.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gylaqwyqn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/ghcnzqtco.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/glrtvdirs.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/grftriidy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gdfqoysrx.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gofxmkgod.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gecetcvid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ggrnqbojq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/ggoqaqoxp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gotmchpjl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gfybcpxyl.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gyygtweeg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdosudthp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gghzpycvh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gzjbvhhcy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gigniozks.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gdgadognx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gzzmjguxp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gmdmtkopt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gjewmdvwa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gjyghpdff.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gpxxyakox.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/glwzervdt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gfzjeihqr.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gqalythby.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzmdqdnwu.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjhzcrpmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gmkyssmhh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/govoiwzbb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/grvtvvinx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/glnaiiflj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gfsvguilo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gltsbxnyy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gbjzrxukq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gtpmfygyh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gdgjyoppr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/glqeetoya.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gtatijviy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/glsvachdf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gclilkdxm.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/ghkzpjhwb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gsmpzzdiw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gleqbclfq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gansdkacf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gmnbqhdvm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gcukfgiaq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gwhsyxmbv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gxykrextv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gpfdsvugj.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gqntjavcq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gcnyzpncs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gmlbjxnvn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gqvmsqsbo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gflfrfaei.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gaetzpail.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gbwuenyal.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gicchgqjk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdckbyeox.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grcwxyqku.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gdzdmyvwn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyhfytndj.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gbolwdotm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gytnwfbsw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gmmqghlzj.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gmbtosbnu.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giyoxptex.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gbghzudzt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gvwlzsmjf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gcnbpesji.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gbpgwdgxz.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gseeklftn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gprnnzgfl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gdyuazpmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gtldiaavb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/giddpletg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gggwtfkko.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gtezkajdb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gapbwlkxj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtnoanwth.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gnqlipzoq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkcxwphnv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/guhpcyzdp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gmcwbcfxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gfxwnjljd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gxvpsqhnl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/ghdhuxilo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gqcgviiwx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gohbtlfkb.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gzvxtbmjr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqcvpepxa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/geerpjlgb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gdmycptrq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gkhseajhz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gbouobwai.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/glubuyidz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gcluwaeth.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gaffevoed.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gajkveiaw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gioyilvbb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gfjlvllmo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gldnoszpe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/glxshgxgo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/ggoyiaaoq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gpdhweebr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ghahfvnxz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/ggzxzgitn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gclodmbbg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gjjwupbbg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gjebjcdhj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ggxrxvkcz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gapqmgqwb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gwovwthdq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/ghumreloy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gdzsyvgyi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/geljqybef.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gjqknvcev.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/goyugxpbu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gmpgfxtkl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/ggretkquw.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/grzycejpj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/glysipfgy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gvklotydc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/ggxyxdrwt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gcxyfvfgl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gjmhhwafj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/griemohht.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/glvlvqoif.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gznodugti.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gcecpeykk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gljikmmjf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gjjfsvvsx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gwgwdyiqf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gesepwwjc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbyhopmhz.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/ggooxjqsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfgsergvx.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gvoraufyt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gvvzmgnzm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gdtoopswv.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gagrdgmkc.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gtsoktfho.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/ggmvnpqhk.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gaesmsrfr.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gwjhcdulk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gniiqhgwa.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gnihehzxi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/geqwomkmf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gjtuszkig.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/goivcsnsb.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gcedcuouo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gzaxgqvhd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gdlccuirg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gbffohwml.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gaiulntzy.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gaszkyfjp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/goyplfdvy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gsmgucouq.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gteehjqke.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gofygimbo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gjqcoldrg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gwjtznpyi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gdlcpncjc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gnlvwzmxj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/ghxealfpp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gvwwbgycp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gdbnvzshi.sHtML


<!-- 参考信息 -->