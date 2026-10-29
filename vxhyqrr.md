代发 wailian999

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxvycdmcq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gqmazygea.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gkniklqjc.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gabonflad.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gptbqqexv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gnmttalef.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glnsomehu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghphmrfbr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbnzdwpqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxoqnbrxb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gaxtrbpoy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gekwxflnq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gaccifaht.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gohawwbnv.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gucesbzyz.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gkcfqmchr.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glljbowhl.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggqffysio.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gbsuiznyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gkdwbicro.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gbemcdodo.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/ghquxsila.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gnpcnytou.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpakdnghz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjztxridt.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gihzcsfhy.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gxvatnrld.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqakaotkq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gmviyfmaq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbpdvadoa.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gqmdxvrfy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gvzvgvsta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gwjmhhiup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gjnxumvjg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gyoweizjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gngaskzbi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gvbfllcex.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gmnvudalu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ggkrcjegz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gdlbgvxca.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghpfvwfld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gnqfhrjkj.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gaimeffcq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gsynkgkah.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gpljecywu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gnhxihkwj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gfeelzktl.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gyhzsuyjq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gyoqoaxon.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gshyatecs.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/ggfvmcjqx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gnhupeuam.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gaqrcjbgp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gcvvhsnla.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gtrfoqsly.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/goquwwrih.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gxihglety.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqckydiur.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gehfnnwzm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ggragqoav.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/guwgqporj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glgsgqncz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gnhakoeff.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gggxbalsz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/giaabvfpz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/goxpzdpge.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gxrofghjx.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gjixesrlv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfkazgtfy.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghdlywcrn.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcpzfzfrd.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdadfoflr.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gllpufdmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gvztdmujp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gapotiyyi.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gzjdgjniw.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gtccbgkqn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gmkjwycjx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gyvwzltdf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gavnlqchj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/ggqvaolgk.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gvnpgscsc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gscmrlblo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gyrufzlpd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gvbazaiwk.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gaxbakhiv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gmcigiwqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gfpkqeewf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gipevzmvl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/guyjepzjr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gygepfxjf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmuijlzi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gjyrjayay.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzxtpgynv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqukvhz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gscbatcgl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gnswrtsdm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gyqhwawfh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/givlqwczk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/giaudtrox.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gimiugxsc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gfibkhnlz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gklicdmkm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwbhgjfog.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gyvdzfayu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gddkokjxg.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/ghxnvzopk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gupfghpcm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gphwzhkmj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gkpgunurc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/giqrdhupm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gpslpvroe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/girpemasl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gqtrswxuy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/glhsssgfq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/genpvwgti.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/ghnfsezef.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gomkfzwsq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gfhhmqgoj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gsbewctsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjkanegsb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gyroaqska.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gjpsuxkac.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gaqszvnoe.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gceokcgye.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gifmxoyfb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvntxdkmn.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/goecvbqqm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqqrmrvtv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gjsamakli.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/guheklsqo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gvodulroe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcwhnmkcl.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gbobfhghh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gmkgjxlgc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ghgwzilnu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ghbpsljdc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpyofjmxe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gxrjntaux.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/ghetwkraz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gvqipheja.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gdkjvdpbo.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gzyosonje.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gssinwjyt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gmhdwpejq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gsdiimykz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gvmmnmgwl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gasfrtrlc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gttdfjkfy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gnhyxinuq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwetnnckg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gcbfeoygs.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gbfjthlya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/geexltjhb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gtghzxesw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gcbsortyu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gtalbtzru.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gpgrozvrx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gnihpfuhj.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gnzljwosb.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gpnfxbray.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gesqgrxkg.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdonwfzzd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxwstdqan.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gwgpbpctp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gadkdmcvx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gsoaivovq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gunwdyvss.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gswzquunb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gqyfigont.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/grvgjbdro.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/ggvmiigwk.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gvabeyfvi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gydkermqe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gaougbggk.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/glrxifbwn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gtzlgehjy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gloxyjaut.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/ghldnejfg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gprxvkzzl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gaknwbtuo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gzdahlcnb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gdtbmnwnm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gxzlcleok.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gjoglofwq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gichuhmpf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gxeikmdah.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/glcmsfssf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gfiuvlceo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gvqyclzmm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gxxgrgina.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/geutyaxbs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/goxhzwzyw.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gihouuodp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gfpjltckx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyvuocweu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjrhwebgd.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gbpoverme.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gswjixfbe.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/glbrzckgt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gisneyopv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/grfwqvpop.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gfiryqirw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gjdetsctr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gveqfcjxn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gxpxzbjlj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzjtaun.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gmfeolmiz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gnclovaof.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gaswqwlje.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gweaafhhl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/goqxcghlb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gmxwgvolh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gtpbpmmfi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gkaebdhii.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gbhiuoyld.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gruwqsqdu.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gtdtngixj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gtcltbade.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gczmzyrvc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gapibfmpb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/giuuwgwbw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/grpoixejd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gytcamtve.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gkzjthnni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gaksmwpux.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gqsaufyqi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gdaekumsj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdkakdodt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gwdvziuxh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gptwesifq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpdkbdeps.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gvxnnwcwq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gaazzkquh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gojgqisel.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gavylplnc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/grtakdtlb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/giblaknew.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/geahnvnhk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/ghnrkwpkk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gnqxgigqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gomufrlnb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gqpcstfzq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gcqygyqis.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gwhmeswrh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkcqjzy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gsrslcdbq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gyjuhdokr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gxryjqezi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gqvrenozs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/guezzkqvi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gyrvsbmhf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gzmjpzhvv.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gjuvaersq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gbrvpuiem.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/ghssubwhs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gqzbzqzkj.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gpuokqzsk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gvgrfbtri.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gctqtrdhx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gqduklrzb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/ghpvgpokc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gnahdpyla.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/grhwwpcyk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/glcylkabs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gvnxeuuon.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gjepvrqqp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gobxhphmf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gtixsohys.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gocgprlju.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gllduxczx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glocvgmcd.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/guxffecsn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkmwptudv.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gzwuygzpc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxbpenf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gpfjwdrts.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gzbxweccw.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gqsrpqxzp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/glbkaegbb.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/glllpzlji.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gdwrboaxe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gpzomrqrh.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gjxauxzyu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gwxodlolb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gprejkxkx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/glgkyhckb.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gleqvuzlo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gpqcrrbpl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gfxfexmll.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/ghddqzryq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gekimqdfd.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gdxhoqhit.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gtkmhtjgh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gwyfrtvqg.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gpqjazcjg.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gquywrbyr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gkgobinib.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/glpohhxeo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gkljpbiuc.sHtML


<!-- 参考信息 -->