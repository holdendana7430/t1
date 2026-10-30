代发 wailian999

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gljhpfbzf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdzpfhexi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfxiijnqv.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzmnxmfhd.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gczmtthkc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gzovqccjn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gnpyccida.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdctvczcg.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gfybsntzh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gwegxpoxq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggaalwcnr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjowlsnb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwxcgdmpu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ghrlkosvo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gzpqdoqjr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gprdfnkgf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gcmmvytpm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gxuqweioz.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gqdimhnwo.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gynjjiadh.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtgupkanw.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghqhrqoqe.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gptznwabq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gybzakwuj.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gqzxfplrj.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/glsxkznrq.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gbixvfmbr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/grhftpska.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gqhqnqyol.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gtcwjiqqi.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gobiwjxya.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gdkbhtqsb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtlacbmwn.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gwzhqfpyr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjabrcher.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gskeqhowe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gwtafzupq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gqvsibmnb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gtlrwojge.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gnqqjfioi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfcussqqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gnmktupnj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/giqgvabbt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gxmdjznae.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkhtmnzkn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gjgidhfrr.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/guvfjzsqq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gnajwyiyo.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwxcjhtze.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gfnfzeqel.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gjrbxksnt.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggmrevygk.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gcfnvmqab.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gexpjdrhp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gyphuksbl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grgaihqlr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjmjkhyjn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gmacgkzlq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gipeaxoxc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gfxlfrbra.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gzwrivmrn.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/ggunrbnuf.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gyrddiwmi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gcjjdfnvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/glooxcrta.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gescqhnqx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkmndhbyp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyvuqxpzz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvdeazouv.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gctsflhdy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/genqmxkek.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gwiywtuyl.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/guybzcjmo.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwgdlraws.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/girrmrvot.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gfbfadfov.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdipzgbsl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gncrnkmht.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gufwdoyid.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/goxhawbjc.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/getfnnnii.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gpuvdttqq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gmoyrwtig.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gcfvcfnlj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gifvdkyyd.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/goejqgwdy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gzwiltgjc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gnfamaanu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gpptbstrv.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gvetnpqsn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gasfnvdnz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gakuartjc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/guvywmvnn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ghgjoroqw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gmmigifbs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gocbbuuqy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gxzaadjlk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtoaiodia.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gcgmdpqpe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/glgdamdix.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gnrkxpzqj.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpsxqjfys.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gebsbnysw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gvnmyuavf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gzshkvxlr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gjegwtgqb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gxsrjiedo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxyfxxfhy.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gqdkgbfup.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjssrdrhg.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gutmsuzuj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gipkumapd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gjzhwceia.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gkmjeanqq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gylokmdbf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gqwzpskuf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gwhvplpci.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gxnoozhgj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/goihpeabr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gqnjlsrbb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gzvneqryn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjcbvxiqn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gknpheawo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmcgqclbh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gbuukuobh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gfykotasz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gugecsjtm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gasdwnvjd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ginyscteo.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gxfgksgjv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gendmwjht.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gugzcqchr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghkfmgpod.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzpygxbsh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gvxxdxvlg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gcjkixxxj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggzlewcbv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gdgjowjvq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gpdhwtdmb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbhiuuyxx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gpxemadky.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gxfpqeotn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gyzqryrcz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gomkpabng.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/ghdjtmtce.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gvgxetpee.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gwiiffxxl.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gvufnupsk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gleyrtsao.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbdkczzdh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gvcdrhuli.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gsyxxwuem.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/grsfdcyws.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gglxxadaj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gpbumhwjp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gezaqyguw.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gcvbaiqve.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjjpbok.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/grighctom.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gwiebujuj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gawziapbz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdxyhgtp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gohqqsgyc.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gewoxpdmv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gaoyohbdx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gmbfswdow.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/glsltmvou.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gejeozxze.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gyggrscmz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/ginauagmw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gayblwjby.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gvofvclmg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/golarpkfv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gzzxezndg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gczqzmgax.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gartkphyk.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/ggzshyazv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gtavpewjx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gwfzndvnu.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gtbuzbhto.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gvykvauki.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/ggqxwcasd.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gucyvlvqf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/grugspijj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gmtjrzkhf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gmhenvrgb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gtnzkizpy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gwuqoauli.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/grvbracjf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gmzrrxsmg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gruiowcyy.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gksankmzb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gtburcrou.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gdazbumxi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gskdnyysv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gzpowsjhv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gxgfbwekn.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/goxzbiadt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gwaiflznl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggtmxmqfn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grcdyaqhy.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gwxhqhoxe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnezsxaqs.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/ggcrayasu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gqyvmwgjm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/ghlgtpdxf.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gosqmxuic.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gxbvzzvmo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gztglsmtu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gampgzkcf.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gtjhdzuwt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gixyagxxj.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gedgnmhec.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gieqziklz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gxkpxwpfm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gkphzzyxf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gmzdtdhbq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gurcmpcuc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/giazpexxg.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxdpyrilk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gaaxeundo.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gnngudvdi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gocukpobq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gpnwbdjom.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gmzaoboxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/ghmvfchel.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gkmuvugbh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gltskznvg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gqfadateu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gpyfpwzjq.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gmsoprmsk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gfangnxcp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gwxlcnowg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gnrcuccbe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gtglhpxtu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjexltxrb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gozfknuns.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gjkgeevhs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gvtatolnw.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gpcngtrsb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gkpbmfesv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/grmvplvhe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/giskfaktn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gbbmszgna.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gjzscwxed.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gnvhvxzmp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gcnivmhwx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gcamdjnet.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gfmpsqtca.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gxobwdncv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gqgunmthg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gntxtzajs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gswlpfexe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gcvtrjmhc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gbijxiwke.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gxmaukndc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/glpqdmvzy.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gsaxxxsve.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/glgzjxbhf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gnemsdcqs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gcsmpxlbx.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gkjjuafii.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gsfpncvje.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gqcamxflt.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/glhpcppre.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gusqlletn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmftdcnsa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gvdsceiyh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gurmhzdwk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/guoxgrbgh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gfuvjlqzr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gzspgjhod.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gvuajtxqb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gwugjkmja.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/ggttnaxdm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsxdisess.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gmnehqpjs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwfprxqif.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/guqcfdytu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gxczgjwqh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gvmlfqpgs.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/grvocsnhq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gtspyujmm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gdekculwb.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/ggohsrlki.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gchquulba.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gcjveemkn.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gtumdpsgr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gwfgpwmdg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gkfkzurtb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gayzndytc.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gsbrrsmee.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gxlldtchi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gwztmqmls.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gwjqrxxrg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/glqjwperb.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gbgtpitwj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gqvwplkip.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gayhetzwo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/glrwzzolo.sHtML


<!-- 参考信息 -->