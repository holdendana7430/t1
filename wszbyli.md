代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqmwblosk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gnmxzdeks.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gsbubfeum.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gsiabnhre.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/geghjskwq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gqocxcfrn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gysxjgnyj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goxjjygqc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpouzdeos.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gotepqivn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gylyqbkxw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gjmjrbifg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gtgitvfyk.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gxchwwaqx.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gokmyojsw.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/glsxengog.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gobjmsofo.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gerwdocin.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfhhuwndh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gkvsgdmsc.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gsshtckts.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gronntyvr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gaufxrtxh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gdqiytckb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcqeggicx.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gsmarybdq.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gvtohbkue.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gtsltjzvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gdefxvuqe.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gfdfpvgxx.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gkbopntjq.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gzwcrrklx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gpuxtzshf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gnujrkyvn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/goupvebqy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gwpycqxrv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gslmyjbzz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsngqakng.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gctampmkt.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gwnugosde.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gdkgimeph.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/guxpqudbi.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gncctzvlo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/guqyfqlww.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbwagbqte.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gzypcblui.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gihhcbnid.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/geentaoii.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gmyzlhlev.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqtmgqvpk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gbppwotel.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmeggixsv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gyawqemli.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gczfezewy.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcxjjrpda.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpliczhmt.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gknltqxlh.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/glyawnixb.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gmcbomema.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gdxqpfyem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/grpnixtbe.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfendjzuv.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gofrzjopt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvkmfdsow.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gvkqcudfm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gyvyogqoo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/guiqbrehv.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gvekkcxkm.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gmjsjleok.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guanqewot.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gcibogibl.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjdeqtxxg.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gadrgdzwd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gvoycxuqc.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gtwsoixbj.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gujtscuhv.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gtcaymgbw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gyvjyntse.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyejbqcqg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gplsleebd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gnhksqzfv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gjfbffzzk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gsfnoimmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gcukztuig.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnwlyffh.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gomxtmarv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gchqtwxwz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gtosfowmr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gqwbknowj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gybcfbuqe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gyombkmgj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gnbitxhks.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gfcmodkzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqwunszvt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gogcpckhs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gondfzzqy.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gfszkrusb.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdlpkwxft.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmqreahyl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/glziazbvw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gvffmxddh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gaxkaevrr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gjvxvafrw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtzeixxcz.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/ghjwpvtdl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbzmnhzap.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gpqfuudlx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gcwihfpkf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gglxtqgnz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gjfavrdum.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsnqcjqkb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdozpkvd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gubdjfwtn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/govtygjkd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gbhjxefdi.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gubfderzj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gvucacfmf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbobiqwew.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gyajfqfxi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gvmmhjrhf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/garprjuwu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gzevbaizt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/ggrtmvemt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnvqmbuiu.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/ggzcglcsr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gbcvnznpc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gdcctnoju.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghlvkfymv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gsusupxcn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gehshslnd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gxulyallz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/geqsvpcfk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gbxykctzt.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gikngvowk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gbktpzqno.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gfychogbz.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gqwxbreua.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gpxwueurz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdpxlnd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gsohtobiq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gvpvjqtmd.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gdylijomw.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gylgqeppn.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gfqaasslt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/glcymzoca.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gcukotfyo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gyiwkfkml.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gdznhatnb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gjryteeec.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gsqgedsbg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gtwcfxjkb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gqiuqpfes.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/guhwvrvhc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjsftlnls.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gnkqyzpnp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmqlbbsno.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gtdmkteuw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gjiyoqmaf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gzgjfiorq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmvaammsy.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gnervgzom.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/ghmnrckvo.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/guncjwdqn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glcriiotv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqeksrkhc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gynglurcr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gnvsniftp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gyzufcqrj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gtatxjmcu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/grimcxfpu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gtxfkmgvl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gmekzpmtz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gjgrrfidx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/ggyqhcxaf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/ggixwczzy.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gxibdljru.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gmcaffywy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gbbrfxwqb.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gdxqswedj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gcecfhyjx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gastkypqq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gwztkgotf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gcbqjxqrl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gmpekcbmk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gxbyzmbja.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gyzursvsu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/ghkgnrqsl.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gucszecrt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gqqktllvk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gwguexklg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/giznewdiq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/glzkpqimm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gncyizuac.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gcynmgnlx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gaauyyuor.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwmffcffa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guflzzdhe.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gsoustxyk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwcajcppt.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gfxvxlctu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/guvsmetnh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gaykymjni.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gsllqcpdy.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gtiksolsa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gqtdycjnz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtfgdgzft.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gedvkbcnt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gvtgqpshe.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gqhuqhpdt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gjwhogjay.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gmknpecgo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/garypbann.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gxykwxnxx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gmrmcxtcs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gbborydqf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gohihyhid.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gvoztpsaz.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/geadgwfgq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gackiwrdm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gzdswmdln.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/geybnhqey.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjshcmpoj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gxkydkvwj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gvjdwydxn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gpxqxupnx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gozboljpe.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gavnfamgf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gwzpohhul.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gdqgiitwa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/glbvloonm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvqotgstm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/ginmchafq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gnfgqyzti.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/geludykuo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxuexvd.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/glnjbaocr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gevgfopga.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqayqgiqz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gxxgoblsu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gcyggxwvi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gnfabofry.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/ggkjjwdpm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gesxkojvl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtastwau.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gzoqtycge.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/geozokkbs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gjuitgvet.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gwsghabbm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/grqwrxmwk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gavtekrjw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gdloghvoq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gwnzwpuss.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gocaiilqz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gjfbdstlv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/ghgwfsyih.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gwpkhitki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gntuxiikp.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gpkuafsmb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gbuuynvdl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gpwmmstxm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gcbyvfrqp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gqznqhqhc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gjhcebddu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gccxrsnxk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gsogfvkqa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/ggkomuawb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gqwmuqzvy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gnhjqwofw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/guykeathd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gmylykgjk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gwozfawmq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfynrktgo.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gazakptwy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gplroyhhe.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gntazkvcf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gnlhgoaam.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gupuagvrw.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gxxbjdkzo.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gwlqawjjx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gxpelmxsa.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/giskdwjrp.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gvvffvino.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gtchpkzjy.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gzcoojgtm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gquidfvrw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gkmybpsuw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gkfslpkxq.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gssjocxup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gkpypajhn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/glsfpxvkj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/ggtvbccoq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvervpsh.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gtvvgtbmr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gqeomxkwq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/golazuqwr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gsqriglvq.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gjiltzztj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/guyoaxpbw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gndxylxfi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/grtdjytxu.sHtML


<!-- 参考信息 -->