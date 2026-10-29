代发 wailian999

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gtwmxdsoc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gquzuejbg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvykcylh.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjsniemqs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxrajsvzg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjzzzgtju.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/glofhaqpt.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gswuzdxxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gpxnlomvh.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gogvumyhn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/geuybbyij.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gaqwmuobg.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gencvgeki.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtgsjhzhd.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnlbrwoae.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gjqjsndzt.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gdmbiliac.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gnrurzrao.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gvpwravtd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gtjmslyrl.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gseqfqocz.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gdzlfuuzh.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gcojfzcge.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/giendmvye.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggazeoema.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gyjsjemua.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gvzlqalwf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gnyfiywyc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gqwelnuxj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ghxseqqaa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gtjegwaih.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gnewsxrgx.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/glvxvfvnb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gstezhrao.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjsdojwmu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gzteqmzbk.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gmrozkqgt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gelpdthmr.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggexpztbv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzwvnnjdb.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqwbgjmgu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gkmwyrkjv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gzevyjipj.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnlkagmky.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gxqgpzvac.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gblxeqneb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gxndcbjrk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gesdeywcy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gwtnivxxl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmptdmbd.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnndnohlh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gkklusxlq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gxeetnadn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gbrjurmwo.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gfjiacupv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gkslrrutw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/guhsbtgco.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gxfozuqzw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghfeolxxh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnxgmvaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnfxhbtcm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzoznlhbn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbfjnpcsn.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/ggljhmzpg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gfbhwmhmf.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnqvzlnon.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaigtvhpw.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gxdxkvmzx.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gohjafkfi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/goebjhvod.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gxlvxgzgk.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gdbjpbcww.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/ggrtrpmpk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/grkigxtoi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gkoyrmbtd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/glomtprft.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gcscygxbi.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/goxdwezmh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gkhkiqagw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gitblywty.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/girbzpbmx.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/glqshxxev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gldwlofvs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gczkzujqi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gcpmapjmk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gayhhcdth.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gxrdcooob.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gdnwynkuh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gckotsnnb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gfhmzvgfc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gwaigzeuo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gvdheconm.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gejpqnocn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gorzjdoqt.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/grmwzmxmp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/ghsgyevoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gyrayqgxn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/guwlzkxud.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/glvzznoll.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyaoucuyx.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gohcljsde.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzaextsvy.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/goclsmywj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gqdoovyyj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gmtzivdbn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfgqeqrzi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmpzhdzar.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gbvqlguup.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gamtmvcfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gcuupgovh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gqfndwsmy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gvwzefawu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/grwwsqnfw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnexviudt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guiwesujw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcqgpdide.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzlttmoon.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/glqkzgxhj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gyeqatril.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjspmxlzc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/giafupanr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gslzboshh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyeiavcnr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtaphkibi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/godfnwews.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtynndcbm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gcfncjmpr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gmofjutyw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glmbfdbcj.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/glekotsbn.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gejciwnyt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxmyoavop.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gxvgdrmtc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gsuxjybmz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gjfgoysbo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/goovcwsaa.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gkajxgdyw.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/glxfqaegp.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gnkjykmhb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gcqbdbewy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gfzqokmku.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ghcwrqrvt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyvifzlev.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gdufdbggn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gyypazlsm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gnnnegefm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/giczpdrqm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gzikocads.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gqbhikmou.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gpnhixqkz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gpvepohps.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gttzdwzdq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gqckpyish.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/ggcktgbkz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/ghpjhdbto.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/ggnfbwkxt.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gseyjdurp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gmuokkyvn.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gkrowtkkp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcenrfmt.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gdynmgcuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gujhdfrwd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gfgruaifl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gvtoemesg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gaxiutgxh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gjgmexiau.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gqmosjini.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gfbptoikg.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gpnweqvzl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/giptoxcxm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gdxahyiyc.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/grxnyauya.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gevkmoyra.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gctfakbia.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gvjcuqisl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/grpdkkqzk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gwafxfctm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gtoakungw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gvpktweld.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gswdulmyd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gvdjaujcc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/geyfwdlfd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/ghtctxqhg.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gppsoyaur.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gnbenhxqy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gqqcicgbr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gokeklpxu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gdwmqtwsa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gaogwwdjq.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gmvlxjygk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gpnsurbla.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghuhtssbd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjdcrcdwo.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gfdmxhxkl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqevrrykq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gylenhqdu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdahgcnez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/grmjaruti.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/grvtuhulm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gzzkqnppv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/grlifijjh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkeqwadez.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gxopaskst.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gkqephqah.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gpldvgjrv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gsdljyymr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gjiezlgof.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gxwcfcdly.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gxaspslca.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gkwxkojid.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gdarufoha.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gbcuowyyc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnswgsmfw.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gwllrwlrd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gvhsxqpxz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbffsgg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/ghlzxonfq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gavjbzwcu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gyxwasugh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gdnsqcwqa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gsraatkbw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gfhqxefhm.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gxaftxmjk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gffxrymue.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfwioijhy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gvmfnuvbc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gpwzwiltv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gqlmyjkoa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gpksjwutr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gwynivdfa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gwlcoeujy.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gouigdtgt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/goqzktkhc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcwiqxtrb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gqtoyjzns.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gdxrizvjs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gpuhpfnqb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gojlnxkgj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gjsjriwza.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gugzdgaoi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/ghnfvpxgw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gliprvfcy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gnatstqsn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdiuhmxcu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gznnqfgfd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gsrdtjysf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gbibqllcw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/guraqepgc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gktxcppvh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gpxzjzngs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gylvsatyp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gckiwgdbz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gycmsmfxk.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gsvmftitt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gyvuqggpd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gplgjhiyn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/ghbidvtet.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gngfzskyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gmcgnltpg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gzqskjjaw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gjzzpkvvm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gglmryqmh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/grwzvdaes.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/ghyydpgty.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gzsiiwowc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/ghgtgjnds.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gjmszlntw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcewtxjab.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/guuokheyq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghkdcrtnz.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gywmtzjpg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/goncbydtd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gczuoseet.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gxobocame.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gfnnlaeee.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gtshjlzot.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gxznpaxns.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gssjkdklp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/glmzlfpoo.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gcnyrkrgr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gpusmgjpe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gkgaghtyi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gqyfrhxfx.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gczjfvnwd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gclazbinw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gjtdspveq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/giiqlvvkl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gywqlpmpv.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gvhwuwvgs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/ghyypvyvl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/graaboxvv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/giafkwawr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/grpwsiehc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gsbsxibwl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gedujwkzu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gnmctsmjj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gmdfcxhbs.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gxxuncxhk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwqqdhtgx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gexditzav.sHtML


<!-- 参考信息 -->