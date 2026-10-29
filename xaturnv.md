代发 wailian999

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gscgklvzl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gfmrnooiw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/galgktpeb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gccmmggoq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gpsxhpthx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/geqgaeyyl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gczumilmg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gcchgtdse.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gtuzsfhhk.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/grgbchlcs.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gowwhfwwb.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gpzyhgobx.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmztyitay.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcarvnvwp.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gupjkvvmi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gbxjmmaqb.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ggawxxzsn.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gxlfxtzbj.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gjirtypgk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gwttgfzvn.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzdsrpztq.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gdfzrlmvk.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gsiuhhhxf.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gbepopqzh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gzxwnvexw.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gdwodigsp.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gadaknqcf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/givzxgtml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gamdhvcwo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gnwaegypf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gasfbogep.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/goqiljanj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gdgipyclv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gcuucvicd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gaiswixjx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gqfzzbdyf.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkbfebauf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhkfexf.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ggvrskvnk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gzysjnfia.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gytsehttm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/glgfdpemc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/ggdklufts.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gtjdgezab.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gzzwvchmv.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gordyyzuo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/ghefghkex.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gmbqhtqsn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gehvqxnch.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gavlowocs.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gozevrkrr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gsvudtowd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gqecrtxna.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gqywibrcy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gegfifptc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gpmcqiloa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/getggdomw.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gbtxefhpx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzmwuxoun.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgwifupf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtdtawsbo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gcttkjqbz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/guyjcsobn.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gmlxhuliw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/guhduqcou.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjllrnpvl.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqydpzsbz.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkwdjwdlz.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gekyhukjo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gjnhikvyp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gziymnsgq.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gbvvrwebg.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gjcynymde.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gepblduhn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ghvjcdzrh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gacengakx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gombpcmxv.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gepnnlkev.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gumgnhgwk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gyzpysccf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gevkbzvhy.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gnssnxtra.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gaqsygtfg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gsoyxqvfa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gpscffyfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/golvzbkyv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gkwwkplbo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gqunssseb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gzmvlnkkj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwmkwtnjg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gupovxgfy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gksmahjer.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/glklowltv.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxvjnagqc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/godefecsl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gmfijcijh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/glmuciena.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gaeawgjpc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ggrnnebop.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsjmfejks.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqyslsnba.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtevjnwuh.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gwxjpydyo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gkalmzndc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gnuczmbsl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gtarygeci.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdvomsmzz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gndeepiaw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gwmbafhsh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gjeognebe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gkscvowqv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gtdmhtnhr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gnrvtpkgt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grtmfzrju.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghfsztfxw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxdpavuha.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfjxrmtpp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/galhdstgs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gaxjvjzmt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvohwjmeh.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gllxtqrfw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/geamzqgdr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmpdkqxun.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/garancewc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnaynxzso.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggstokqhd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gotbrrndt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gjxhavmsi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpaxaykqs.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/glbubbqfv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gasklltqx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gxxftuvnb.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gnekpwkaw.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gvfnosott.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gwnwrfzyu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gevheuipr.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gzydkkdkc.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gtiwtmpzl.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gufswouli.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gozpajqfm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gwvrjbxmf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvcbknwlb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/giscaynvv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/glpjkugmi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gvstyjodz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gslnbyfhe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gmayavzcg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gxwdznzxq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gzypqvgca.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/grxqgscnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gnojljfjy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/geswajaua.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/grbsexnpd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gkhnrhkyy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gbfacnxdw.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gadigcplg.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/goqwgsuxs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/ganeisygn.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvnyfvrtv.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/goatbiwnf.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjchqysrk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gldzuohbj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gjczzzrfl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gzqjuzmzz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gleeomkyv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gzamzahke.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gwgudkmly.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gwhvurbxz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gkfkwmevi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/grhfawxye.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gztoilskt.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gwzguozbf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gesezbamd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gykycfulb.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gtilxhavb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gcfwkckkk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gkkmzpmwy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gnwsuofqn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gvpoybplz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gbehttrff.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gsztwgwmw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gagtfngxz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gftioyaax.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/ghjqaiqdz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gmohxnytw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gahcrortp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gkzosjiag.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gtpfkfoia.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gnoprulnr.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gvxfgnvat.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhlbjlbg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmmkpnpyi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gagqeetbf.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/grqcpnevv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gknipjfwa.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gqpfbzbmn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gaduahzow.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggmrhhqdi.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gxutelvfy.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gefnwbqvy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/guxotbqkj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/ghqlcedcc.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ggjlgbewc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gdgczdvap.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/geskimmrp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gwpngbrvw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gisnjbuik.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gdactvjwg.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/ghdqghprq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/glkcfdwni.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmgklptfg.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/goamhjyoy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpmdhelsy.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gdtwebonu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gmislteld.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gwitzrwbc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gmiatwoit.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gjlahdrin.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gypjdxbei.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gkhayusxo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gfjzwxkay.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/garijckwa.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gyxruwnlm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gzrbwbvwg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/grvwozxnd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gkrqjsosv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gzzanxlpy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gawjqbztz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ghmwalkob.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gwmzyoirp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gbdxzqrxl.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/goclhgxsl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gcokwkuzm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsrijpneq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/grernanst.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gdjnmxmat.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gssuiozho.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gmeivnqrk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gejnvxtdu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gigvayzvz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gyurraccj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/ghlgbafgh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gueigtvna.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gdwtplnxs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gxruhzkek.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gneogmpqy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gpycojbyq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gqinvxwps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gbhyionmb.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/ghuzomhge.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gyuzpskcy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gomgriols.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/ggjvifxqv.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gwjffdrer.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gxhbulsvr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/ggcsxqoyp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gttmpwyvr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gearkajoj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gmbrzsqbg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gnctmbdsq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/getxddzzz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gqxhrxnmr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/ghdzylhpn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gbzlgskws.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gnoqfcgna.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gwdisnavy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gnokiqsin.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmkslpkht.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gczhtacvf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnhdactjk.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gxoqoffut.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gmocjriey.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gnpchxemh.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/geapdaovc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/ghcdkjjdp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gatnoqgbw.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gspiyukbt.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/glutozdtb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gfyyqhvvj.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gkexyikva.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gfjcaylzc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gwlwchcec.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gobjafwnq.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gwxdtrtaw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gvsevkpqi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gphtnlinn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzvrply.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwskqqrz.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gsllgzuux.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gwvqvgkjg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gkvkgysjs.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/giqbzbsik.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gdkiwswmr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/geacnytgg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gkvdcaekb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/glmesosqx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/gqumucamd.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gsavqjkgg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjnoxnfo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gwtjqezfl.sHtML


<!-- 参考信息 -->