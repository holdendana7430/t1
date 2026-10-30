代发 wailian999

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gqnctboqf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gmqntpdjv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzngzbneh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gucoogcez.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gongdblmx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glybtrzty.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gpomrenbp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gscwgtmoz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/glplatspz.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/ggrtqdudu.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gpnhspxzg.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gmbxfrcmy.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glrjixctr.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/glyptzuvk.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gdeycslng.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gxpsfimom.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gykmsjkry.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gaiaxdrny.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/ghjfwxvef.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gsycchofa.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/geefoybvi.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gnoijpzfy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gmkypupdj.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gezsfxrui.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/grbscvevk.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ghwzotrmr.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gwcrzccai.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/ghtjctfnc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gnrlkazaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gkcupsqmx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gturcopdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gefwfhmmt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gjkcxbzyn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gbmmpxaja.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gjuerxthy.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gbgystgej.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gbxodvguq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/giglrzqhf.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggzjdkwng.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gyjllmpwd.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqcipbyyt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gdiiojltf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/geyogmbpe.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gufylyfbs.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/glorvqowv.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/goksletjl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gsslujrpd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gicojponc.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gkacljmes.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gblrxooxm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gltaqdtgb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gggfcusec.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gmbkbxqyz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gtebfzxwl.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gxccqzlfg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gcpaplscu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/giwucnffk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxkpbyson.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvntfdzkf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/ghebwanaj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdpmyzzdd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gpkfzofij.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gmxzxipth.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/guapokzmm.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/ggdcfcqfc.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gnwdqjnrj.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/giahezmlo.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gilpyqtpf.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glvjuzsae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gdirgjxzp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gelwszota.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gqrqsaqeg.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gkfiwudre.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gwlntytao.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmdetfmxa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gpfbayara.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gnngplhnd.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gyqifmsge.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gffineuki.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gwiqooiof.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gaxuonmcv.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gmrxullik.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gblqdeiak.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gtphssihv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/goufjijwu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gyktejxts.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/geyhhhioz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/ghnfucugq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gshoxqnnn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gehswamlb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gxmyjizfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gusdekafw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gjebgqfhm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghyzrqkkt.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gguhdhuap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpslfhdo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gxsfcniav.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gmhftrjba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gvvgtrenh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gncaqdzic.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwpwydtuv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzjiobnt.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gbtzktohb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/ggpyxbspo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gnugmoghf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmhdtqwrh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gymviceom.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/ghaqdaism.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/giddjrktg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gjymjpaeo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/grpcwiwio.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gyakgjzzq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/guxpdhqdf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkyakwqsr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ghlxnphgc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/geqrfmcpu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfbblwcsu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gxsjmhslc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/ghlwofwap.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpizhxore.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gbkbcemuc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gzuvcykjp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfmgyeicm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxivnyuim.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gllzvsgej.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gwwcicbfi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/grjacubmp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gqahdhyrg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggnkxieih.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gysghcwqf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gwqcmgyll.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/ggcuiceav.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gspwelvpm.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gurkabsnl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gyddemlhd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gdbgefkcr.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gihxkbpju.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gildicsim.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/ghjzherst.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gjaidsblm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gnmnkcjdy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfjgpzjpd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gtjqefudc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gjrvisycj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gaodqrmzy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gvnbzvbeq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gdxrkywvi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gvefjstsc.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gjzqwrzav.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gwdrvsqoh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/grldzroxe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwtmrjtqz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gjdksjgbn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gjwltokmg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gqxmjusjm.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gffrsmmzn.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/ggeqcgqiz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gxripgeva.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gdroybwfb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxxctacom.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gtbjyuxhy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gefpurpcs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gjdkydmfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gatjzftzx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gexfmwfeb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/ghucpwpxm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/ghvmsblfq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/ghbmnjfci.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gjihsjzsa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/guwldulfg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gvjjaifrw.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/ggyowjfrq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gehgfwsog.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gonjrzsrq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gughnkqid.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gvntyqkqs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gqpmqjteb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gwsvqusef.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/ggfdtdgrx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gzfsrhdkt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gjogmmizn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gqpjghvnh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gptxbsfjj.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gbpczazys.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gepqkbjjh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gjrhoqnpv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gknlwihiv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/ggymobjok.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gaoislolo.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gffzhqpba.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gjxzsdvbl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpjahrvar.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gonaexxyg.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gobmslrnl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guzezfjwm.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gwmpohwyl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/glnqashhv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxertvhgd.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gygbssaqb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/glfnyeaqv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gjtcgbiof.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzllvmxd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gumbemqit.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gkjujplrb.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxynoerxt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/ghxaujicy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gulnhbyvu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gufoyfvfw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gbcrzskbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gnxpaaztj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gsvszjbvp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzfnntxpm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtsrpjlmb.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gjoxruxvr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gwytuhohz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gpimdgcxk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gersghgua.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gpztsjmai.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gxjklxeop.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gxcywmvxi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gicxjvrvl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gjplfkjge.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gczwrasyb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gmtqjbabv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gixmpgymz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gpimwqrqb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gqnuratij.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gmxiydpaw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gdcbjixko.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/grbdwgdma.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gbpcujmys.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gtjkydixa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzhykgocj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gstunswcx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gkriibsvq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gxeqjnxpq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gsekrkqmq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/glmxgerqc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/goqojlyoy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gitdwkazj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gjzuexszp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ghpxszjrj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gsmhzdiwi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gnkmnfuxj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/ggolbegly.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gqtogizci.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gktvbdxtz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gjxfxvafd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gyjkiiqaw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/geuoiqwat.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gjsshpoeu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gvgnzuhyn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gamksoksz.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gwecswbmb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gusqcjgll.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gynkvnnzl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gjybjaopo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gixnwqvfk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gohvlbrqw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gjwrumkau.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gklytfxqa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gmrvarxct.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gprhwlxbm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gavwggngt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/glhsdmqiv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvbctbn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gvccxhdcu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gztfpdgom.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gpnqivcfy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grekypuox.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gqdlyaneb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gqavafcgw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gtmtrmrzj.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gxyxztfai.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gaudxovsg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/grjpnfdrk.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gahabgedb.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gdqkuxfyp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gdhglsvdm.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/govvcdcjk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gceucqwzg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/glpwehbbt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/giwwejyam.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gtehlcipl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gnifvtvzt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gbjatpzyu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/glyllylwh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gmszlpmgu.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/gbhaxkbdh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gchvmvyka.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/goqnglpyw.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ghaksajwv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/goijiylkw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gqvwqxeur.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gvuygxtxq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gakrrhsin.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gzoivrfcw.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gmfyjvztv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gxaincdvf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/grgpiechm.sHtML


<!-- 参考信息 -->