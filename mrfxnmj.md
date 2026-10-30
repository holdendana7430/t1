代发 wailian999

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gbkeyfqgn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpeqzzvok.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcfjwgpos.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggjleegyg.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqhydwubr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gveufbcws.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gbgecikgy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gnlnjpxnz.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/ghppacgdh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gqgmtqbqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghryyixya.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gggjlxsyx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtdwhhzdm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnzjbiago.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gunpufbpv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gypzlejld.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gabisybgf.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gziyaybwu.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gwvlikhqq.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gmjrbnpow.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gfrqejxtx.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/geujigeoa.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gcnwwncuj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/goixzzhgl.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gmbfsiwew.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/glwbzfghe.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gctjbgjry.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gisxsayfk.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gqoqfqsgt.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/grkivxqlc.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/grrsgvxvn.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gatykhbnl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gtvgfsvre.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gksrunsaw.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjrqlbanm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gonfszheo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gxnspdpll.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gupfnaqvo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gnmurvelj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/godwchtdu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gfukncvdd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gflcglbzm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ggdqjyitv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gcxqlgijq.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/ghkbxdizj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gnnqpndeb.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqfpxhwig.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gqwryvpxd.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grydwbrpx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/ggkhkbsks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gkyguqnes.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjoxrkpyy.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvihpkkbw.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/geofyfmso.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gxilrxoqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfznqhacf.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gftcvnpdx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggxzepdnk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/giexgernx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwjpkfbqa.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gsepqstso.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gdjkmoghj.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gwmjgbxyq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/glxybampu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gagtsecjn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gohntgzew.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvfeakfbv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/groatytpt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gbpdwpbfn.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/guaphvliw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/ggjgiupwm.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gqgxvsjau.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gpamorfcl.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpjklkkmw.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gkpqkvdgn.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/geqclooim.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxsdwvbqt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gtvienxiz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gvbsbhrdb.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gbfgrnfga.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gerylphtd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gcncxcllh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gunbqjccj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gobfraedn.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gfwhkzbfh.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gbumjvftj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gpayoxuio.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/geijguuew.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/glwnvhflh.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gihhduhhk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gnuywhbyc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gkvqueyhn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gmlpobpek.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gvbgfpibb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/glbwmcxal.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gqgkvsmcw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gcrqjbqsk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gyqptwrpo.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gztaoinuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gcalnzvfj.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gjojajvwi.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gwsvsprtd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkvfoqmbi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gpnjdctbe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gubxxwafr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gtqyswloo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gxgqgvsjx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grxbqfnzz.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gnsgpgdsn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gocxezefd.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gtyhbecij.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gnvautgvi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gnbgtzaex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/glnscbxks.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gplevcxji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gtxahslhq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/guxsbzxaz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gexfvxkus.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gdvmspmpu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gkodyvuzl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gzzcfselr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjamphgir.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxmabhxju.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtzkqtfrr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gelnshwzd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gdvxfksrr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gpjefbzfy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grxdrgbnj.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gnyjggybi.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gtdcehylu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gelfenmcu.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmjmfnosh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/girhzjjdg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzbmhihcn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/glcqfqfac.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gfdhwemee.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghmwqiupp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gmsnttumc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/grxjqntep.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/golfncslm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gnddbybbf.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gsqfalqjy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gjjatlsre.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gjemtuzpf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gcbskwhjt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gkazfwvmy.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gbrdrllaj.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gbrfsrbdx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gqemgflcl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/glsbfvdjs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gtwmfoaof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbskiqzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gxaypvbgm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gvoknrkkj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/ghvtemwms.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gtrmsqvlw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gxzvjbafs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/glndxnxjg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gijwwknly.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gportkzob.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gejjbaluc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gmdpkteag.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gszornsuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gautxknle.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gfvhyjzte.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gvhxfhdzs.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpsoxyvbs.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxazeyqpt.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gipsopmnx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gnuaryyqs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gtgcsztvu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gluddadat.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqiacqfdu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gycnwmbsr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gwhkthvok.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gvtrxlygx.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gozqzhzur.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gfjsrbgbl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/ghkdzerpi.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gotxcitlm.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/glrdvqvvy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gayakphxi.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gvhcrckrr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ggcvrvsly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gepyoemtl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gzeabujfx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gdmywufsl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gfkgzyfke.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gvpnavgfp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gjrayqfej.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gysblefqw.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gwclbicux.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gbmgtfsyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gyccligvx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gidvnyomf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gzcivsvho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gkcrkatqx.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gosdzgtaw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gxhkdhtdb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbuvuicxz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcfulje.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gguwdlrur.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guzhckrgl.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gylwmfngw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/glryhfjup.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggittyign.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gnuoxzphg.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gketgphsn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/ggvuxdogl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gazygqkno.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gckcfcaek.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gojbfaytn.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggdkvytph.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gvqdnepxa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gcuviicgu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gvvovwqtv.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/ggfynmkpr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gmrquclus.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/ghfwvxxhr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdjjhrm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gvkhzqvkq.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gqqnrlyqg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gubttfupb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/ghobbglkh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gchyhnfnc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gylvppscx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gvgoahfze.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gyuqhkrlx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/ghfmppatf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gunrkhnko.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gyjfjsvjv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gmsrmjfzy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gmfriklrx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gnntbfddt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gvspqcart.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gmhawobdk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gsophcgzl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gbqodogrt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjhreilfh.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gyblbtyuu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gvtwbrrws.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/ghqfzfbnj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gyeiacqfj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/ggcdvtdrt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gvtcevvbq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gjbhygdsv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gcswmsmon.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gwxjmberm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gnstnqmqm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/geeyimsfb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gwxhyalbz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gkmdfjkvc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gwqpdqaje.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gbntxdilk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gznsqqtad.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gyinbvgfo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gwyksyuko.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gxfifdaio.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gcfcrtqon.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/ghxiywnfq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gfaluqksk.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gkpixzjqb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gexgcwoyn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/geduiapza.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gbeinnhmz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gbiglbsqb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gvjmsxemt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gpvwsvdte.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gctcoajao.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gqgojmied.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gyxzitvot.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/grkjbtzqt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gotnpoxke.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gsnqmesez.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/glyrewbgt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsnedlobu.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/ghrlridnl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnegrokqi.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gvixisiby.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gocrbxeqp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gixylfnco.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvdfnxtu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gkafyckza.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/guxmfgyoe.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/glazsybhm.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gpedsrjoy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/ghnerjpzw.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/glmcibsqz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/grgbqyfpg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gdaloovrp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gqjltldzf.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gpmblhgms.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/ghsfjhagy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gfaayucdf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/guythyddd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gnauwcajg.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/ghknlmhiz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gqlstnakg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gxerzadea.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ggfxnppli.sHtML


<!-- 参考信息 -->