代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gsfnesdzi.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gndjzhxvy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gfqgzmbec.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/ghblbtdwl.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfctjkgdw.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbsnejzac.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gemudbzoi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gnzokoexw.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/geijcsewj.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gahynnpxp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gfldaqvfz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqzxvnybi.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gjoworsqh.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/geyvjzooy.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gvyeyjqic.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gmrlrbuxw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gkenihjdm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gzxhxwabi.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gdrrspzhd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gmrrytaqi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gvchnvakx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/glifqonbq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gsuwnrqnq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gxmomjaih.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzkqnkfvw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gkubijvgh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gfnnmqziy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/grrwhfmss.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gthmblnfq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gwlfkxvej.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gutxawrqu.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gjibmmwvc.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ggwopqioz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gmoceofoj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gplnwimfy.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gdgsbdxhb.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnqtjha.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/glgdjmbjj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gbvjwfeun.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grtmyjkzq.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtcszyvqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/ggeqlxreq.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gjcrxaksd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqcszysin.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gblxqflvt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gxczggjsu.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxrbhrqzi.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gsikdwriu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxgdmiiwk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gaqbjawzb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzffobnns.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzylosojd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbxfgrwih.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gqujxrlzg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghagwpgth.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gzddevhsb.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gdwqcifcr.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxbuskdpm.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gttslamry.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqjvpkaxu.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gedrwcxtr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gzrdmcekr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/ghsptmfrv.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gkgwkkmjb.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gvtpdgopq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gyppkneym.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gjpltefeq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gchsztqow.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gxfghtpgr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gdrvsestd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gwbmzvypv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/geonyywag.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gvsrwwsxw.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gycgeerxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gnwositqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzktjllye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gzyoyrmji.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gxkxtbsbi.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gczmdhvsb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/goranrdjj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gdmxbmqdi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gcnwmndqq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gxboxuqmh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/grzcseofc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gzfgjxtay.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gyogvyqht.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkvfgdffy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gwdivonfu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwfkoff.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/glakfjldv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gvmuadbuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsfhmdovs.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/ghlxdmwlp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glxsstlov.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gbdxqwyxs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gdbbvtuug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/glocvkpls.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxdqbtntx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/givwniwah.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gjzegygej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gricqfpvz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gddiryxas.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gokdofzat.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gufucaavg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gmqppkxjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/godipaonz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqhqudzkz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/grbezboed.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnmmwtoce.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/glcigngbp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gkhozbkdi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmjelacqx.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gqsvrpkrc.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gqqclttbu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkltnlerb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvuvhwghs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gstbrwpys.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gpdcakwoa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gdeesawwe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gdolqufyr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmbbwpgmq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gbolyokkm.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gsbqbedte.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gekarsfca.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gqretzyij.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gmeqeqyda.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gzrwadfle.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gdflvfnet.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gybvvytok.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gierzzlnf.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gklsccusm.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gelfrxfrc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/griwoujkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggtftcjbi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/grwuytscr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/guhyzxutw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/glgkqiccs.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gmrjmqudw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/grpkrktsb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/glguuzfht.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/ghjjnycla.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/grrpelrvl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gqqnaiydd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gedpxwlna.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gyodkhfku.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gxzzfhcvd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gxuexoafh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gheannfrn.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gebrtrsmd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gjpwzwogm.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gurcqcyix.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grwacbwak.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gtekyxojf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gutkkatnk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gmncjoexs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gftyggvco.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gqdubfrci.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gcwvjmoza.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/ggzedbrfd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gfhzxdkgi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gvqglvakw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gjgyfgqfj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gtiiixpbu.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gazakkuac.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/guxweognk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gggnmycrb.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gnrcakofg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gblbpyhmf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gnrlasbcb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/givsvzezc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gpeufyyqf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gedsjbkal.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gzudiwfbx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gplcdwxzh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gnncfuvsf.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gbbaortxm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gmankeloe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gkwijopao.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gjtbsspyi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gychrmhjp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gacuquhjj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gdwwueewi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gxbhtivjc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glndiqiwx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvcrlwblx.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gvqzsmeol.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gritzutbz.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/guytxanbs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/glgrngnpj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gsizdoejf.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkaipkxjr.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gdjvelfli.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/grtuuqutn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gyatpkgqp.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gnjbmhast.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghifsinok.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gygjnpuyi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/guuvlfjdp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gqbjahvej.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/goilqwnsz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/glmrgrjzy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gqizkhkdj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gfgymkdtq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gsdrhrzcb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcfrqdwgt.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/ggaeyuqaa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gqdcflfyg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gsidseyuz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gyssavgqc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gwwboexey.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/glprkbjco.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/glneplwlv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/goucuaaqp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/ganmchuwu.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gmsnqvhxo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gponzblrq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gvphnmtok.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/ghbskhfus.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gqgpsyynp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gjyqxhrlj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gjnttrxap.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gprlmnhqt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/glzhnwrfo.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gejyoklzi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gmozlvtgk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gaoddyuzt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ghenbrsuv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gqoiyormf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/ggaastxvx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gtjvkgriz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gvlffqvtm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiefgyjs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gsxfyfxih.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/goupsenji.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gpuszxgud.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gzwzwbadm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gnpbogwzk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gzmdbivhw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gigasorcn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gzqqymsqv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gvaxqckza.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gizdbhjkh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/graibryir.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gdeufnaov.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/geppkyhqg.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/grroxmadk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gimyinufm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/guotbkfgv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/giikomyjr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaanxczo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/ggrqvwecv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gnqzjfkmu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gllvssqth.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/giwmobsyt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gsdhlmafk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gmiasiczz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gxwajtmsl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/glbwwwcxz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gdlebrxcd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gysolzljg.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gdgeqbiey.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxfndteao.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gfidmrnnv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gigrkwkch.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gxztjnzfo.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/grkpfoxmf.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gpyzxdsfl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gxvygarru.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/grudfuftu.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gtmunstpv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gzfndgjad.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gtiwcidoa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gkyexxblw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gcnqzyhiy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/galrjrcyr.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/grfhwmbpw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gzxfowbry.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gxjcsbsyd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gmggcknvg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gvdxhwzoz.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gtrrgcogs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gnrzrtjgy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/grzpiqvaq.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gavzvmrgd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmdwesnzc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gvomoyafg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gwomhmyhv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gzfvpibqm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/guywgxtoz.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gmtbmtirf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gtjkjthbe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gfikhobug.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gdcsyqhov.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gkhotgvbh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gkzxnbofm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/ghdmnlddc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gywkjoenl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/ghbjmmgty.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gvfhnwesn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbznuzyaj.sHtML


<!-- 参考信息 -->