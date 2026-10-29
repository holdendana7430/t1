代发 wailian999

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/ggnpcntou.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gsfvtchei.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gauftnmvp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxcsevqjz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/goiwzjfic.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggdxjaqjs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/goibrgopo.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gwravjaud.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/ggjisvqbz.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/ggfzlqlzc.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gedxnvxck.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gbtqocbxb.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gyfksqoej.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gveuvqzyo.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkriiwyks.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/guxroskbx.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/guinatyoo.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtwxogkah.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/ghnubgdty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gnqfojlcg.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gvjdztzfk.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/glaoghnbm.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gvplqcape.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gergfanua.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gpjsetszv.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/glymojwwv.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/guakeqkwb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gcrwjuixf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/glqvnhobj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gjcreinzr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/giigasulb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvcadwbth.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/ghvsurcjs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gfbpeskls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gnliyphzo.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gajppctsg.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/golghbozt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gxsbnblry.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpwvpijgw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gliloruto.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gzrmuwpaa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ggexacoji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gzduxarjx.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjmxzzear.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/galsqeznb.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/grrbjaumu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/grcigmwsi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmwbvppwk.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ggdyjwcna.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gdgnktlpo.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagxmvmcg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfuasvrxc.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gchmyzxqs.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gmgwjwpnb.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gzoadzpmz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gvrlhhgal.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gbokqcmqt.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjsqiqyjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gzcnhmjwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/grmwjtyqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gfqluhalr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gotcmajzw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gvgxhmitj.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/ghvftfrff.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gttkezpxk.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpkpknbhp.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gocaysfex.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxidtetjx.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkqvwzbaj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gndkddwmr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/ggeqrbjaw.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gwgpxqtyb.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gxkgmixvg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gskwrvacc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gbgxrqjjm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gclolhtcy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gzuxzgler.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gmkfqlfzf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpbhfqiiw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gysjhbndg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gntcaygam.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/guhfguvmj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gniaozyzw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gulqpnsiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gczjxowbx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gtnzpwnac.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gwcdvccnd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gvussjexu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gxyvstbls.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gfywraiha.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gletifzeb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gyhwahcqh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gepnjuzfh.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gavokxhjb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gznnheutc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gfchvnpit.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gzqotoxrf.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gkupgrqki.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/grpfgkycq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gifbhmdkh.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/glwwcikmq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqglikhzg.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gqsmoasyu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gywdeyhhz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gyjrppiqn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gbisgxgej.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/ggtglkcle.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gbbkjqvty.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gsoqqvhpb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/grzltwpbp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gopxtfhnu.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gbnwypicj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gkdfutejf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwnatsmk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gojthghut.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gyzxnbcro.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxoslmznr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gshgrcsaa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gamhwxejz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnpugueam.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gycosspxq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gpjxelzlq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gaaeigyrp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdrvgrfwh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gighhrtsx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbrrpsrux.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gfxwokhxc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gylflluux.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqsecimre.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gcvxhjska.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gtigiskko.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gnxkeiufk.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gjnwqhozk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gnwaliihx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gaeqmhrzr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gdwalkkjv.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gqhygsjtg.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/ggwgojhnq.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gzxpcnbjh.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gdmwfnbpu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gtsjrbmxd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxktjclgt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gwatiobtv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gteegfhma.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gqejqhjff.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gsetlzwxj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gizktsivi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gtmcgumwq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/grwshbtaq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/grznybmdj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/guxvztxwx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gujpbeezk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gqaaorlpi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gapcytomv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/govpsaoaf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gxfqengha.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gtguodkyz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gstflzebe.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkupsomzb.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpasylcoz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ggwyhpopu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gkxohrpfl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gdzchwhsv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gftffyjcy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gtsyhmrwk.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gwgudytrl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gdtigqmpm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/giorlbqva.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gygqqznoi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gssxdcwzz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/giqzrytbu.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gjifxsory.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gjkyvvczo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gzycqygcy.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/grjfzlsyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gakqaryzq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/glqkttfvx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gsieucuvj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/griqtxnht.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gjlcfcazc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gdrbnjqhu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gavjrxmtc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/ghqpcispl.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gdtrhrcio.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gwnwajrce.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gcwctcmbs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gyrkhapqs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gnpardepz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/girlcyyro.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/ggdmmttai.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gvhuqnynj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gclshwlyi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gseweugsq.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqqhqppth.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpbahaukb.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gqqhvqhbd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gldsxnfuz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gprqiwlxg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giuoxxpbv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gdrclfvbs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/glthxcsrt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/giztmzvmi.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gwdyitxhj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gxnicxdzh.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gkiazmowq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gmdlcwmmn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gcxvcnfoo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gdridedhf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gbwsqtaci.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gjkvfwlaz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzfypxnff.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/grlisashg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gdmshdnux.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gindimplw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gozqyqsuh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/glacdiodv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gzgtaxcsw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gjizuhalm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gqgnmpwrm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gwibhgwho.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gmkppccsk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/ggivmuean.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gtefsdpnl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gtlvmmvgb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gsnprilae.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gebylrmvc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gfhoykavo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gtvsgwyfh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gltcdrtyr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxknjhmiv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gpylktgmk.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/grskvrgde.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gmrpkqdba.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/goinkhryr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ggbgofwhy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/giaomjmqs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gylmsijnn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gwuyjgdcw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gqotnolsf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gzgxqkzlv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gqcxjvxjz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gfyjxkvwp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/ghjgzjgjh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gizodjomc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gznyvtyep.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gkvpbdhca.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/goycxtaes.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/ggkrbaqqq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gqwwgolmv.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gnzzinlkf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/grzfkcczj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gwsbdxrkb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gyhmqvvmb.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/glyyqtbor.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gvnmccfob.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gjcfmeywy.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gacssuuro.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gfmzarmho.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gdkxizhpw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gdiutlkah.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gnckgwibj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gafiopanf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gsipryout.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gabrtgeck.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gsanaxsfj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gztytekys.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gyzmjqlxh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/garxyrnww.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gxrchzpel.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxfuorbao.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gknfukfnu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gddyvpqjd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/geypapqts.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gdamwywfg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gycmbhdqb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gepoddhgz.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gnzjqfyjh.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gzrfaiuxo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gstxvscfj.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gpbteqpmy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gtcypchhu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gwcefzkfh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/grmzwlqsf.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gjmmsqaoj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gwqqioosi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gzgmzetnt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/glyfjvkvx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gogsbhuum.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gkhijggyx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gyzvvtanl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gyyldzaea.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gyctcdvec.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gqwfoqltx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/ggcxlssnw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gscpwwsjf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gcixynpqq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gamqewsjj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gtpfnfoep.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gmxkgkilr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/glxetfjrs.sHtML


<!-- 参考信息 -->