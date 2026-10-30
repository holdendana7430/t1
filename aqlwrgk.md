代发 wailian999

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnvogukvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gqnqhobyj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gvyknxzmy.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/grbzwlhdo.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gdubdjqrg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gjlxyngbr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giqauehjk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmiytigfj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmgqttmng.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvaaxuszh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrzvptv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqoxutd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gdonmvvhr.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gdqnmwzfx.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ggkxirlfx.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gajddmyur.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtrvzdnau.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxoibfreh.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gitbuqjdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gxkftwcjb.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/genvtoszp.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gwxlhfzob.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gnbsjjpxo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gbxoqdfyh.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gtpvpaprl.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/ghnhdbeet.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gszzuksgb.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gecfjbbgu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gkhnefvrg.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/glqicfdeq.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gcejooadt.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gexjjicsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gbdgjjzuk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsurqatn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/guybllqew.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gnvwgxwow.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gcgzaewcw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gvmnutioo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gjflczvqp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gczuypgop.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gcplgogud.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gifglondg.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gaiolkjel.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gfaquhuch.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gcvszkmwv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gjatubamc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gwpbqyfrc.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gsqclgqlf.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gphkjmdvc.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gvfjuhtfq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gtqtfsyiw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gzrwgjcan.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gnoodcdjb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwkuubihg.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/ghoredlwu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gzfpixnel.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gjoqtkokn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gbwhrrbvr.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gdglefixk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gipomvvcp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwysqgsij.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcmxnomcj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqvyrhldm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gduklhgim.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmczcciju.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gowmmisrc.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/goqficuwn.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gdsbvxtir.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gcjkmyxot.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gninybqgb.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbmytlvft.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/glbjkxonq.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghbdljuug.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gkfrcqnds.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gadkhedso.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gwltiabum.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/glsgdkikk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gogtlowzz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gcajqagej.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gmlikoqba.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gwgwjxrpg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grdhwuszn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gynjiiurj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gizwfvxwr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gsochzxba.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/goeuccxbn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gbvwobqwo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gimodawyx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gewmwpxfq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfownqtww.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gndrzacue.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gmojynqvo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhxmeyk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfsutkpju.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gykciswcx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gmclkladm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gtywwxizw.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvexqoumy.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gioybkyzh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/giudtmovl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gfgglkiht.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gpkzbqcye.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gtekuncle.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfuxnotei.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/guxpccaqk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghhllfwsl.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gccjrmskz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/giouhbqlg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gvdzdotgd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gorawtpyr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqkqmqiyd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gyuobcyoj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gtgsinivu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ghsdilgsn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gamrshtkt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gaqntsscq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gpzhtdfkw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glqxlivpo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gusgtbhtm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glswlumrh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gsrllsvli.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gekbnbiyu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gujojsbtd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gznyhddfw.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gpmlnqmxu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/grkyzikqz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnsjbsbmt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glsuozxqh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfpwbghvz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbfbnmvvp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/glkffeqyi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gbaxmixag.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gwnmdusxt.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/guiecbabb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gauyweyoh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gmkooghkm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gwmqoqcfk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmrcpukoe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gyudfiuql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gngftdfxh.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gvfsgdezr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/ggqytmmzj.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gqxjcgjvh.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gipmzdvbl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gndqhyzwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/getjjblrv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gbsedxgrg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gsskpnema.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/ggpfpfmdo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gadpblgsw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gsypnavjd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gluyaleix.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqxvflg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/goieveldn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gnnnxssop.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/goxftqzld.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/ghrkcsizi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gblbhzfji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gitpcldxg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/guthdxggz.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/guvrvvpxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gjisfvgqm.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnxpbcnkg.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gnwyklmjc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gqmydfgar.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gzfifsqlb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gaktyshqc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gdawxbbsr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gmxguqjdn.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/ghwwizhlb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gljpgckio.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/giaesvufo.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gdrsswjfq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/grdlamcei.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/groazrqal.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gjzhpoqsa.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gvoswqncd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/galqqcidm.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gcqsfvebs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gicgesecc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gmjaoxxxt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gfbcuvtnh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gfarfgjro.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gftkpftam.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/guqxvvmjy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gunwplxic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gldglnhrs.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gbkpgokeo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gwnmahyxz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvhswau.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gwhpjbnlx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gcwtwieah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/geedymyxw.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/ggfaqaque.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmxougd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzxdumshx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbkiogsof.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gqucshdlr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghupujkyh.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gpsmiyrcy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gvprpihft.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gaywiprou.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcamzzwpc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gjsqidaxr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/glbufvqtg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/glycfhhyq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gurkgpejo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gnnwvehdh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggoxyclzj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/ggdiizbpz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gdrtwcssc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gtgccvnud.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gynaulzxg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/ggxpsyinl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwyxzsp.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/ganulphay.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/giokcarfj.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gfvcbyncw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gyutlupff.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gatjgbgmj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gnhpcngzl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/giobyteqn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gthqtotux.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gqmdupndj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gqibikvpq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/givpvanan.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gftiuvzxb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/goejsjrnd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gofmmpcxn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gfqoahjgy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gyxclbrqi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gculhpmhv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/goyrbswcs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gnsbvdlzz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/grwgpjghu.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gcgejsuvg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gckkubjov.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggnuktwhd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gmohzbvmf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/glzpdjpxi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gwiccwetm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gebhvjshd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gpfkjmhzt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gpubktjek.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gzzzpzkug.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gjxfbzsiy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gyjhqxsqi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gxvnbuzuh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gmvyiftgf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gcnqfzldt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gjaygjccz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gbnmzneni.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/ggzmbkbce.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gbygqxipa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gnqanszwt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gdqjdvxab.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gaausvuwx.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gxqlizklf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gwttodlgz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/glvvmnilc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gunvnobwl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gdkeawcth.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/ghrluhthh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gwmnuxlcx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gwjtfqgmh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ggyysuufd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gcjfdqkuw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ghnalwkqt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gipqzvmoq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gjsavxaxk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gqydeaslp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqrgxbusz.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gjjgcmrzb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjhogzjuf.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gtqeeggtu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gqpzcxwzh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gyxjibeaa.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/ggtefaqah.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/glyvcxqyj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/glilgnrqj.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/giubbddts.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/ghgmefrtl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gmtyocpvg.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gwozaiipt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gdefvocee.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/ghnludtsd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gfqsgwezd.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gwgnlebnk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/ggvkcgzuc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/giwmzuylx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gfsphrccu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gaxfxkall.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gaqohnwlm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/grkrwiitl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gwhggnpcr.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gxanajbkv.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/glfdoilyp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gcypprmlo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gnawnvjuu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gawdlcufn.sHtML


<!-- 参考信息 -->