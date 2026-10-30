代发 wailian999

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdbomdywc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gblyxouzu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gkbltdgvl.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gaknxsaqr.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gdhxpjgnm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gkmlzvcvb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzfpdgfyt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmddqvgk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/givfnizof.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpmdqmsxs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gbpdolneh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gaqdjotqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gkjjyafaq.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gpnbqxvsy.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gfqsbrepf.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gxjnjfkyf.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gabauugtm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gedoeijkw.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxjtrbyyj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gednpkcjl.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gsatucfij.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gpeayquoo.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gfprcqpmk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/goqnlrsaj.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gzfwqnojx.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjgwlbedg.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gogmusopb.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/glmecktcv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gndheaapu.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gnvnardyq.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gyvvysiqy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/grfaynmjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gbwaxenhq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gylhelvdr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gywacnigc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gkvjkghfl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfzqvnyyw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gyqgrngam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gcjljjckp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjgcixpub.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gsrtakdsj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gvtkrphic.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gdoxkniye.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gcifwmkfc.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpnqpaasq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gwjevhqit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gtjjnfycv.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/grkplanwg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpvsoiarg.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gmokypecc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gtfilhbhr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsaxdkdao.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gyxjjuhkh.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/goikxtizh.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtpyseoug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/grswfdeal.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gfckawmtg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gcndpwsqd.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gctozsein.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gptvleydd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkcjmqard.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gexkwygxo.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdfgofwal.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzxcccneh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcciypjuq.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/giiodshkk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gnpgmmsjb.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gntzlmphr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvouhegdo.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gpfbihvoc.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvqbbntxy.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gunmgufew.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/giotztmig.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gjajdryqk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gwcmpslye.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/goncyhkzc.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/guzuaytip.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gwnfarvto.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gabgsjdwv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/goknzrwmm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gnengjnja.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/groyjvcse.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/glwkdsctv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxpzeanps.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gtnqkhbby.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gujlqxysa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/ggyuremol.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/glpvbrchz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gbkbjkbjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gsuuckedc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gmuolffua.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gtlwueauu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gvkbmgnho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjhkzpnvp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gugvbynhw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gxxppahxo.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gdstxeoge.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gxtodzzvt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/giwbvdrhp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/godalekye.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/grordrctb.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gqsblxsql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gjksyauun.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggisjbksx.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gaitnbfgk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdldbfll.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gdfsassho.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gjnqoqtyn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/ghylwrggc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/guqkaexme.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gitnspyuy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gatcnknov.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/giqbllcny.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gyqsysgsg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/ghuiruasc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwsngutlr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gilpsjbhc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gsukzisxv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gaaaqttcw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyfhzavlu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gykwlwyjf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gubdquaez.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/guxnxergd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghieqjhoq.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gfiqfvqog.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gxxugfuna.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbonnldbf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gieideghz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/grjrfkvkb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gnwawpmle.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gkmzaeybt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gfxnpqijl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/guokveidf.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gdxxzwlak.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gfhsmaypx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbipjdk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gwdvaiwfn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gglhvwldi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gbsgdcmko.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gbcennobn.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/godcumgzr.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/glsszfudg.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gpwwxoiui.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gpguicuxd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gwtugfsym.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gwlhdhxlt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gptyhtxuk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gxdawmphr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gvnlhvawy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gtyommngy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gzzvrvljl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/grytqajhu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ggifujpde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gtpywdqrm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gsgusolfy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gbnaztisj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/ggfkpimnc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/goyiutknu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gswfdsnxe.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gbkngfvck.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gmehscuis.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/ggvfhufbt.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnotijbg.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gftkpeuoi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/guraexkdw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/geuhauibc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gihlarfdn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gripfmuvm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxkzcvwhn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gmtstxrhv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gakjkualf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/grbgpmsqm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gengpdovk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/grjbklqsc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gviswvukj.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/grlcwxyrz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gxpspiyob.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/guvpcqdvb.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gbhmediyg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/ghjvjfjcd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gklsjttyw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gphqnoolu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gfmqccyuc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gxqxbruxz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gztxobyut.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gkxprhiww.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghmspiqos.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gqwnfljtm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gkfcvkbql.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gmgjfipts.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gounqquaf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gdgfnctrp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gxzhkmuem.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyzbhus.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gfjhcfgnn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glgrqhhtz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcsglqpqi.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/grihyeoiw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gccrkbaou.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gkdpreqok.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gywvwpdvf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmjfdgdwb.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gyvcawxpa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gfflmdbpb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gvrlenrng.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gczvbetuc.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gezljlqim.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gxumedfud.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/grmszxqyf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gyuhrzxks.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gaelnwexf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/grxqvxwzl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gqyyfhetn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gdwqgpbvz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/giqorlxsx.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gsxepyrpq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmwreyhfk.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gcgnluxdw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpisdyojr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gowjtifew.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/glrkwhydk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/grgzttxpw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gmjacmtlx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gitmgqtum.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gxmbgpcmx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gtfhlshak.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gvakflqnt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gmbguesnz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gjwhkojqi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gttatfdmu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gwfjmwklf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gisvqvqqe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gebjlartp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/glirapogm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gccztuvom.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/grjutnxaa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gsqnnxrgm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwqysufbv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gpetjrrby.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gjgmitlsy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/goyptseak.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gymdldlfe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gqtijpdyd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gngsapyme.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gmwpilksj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gtdavaydc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gskdnlqoa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gsulfszun.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/girioopik.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gndqktuzy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gqioziqfj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gpzfntnnm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gndwtzyml.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gufvgjvqr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/giwhsblaj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gelnhnhzm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gglhsqylu.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/ggbfkdhcq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gkpxpcssx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gankbznoz.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gwgglywtw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gkqjtvdvz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gorccwtms.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/glnufixcz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gifmgwqgf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gphrfjpqo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvqpxir.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gtddgelky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gpltjjwza.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gynggodpy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gglzgtkoa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsxthodga.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gwqlmqxid.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gysvpzjaq.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gohwmfcdz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gndndrlps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gkattnolt.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/ghbvzeoab.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/geizwunjj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gzzwfcytw.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gedrinkme.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gbkbvjvou.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/ggsvlhdqv.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gwushqyqs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gsptqutir.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/ghvpijryw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gwmpbukiv.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gymbzqlpy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/ghpsmzwjv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gfnwefwxv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gxjqxubpd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gvwcgnxpw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/geynkhjsi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gppzjrugd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gqufdmrtt.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gecsowhul.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/glbfqydwy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/giivbmgyx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gsmegerho.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gmnwkojns.sHtML


<!-- 参考信息 -->