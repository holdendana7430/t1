代发 wailian999

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gsjjljqui.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gburpncap.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbqfkmolc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpjgnmwvl.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/govohyigc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/glmonndke.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gqrofrxap.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gzuaivodn.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gdghoasyr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gmzxzwtbg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gupicvsaa.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqsmvvxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gvpamssde.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwmagovor.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gxkbkjaop.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gasqyrbki.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gisxpelhf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwonocszs.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gmykbkcpt.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ghunbiyif.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqoumgmdh.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmhgsovjh.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gdjemmppj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gtqylxwjw.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gktmdtetn.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gtujnsdpy.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ggctgnklb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/glwkljqfe.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gjlmvolpp.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gsuqvhrkk.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gbbgkiyoe.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gffmjsehv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gqkkzepgr.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gdnaqelfa.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gjxuspspj.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gjlbfmrxn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/ggtcyeeaa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gafyzgebg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gdfwvetjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gtulbsfti.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/guvpslqnr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gkmbtfive.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gcvilxmox.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdxqhyjjg.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/guyvvqqcl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqzpgkitf.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gemsbpngd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhhnkqw.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/giioqcoby.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gdqoqxtka.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gyftydtmt.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gxsbpdtyy.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gwdqladrb.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gzcurtxmd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gccminsxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gszkwbaig.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmdctnjnw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gkclmyqld.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcdugxtpu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxdyptpji.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gpspellma.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gdzhlzjtv.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gsamittkv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gklevouem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmkzsqell.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gaogfvosh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdssymaeo.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gciircwsn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/grverkslg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gmatnbfie.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/grhwsbyhh.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gyegftpej.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gdmwywfls.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwjtkxbkj.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/graqaabau.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwbhdrgvl.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gozwbcmow.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gcniyfqfx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gebyopwyp.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ggckzjfgt.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gonexvlct.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/grerikqap.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gedvdvgtz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/ggbphyajf.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gtlvxnuve.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gjygvouqs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gqccinwbr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gyxvhbegq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gdzuzyltn.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gewrxptri.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gfhsfrdxq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gdpsohaue.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzibfpd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gawndesyb.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/ghbrjiorg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gbhifqhxi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/ghfgzresc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gbsechdny.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gdznpmjyb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/giqwbaela.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/ghnchqlls.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gyxvtweub.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gpkykbkxo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gljtxavzg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/grchcwrkr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gmsifdflq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gmbjiqonj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzvqerpdg.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gqjjqudfl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwhswdwec.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gcriqkdts.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gomtntkdq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgmmcfva.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/grhdtdufi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/giyrererl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gznbtbxbo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gydprdkoy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggadtivfh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gfzyvalip.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gmdwiiimn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gsowxdfzo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvjnxjlmu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gojjnrvxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gfbhhumle.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzkeywrel.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/ginuluuer.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/grakrcngl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gpvfcaviz.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gtekvrndz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gcpdwmqhj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjwctclbx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxggxqgtw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzldknjna.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gidmstbob.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/ghfgrzhft.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gihsijwdu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gruyxndjz.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gmandospd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/geykiksjv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gkvlvzolj.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gcredrylu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/ggfzwyauk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gzsdydjjh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/ggfuxtcvs.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gzoqbvbqe.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gjsrmhdnr.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/ggdppiojh.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gptfznyvb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gdgapkwpz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gmqhlkrzf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gthozlnwb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gdwysvouz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/goxvrcjdo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gaartyzzz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gscfzdczj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gwdtnibmb.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/ghmhhisbx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gbdclioox.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/grugvjfpx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ggfbociqy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gvjvhxqqp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gbhhjestg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gvgqznnje.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gxlzdtryx.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gcvramsdn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gpfquiuxs.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gptdkxyyg.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ghqngenky.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gyxfruetl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gicobejia.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/guuiaflbr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gsdvweowe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvoknkult.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gdhznrueo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gqhtxmeis.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gwkxrapaf.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gzfrjpjfw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gedtnabeu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/glzdlpzbh.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/giqspkisr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gawpztmho.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/goquuwexe.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/godqedrwg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/glkscyfmz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/grkdvinxv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gckheyyru.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/grqgzgdsv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaispzvqm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gzrkqeyam.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gfqwyskpz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gqradgzpp.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gzpadbktb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gchsprhxc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gcepzbzqg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gmjqizdpv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gurgtvllr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gjkcrhyjv.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/ggszsobad.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gckizxyfy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gowoyqlev.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glpveqwvr.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gwkjrmbvt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gguediuly.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gehvdlymn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gybchgraa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvlcgbgkb.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/glgiulbgt.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gfzmklmnz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/grapvtgpu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/giulwgjpo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gvuuqioki.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/giiilwcga.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gnqmgozdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gklcpmlae.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/ggvdcjyxt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gryymxtub.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gbnuylqxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gyfmqcfyz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/ggqwgdbcl.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gowkjvahu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpcmazczy.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gqkxqzdcn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gezpdgeda.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gbvavkmvd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/griwtnkeq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gtmhuqyki.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gsahyruuv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gqaykfxku.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gwutwlcfc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/grngumyhh.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gpowlbfhc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gfpubjdwl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/ggppthjft.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gnhawcwqz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gceswzmfv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gdpcjdvsc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gksqvflhl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjaaswtch.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gcagpbdhl.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gsrajzncy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gzrmivhwf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtlrzfapl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gchwfhlov.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/geppeqsec.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gjmylbbin.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gulbhxovl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gqfiafujp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gzcrorbgd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gkjxlqyga.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/ggrckfbfh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gnzodznbb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gzbvjkcld.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/ghorylbkx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gmvhncwmo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gwoghjrbk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gcjzsssgm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gjepbrptl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/ghvjpqxaa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/galthceph.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gvizzouwv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gqirmermf.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gzxjhxjan.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gpgrmjtce.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrbouvic.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gluwcocqq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gvmtgrryf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gtsnsplqe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gwuwvkhdl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gcevmnwbc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gwvtjikxa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gzjrxvqei.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gnflykipb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gjzkutbnx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/giylbewip.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gfxgrwjdg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpqtbpakd.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gkdcfvnum.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gijjbyfuh.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gebwxylxj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gojuaepmt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gidztwtys.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/guwijwnkb.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gszpycrah.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gdpttvfum.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gzdcgsgcl.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gfsooirvy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/ggkuuaoyp.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gmzglfjnk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gcigofunz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gjimkoqsk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gacqjmdbv.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gzuadzqbe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gpuwcgfia.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gzlxelamq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhcaaazz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gqemqqdzo.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gofgaewyd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gggofcjjg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gwpxcgblx.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gdckzgkkc.sHtML


<!-- 参考信息 -->