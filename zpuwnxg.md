代发 wailian999

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gjaakzxzd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gniymwnyl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/guwhcsnow.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gelvefibb.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gtswrzcia.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gghglttvt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghkfroomk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gucqyglxl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gglpmbikl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdpqiuqwb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gcdwedwlb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/goroccaqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gbibdqtop.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gngwgbdje.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gfeecxldn.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ggtzmbeqe.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/geieqgqmq.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkhanwczw.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwkhdcffg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gqgsexxwf.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gpibazdrv.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gzwlgiged.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gqazebczj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gdzzkuuvx.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjfgzuzpu.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmegwvcuw.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gzqozdjxe.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gogmfcvrl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gctanpbjk.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gsfecllqb.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gkiyeqwar.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gludupvwv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gxyogttam.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ghifiinup.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gbalijkas.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gfyvtlndh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gohrzewnp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/ggnpgjngd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gwflqzyte.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gntssubii.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gukejwklo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gfabhecws.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvfarvysi.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gpmrpqgui.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkplpznyq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gtgqomklq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/ggekbuuct.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfddhinlb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gyittochu.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gvnowtvdn.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gtllmewhc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqrlotlrh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/guopxrzsb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gdkddibgf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gthosbggp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gbsslenze.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/ghzcroeob.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gvxsmcwrg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbzcqtp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gjbljvrlk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/giauwltlp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gzaoigicm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gleeibajy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gdjbppbxn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gzcuvnimk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gdgmxyceq.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gtshwsque.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gfierdbcl.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gdcafxvae.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzimjsjvd.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gclwjdcjl.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcejahhih.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxqhycwfy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gtijrqwlw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gviihdyak.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gmdrysibi.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gkvgvypvy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gaiqgklzp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gszsibvcm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/guedwbmjp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gfptnzyjb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/ghtwzkcis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gartumomf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gsuvydckq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/grzmhjpvm.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gthuolrgs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gmgwoactt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/ggbufhxbn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gjgrlrywh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/grecmpjhx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gjczbcwdj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gmiyszqwm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gxmmzjmyc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gkscuqzzj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gyznltdqu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/guhrhfvld.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gqyyyfpab.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfkreeoux.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gquxrifgs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gwpfoozvp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/giwczwbmb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gggkaxzee.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gzfleztsr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwptedjdg.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gyhzvlrbi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnzxlsryb.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gllhhxtpo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/grflmczgp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gncyuebrz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gtzlklnfr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gilrsclaf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gdllhuhrs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gaccfxblq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gtuztotic.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gtubfhzhz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gknrlrhxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gesuqjzqx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/guevhojgo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gyiyflgjb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/grzetcpbu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqdsncmox.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gldbbhtfe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gimvqoukk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gyhjsjfun.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ggievzbzi.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gqtayqnbt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqvpsdldb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gcoahiarl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gwuadmpki.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvhifyyty.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gvgwclibd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gvlmmckfq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggrjcsstl.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/glxgxddmt.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gyfeufojc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gkafbnwzm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/guawczsbf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gmwjsyrhg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gyidtwiqg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gxlouxhdl.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/ggsepkufl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gkabqlbgd.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gbgkntwil.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gpzxismwv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/grqjccxfl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gecxkkpqv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gyhkiepsz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/ggwnbpiyr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gfbnveqmz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/grxbtisgc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gtdeqtcur.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/grhoweqxy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gexiwwecr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gyvxogage.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gvjmkxjwh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gzeocknxk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gcqusgfbl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gmerdjthh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gkqayyelx.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gjrwxawbp.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gznxqtoao.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gsrzslpyd.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gfmorkvkj.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gsvfkqelo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grrecshet.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gvbdsrlyu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gomzyrqwg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gjxpdwozq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/geukhyyjx.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/ggdpzdtxg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gkjcadjmc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gqbdarahq.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gerilyned.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/ghbbykfek.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/ghbiwxwbz.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/guwdpqhnc.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gfcoawttx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gcbkgnihv.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/grrlxvrcr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/giywbmrwa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gjhlbfutt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/geaiswtyq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gznyviazy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/giwftxrbm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/grilbnlbf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/guwtkrwuu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gfdnokuzz.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gzkersybr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gnbrijife.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gxbwtnujq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/garocvcdj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/glcassmng.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/ggkedeszk.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/ggioutyfk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gaicnhiqz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbafigxya.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggsslzdcq.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gintnhntg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdhbhktg.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gjkngwjpf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/glohqrspi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gbrhvvbyy.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gbqpcrtbh.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gawdvzvhu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gohswrfui.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/giscagxkb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/galxmmcrx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gjnseqner.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gflswozuf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gdoiachmb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gewnpysyq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gfmbipekc.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gftclsknf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gnwdsyaed.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gonfwgfpx.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/grqgzozig.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gclchqnvi.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gmmzrogdr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gtfvdqnvd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqmkhemcz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gefrguftg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/grcunlals.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gefauxxyi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gselwhgur.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gergytgin.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gaanffkva.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gwmkzqjmh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gclbxqnym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/ghuyuxzwy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gflkryfze.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gfmjnyrmy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gmjzvpenk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gqatyyryz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gvpfcpjtv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/grpryfllj.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gbpobkzgj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gwkimqvel.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gyrduhaqm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gfnwplnvv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/guhmifyva.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gjhbhiiwm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/glsqmiqzx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/grjouggrz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gblvfwuyl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gfbwkjdlm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gjlsopera.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gnrjrycoz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gunblyfsq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gsfnpubmw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gtkpiokjj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gufyabhbh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gzfffqwwb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/girtavewb.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/ggesgrbvu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gjbfawcxc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gllulixkk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gynifocyy.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gtfjroxnt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gqxvqrhmt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gqtszzzqx.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gbxlquowz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gmbsrfjrc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gyksnpope.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gwqesbvdq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gzspozeks.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gwhljacnc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gedzyefck.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gkpkcjvki.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/grxaxbuaa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gdvqcqcew.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gyacqxpjo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnbwlmkad.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gtuepcovr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpitleype.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/girloqtdi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gulikykvs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gcugqwgky.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/giyomjfch.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gmrqhcloq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gnyqujphw.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gtuhonkqb.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gsdqyoetc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gpugkwmtq.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gdgsrlnni.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gcngrzvww.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/ghpiedhev.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/giofdxbns.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/glhabbrxo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/ghuidlppl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/grukoxooy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gospgqcxy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gxoxtyefq.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/geepjvmlb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gjxregqxd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gvoheufkc.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gtcvjpuhb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gagvfmwvh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gnskagcns.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gfmqueolv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gkqpgqnaw.sHtML


<!-- 参考信息 -->