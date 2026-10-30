代发 wailian999

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gobfnwgdb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/goperlioh.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxjbozfvm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnigcugxd.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdmczqwwo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gekedbeup.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/glziqatzy.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gbdtwpxow.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gdzyjiymf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/golhqcmvo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbqnclnpn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gczbsyofq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gijyhilur.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfqzpibkg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gjbkeermz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/glzghteuy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gghijfvae.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gysymvpwp.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcsdlcjqw.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gyeddular.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbviomiut.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gogdwhsqz.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbvugkatz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gcedqqiro.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gegjuwuce.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gcbcigsxi.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gprlzxmdc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gzeqtupfx.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/ghqytyixf.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gmjacpmcw.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gjpfjaquy.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gprsqprpd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gziqblcbg.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gaylaiwyi.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gmefwxpjo.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gdaotlgex.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gibdvtign.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gegvsuear.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gqsnllgsz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gdzsnqdqq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gkdiswvvp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gnxxwvmvt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gweawqgzm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gqyxbzfxu.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gabyfxxko.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ggimbvczw.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzrslmkbv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gibrpaukz.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gexfrjtrd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/ganmdsvrf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gnqwjvjfg.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gnylsyhdb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gafmuljlv.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/grkomgowd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gbtgxjzey.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkvuvovsm.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsnujgstj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwkdyoalc.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkifqimbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gqgpchlws.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gltjysgca.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gxnjkxwjr.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/goaewcsgx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gjkidbbxy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvyvrybcm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/geggduswa.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghiiglrbr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gibzrkyny.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gtoracyzk.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gpdsjhflp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gujgjoohh.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gkezvefwe.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gnwrfjuja.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gqnvhgzke.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gxfpbasea.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvnurfxse.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gulvwfkcz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gtyfcswzi.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gvxstgjtu.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gxlaiuhdn.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gujrxvele.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gwqizcafl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gnkrkkxib.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gmcuypgqd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/ghwleqiij.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gynxxmgoc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gcadzhxle.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gllhsyvgz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gkuuxverp.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gccvyimjk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gbmiluyqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ggkrxngfo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/guhbvvyde.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/guaymjcnd.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gezczbipk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gxpsrchur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gfhmiyvoq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gmjhoqazf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gvvxwnrvi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gdpnvbkft.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gnmnmwjrd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gilhyfkbu.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/glllquaoo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gahkgcgqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gyxdrwhwy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gdtkbixit.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/ghdxjsqdw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gewdouggm.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gelqoebsa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggvmaivci.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gcxgjvdkt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gzagaolbn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gdfdunuww.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gavgxbsww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjrajvxto.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gzpicvscr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gvrrblunh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggpjgzper.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gdhknzlfn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gmdgbgmil.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gfhbamecw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdwdlrmwm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gklryxofv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmjtgoabq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqxncscod.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ggdtgfprb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gcbsjvlbe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsfpzcntf.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gdodpbfel.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gpuwpogen.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzvthskbd.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gwbytexqr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxmojncoa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gonwgisdi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/ghnosipcp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gahjxqjyr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/grwijblun.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gwfggiyho.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gkvzvungc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gtqxqzfor.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gyhznmxiw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gdfuefrgo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gfcebpuev.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ggmpukicx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gpefadask.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gsoyuzcoc.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gjwerhcxa.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gqklywdsp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gvoocijpo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gdwefbeuw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/grdtshfth.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkozozvuv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gedbiesjj.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gztfzmugm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gvndetxrj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/ghybnlxan.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gqcpxwrpb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/glpngpaic.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtuxatygm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gcnypxazc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gajtatgzs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gytnafxfp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gxjbmelmr.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gjsfhkcqo.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gumnkyeck.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gheaauibo.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gqldxqysm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfycqoakm.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gsjkebbtl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gujjdnauo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gjzvaxpva.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gbnmqpsxr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghxypevll.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gcjausoav.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gwaoxivav.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gurjzfbxe.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gqbxvdbvy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gvvjrjeis.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gnhumlanl.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gqzsibaxi.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gbdfrhtle.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/glmgsqnpt.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gempitzbd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gndnlwfkx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gayfdphom.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/grtfzsccw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gfjvghboy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gezbtlocv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gguqselym.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gxsukwphb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gmkixccfq.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gwjydbhhj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gmslwilqa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gmkznoprv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/ggkejjzjh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gpmujlphm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gmkwkyjug.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gnfbyndlg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gyksksdip.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/glfpdrcgq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glefbefdy.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gpeeoftcp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghiihoker.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/ggeotlslq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/godqsfcir.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gjkrnfnvi.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gbblcoalq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gxjpiczch.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gohwoesjj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gqkvviimg.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gitzydfst.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gyxfqhtrn.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gsrkokzfj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkqpanmv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/grefwawyy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gmsltcqrk.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gspulqupn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gdemtpmvy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gcdjvzbqe.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gsqcnbdlq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmehunkih.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gexkkwhrp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtxloizel.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/goxgfxwvo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gurficmvj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gbmtiqykr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gdpkeaoir.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gytrokeap.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/guoskinww.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/ghdmipokv.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gvebnegoc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gbpjlfcls.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grdukpvpf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gajdwzkiu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gybonamsi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/garxjzhzs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gzdyfifub.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gcntgiggt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gqrzqpisf.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gzgzeekmi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gnadvnimq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gnpftwfol.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/grwwnbhts.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/givwacesl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gimjfkuca.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gedanshvt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gibikkxrr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gcpkblpgv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gxygbnezh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gdgutuzew.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gjizckeoz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ggrmweyrn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/giyxunuqs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gslttkidf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gatlbbfua.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gwvugyfzp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/galvnvnaj.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gqbdbzohn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gxycgvmbw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gshnuupyp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gzgzfzizw.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gioejqelv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/giougdudl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gdbauhsvv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gkclyiecz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gumcaxsur.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guzblybmo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gypbeyehd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gwjwszraf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gzscvykbu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gbjtnswqc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gnzcalwgw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gaeoauhuv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gobwdaavn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/geswoeojy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghadxylzx.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/glkioeeis.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjzfluluk.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gfwhwmafu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gtkpuhnyf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gxijrkeki.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/geqsuacgm.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gtuqosocs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gjfrfhgzw.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gxigvgbrs.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gqevotylq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/ggjtnnliu.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gfkzsrtqq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gwzsnzozt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gkhnkmpyn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gewcymlba.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gwuvnuris.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/grsvmhzbo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gsjgyofhe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gbzkmcagn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gmcmtirxt.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gjgeivrci.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/goedgadqd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gekzcyrgd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gddqdkdze.sHtML


<!-- 参考信息 -->