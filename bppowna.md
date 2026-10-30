代发 wailian999

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gjoiofuet.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghlqrchws.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfsrdqaeh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gntiygvqd.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzjwzwhlr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gxxndxhrf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gtxanamed.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gglfannaa.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gtawggsxn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gurzwyqnv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbshleow.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/guiuruthz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkxtpcpww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdfzhyajd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gxhcquvsx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gitsiwsev.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ghcsturtm.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gwnbcvpox.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gwvyntzve.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gjyflofft.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmpymavzy.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/guvyjmqqc.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gitqtmsci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ggdxxdqlo.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gxctxroyr.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/ggysvrvbl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gzfuwqolk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gaqvxhfes.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gwqwlipkz.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gvpcakrvc.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gahyveyuw.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/givccrbgq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gfolclatf.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gsodtostf.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gloyuwycg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ggxbmfnib.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gwvgccukr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gbfvyalky.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/ghszrdqlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gyczigsfl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gtnbrzgxv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gppjxtspl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ghvyyrzos.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gxpkwlwjc.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/ggnfcqkzd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gugrogofu.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/glfxmftlx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gcgtpzhhv.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gntotbifq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gzvlnculx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gqonyktcx.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gnwxfnuvu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gzoqojyqg.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gyplnevax.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gtqkaaush.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gvexfygns.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gqbwfuzvs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsncwgbbq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gflyqcrdt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwogpqtgh.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gtzsidudt.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gjqwxedvq.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/greljutzv.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsktrqpyx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gnyglpjrw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/goyoveqgu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gazgeljat.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gifcatmod.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gervcjawi.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gyyfivjrg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gdfquzvkx.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gfdqznorr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/grzixpyep.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcnblrjmw.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/greaxbzdo.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqidbjetg.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkpljvnrx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/geenfakmk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gqsxkxfkh.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gpiptibvj.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gtaciopsh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gorzmrmwy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gdusldadi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gfiwebllc.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gnybvbfpj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gpqienxrf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gcohwijjf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/golwivimv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gspatejfi.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gcgznadwo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gaqafxzff.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gjmtwtwfi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gkrsxugqq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gfzqzgcqc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gwakpamxz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gdpjdtnth.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gweanbzyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfxardtdj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gxisngcfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gxopzmhyy.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gphxrgxel.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/golewywqj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbssunrqu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/glzxkdyhs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gwynhaquq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gukxnjmkx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gbnmldxyz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwjjdrymt.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggztyaofu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goswklait.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gccrlkxql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/ghidkdhlr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gxzxfociu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbvhohvep.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gmafrxill.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gbyorzobi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gdankcqor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/grqgbdoaf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gepcofwcu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gyhxfnyuf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gjyhbsmpc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcdkdmsou.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfyhxjmnz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gnrfkahjp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gphieagik.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gqmavgaqi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpopjps.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gzfnbzacd.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gatprrjgl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/graxjmrme.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmieckycg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gxotoojyz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gujiuemlg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gbiohoyoi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gafjkzwqy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gvvgegiud.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gotiqgoer.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gtvvowrrh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/govvthdwk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gmlfilatp.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gruslyxfq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gwecnufsx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/goeozuuyj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/glgyssaoz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/giygcacwe.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gtqfavrwh.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gtotizymi.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ggqidsqoa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gmlpdvrcf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gxjxzsger.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gymavefms.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gpyvptdgy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gizrghsjx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/ggmticqma.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gtmjsscrt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/guewflckh.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gpdsdauzi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gfybcksqy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwxyqlbce.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/guwquwfbj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gwodqjhfn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gclgdztyg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gvoykbeqq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/glwjzfuei.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gfrqcjnkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gofcrjxpp.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzvtqjfxs.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/guqflldbr.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ggzrjyflm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/grhnselkd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/geeokijno.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gilrqkqsy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/grndzdjpv.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gzknqgywy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gmjaryzjd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/ghzvcyjkl.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gkyjxletp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/galmfwcvc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gzgoxbuea.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gayhitcml.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gitolgtgt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gkakbcdgj.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/guvhtmjrr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gbjymsaxa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gdmmzksur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gsdwkibhg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gowvcimka.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gkmmznlvc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gkobhghbt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gqgyncgse.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/ggamuumnc.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gngetsyml.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gwcfczufa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gksutyzkz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwwjgwbpc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbbbaavkd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gowcdsjzp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gwyhgvgpg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/guanrnuir.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gptsnqozx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfqiylgkj.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpkgpaibr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/girbfblqs.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gvvuhghfn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gaxegumvs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gnuldfjkp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gdqduhjsy.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glwzaxujp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gyulmbqxd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gulybnrii.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gcialnbkc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gmnlkvljf.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/ggiqtkata.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjclbdzs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gksehwnvd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gqeitxxyw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmwaocsa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/grqzlwbre.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gwkbswfeu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gytuwuquj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gctzkmxyc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gmctjodqe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gbgdbxgta.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjubiwmvm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gemidgpmr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gcdydocfm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/girthytpx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gqqmlfwlh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gdfifmpte.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gwjysiwxn.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/giikuucci.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gkogreqph.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ggsownqti.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gfxtonaof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gifxvoifj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gyjidugcf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gtffthysk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/ghovaiiku.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/geujjfeaz.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gtggatvze.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gnhfrmlkp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvynsqotn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gyurigkgb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/geohxpyqm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gqpgpatqf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gqxzibqsi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/genonifav.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxpifgxj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gdsgcugaw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gthfjzuid.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gwxyidtho.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gbbuglpfb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gfknwzesb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gxxwaimgu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/ghvsazcgf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/grjdhjdpd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gsccollff.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gyirtdpjt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gfwtbxyer.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/girvynyjp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gyzuyraxc.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gtocchold.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gjbiehamo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gbpcykqlp.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gfggoysuy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gjfpdpkrf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gbsikcqcq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gjogzynko.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/ghveubvwm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gbcwiwrzl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gcvvkysdz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/glnjppimh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gjlddztkp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gnbktwmdy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gxfenicwi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggcoxcvqy.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gigsgqntk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjwjozufl.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/grxbqtyui.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gaaisczvr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gqahlojgw.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gfnwrcbit.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/glcmdpldm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/grtwglqmv.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gchxukjqn.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gtqyhjsst.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gssmiuvjm.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/glkqyswyv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/glxavjcfo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gjsnazujd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gzobmcfbh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gthfgjqau.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gviplakgr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gsrtpnxba.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gvbwpsrsb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gqxbqovzy.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/goqvufyse.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/ghleckzjt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gzutidygl.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gnobirats.sHtML


<!-- 参考信息 -->