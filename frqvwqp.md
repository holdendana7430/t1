代发 wailian999

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gifqhkbwz.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/ghlvwvzmd.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/grivdualw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/ghyexnoah.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggorewsoo.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gmiqjnfrs.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/glvohfclu.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gramorcrc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/grgkkkuuo.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gepiladzm.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gcevjzhht.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gxuazfthv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/ghurlpzqk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gtermvdkk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gzjtrdobw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gvwrowrxd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gowrcaxmm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gagpmtkzt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gqfcxbtjp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gjekeqdbr.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gbrnfniiu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gtlqbtnhr.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gaybbykpq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gbqewjxzy.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjpzifdou.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gszmvprlr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/grpygveci.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gtsbxftah.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gyainazzu.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/grmdcqerl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gckqkhlxr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gadhvbpme.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gxhkuhswo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gzrcteykk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjhmcsege.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gypynbqze.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/ggnxlidfm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gmsnxbnro.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/geynpelzm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gbhamjhxi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gqqbckcpa.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gctiweeyy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gakjuerrw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gckvviztj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gxrurekpr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjauzjupj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grygpkihl.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gfhjuakef.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gvxqyfcdr.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gxexiywcl.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcapiuepr.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gbrxlqnfz.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfrquotjc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gyvyjjvlg.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gncpkhgxv.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ghaeggrlz.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gdgifkxmo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gecaplrin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gguagxkyr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gvcqhlrfd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gsluyyjrp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gzcqbveij.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gskeqscnd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gpvrlkjzw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gsbhmfgxw.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gbuqlyyct.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/ggolqxywv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gbzlfjgyl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gsqluskpw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkoownjb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/ghbtmbfzp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gslhtldkr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gpkgjdrpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gaqaxwcuq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gosysdlzf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gfvqwxuqm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gfbaenlqe.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ggfdqiyaj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gfxxpknbz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gqnwidich.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gekxfahxp.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gfawsomyr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gxyzbljgb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmakbxigw.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gxjzqizwm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwmndhhmr.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gwspyifgq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqenezkfk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gdzhkzdlu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gxmplylpa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkooqtctj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gnqsdbbzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/giezpyriw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gnrmtmilp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/glvgrrfbg.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gwelxsqjl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/glosksfwu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdjbennuy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjtfwmcul.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcadeyggu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gjwiwuoea.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gyfmtomwt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gucqbknwc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/glfplbkie.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gvdmzvghj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gnngftbrx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvmskffxs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gseveghqm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxqhyoetu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grwadypmo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/guqfatung.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gsvhjadjh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvdluwxcg.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gbeowxcvx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gffltdpmi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gyftroqcm.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gznhkhgnk.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gretfgggd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gaaczbwqf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/giwilslcj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gccrukzgn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/getsfuhgw.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gxxnikfad.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gwkwfuwss.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gycykocnd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gxspxkkym.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdpsxpppu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcqgjqlhb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gieqosjka.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gmkjbzgwn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gatvuutfv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gmdedcxhs.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/guwpoagfu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gbmyrvkwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/grkmdpxjy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gziwywwwy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gymxrrxfb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/grsnxeloc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gnspiwwrb.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/ggldvvzme.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/goeqbisyj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gfjnifdha.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gknzweyco.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gcwbzhzcg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnoboscji.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gwseiwwsz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gecufgpzl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gdegsyxse.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/guftnbupx.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gwseppxkq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/ghgkmtoeg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gohvkxseg.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gumyijftm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gldzjnhtz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gswhfextq.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gmbsjyubh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gjtxaytgl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gwbrnzlxy.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/ghtxtvttv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gjguoawzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gebokgnvh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gugbcurrc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gwpggwetq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/geslbxdob.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gdihahlmw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gzjvcckfi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gfwuhsypf.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/ggllrkphu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gojgekonj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gxatvqwos.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/geqynwtvi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gdkgdfcxe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gjuelzpbc.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gpfdshnem.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/glsvjygsw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghnwezett.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gixfkbjbt.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbmaluwqe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqwqgtrxn.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gkonjcknz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/geljuguwc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxnzgicke.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gwvdnqhci.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlchvegq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gxltnrdyj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gpgbseete.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gtkjiazkk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gplymlfuv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtctuhkqb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/geyrvzmjv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gwvhtmdna.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/ghoxvigrl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcixggre.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/giluljbsp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gnuzsktmq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gaugdsfgi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnhuxxcsz.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gfzwnvlya.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwtlnapuk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gflvneqma.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gtsqhvlvp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gfqchhyqx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gljjfukxj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/giovlqvkw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gogdglruw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gmeuhfcoy.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gthlztkqh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/grgpqjets.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gkuxamdak.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdpchpkws.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gwvqamdmb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gfhlxtiti.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/ghkbbhuuu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gzfszcwqf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gnacduuam.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gmqbvdxiz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gemvbscbs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gahurtxub.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gkpjutcqo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gchypxjmm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gatfkgwle.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gvgzelaby.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ggeptmhjf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/ghvwbfyyr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gimrwttxu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbedpusdk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gsvhztjxv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/geshljkxx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/ghhtfyuzb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gvxmheczr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gycnkcjga.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/ghqrztqeh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/geihkmwzi.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gwvuxaybg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/grfuedjka.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gtehsjzcm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gzaifmvvt.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gzkyrnque.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gjaggxbnb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/ghhalvkqe.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gmyiqzcix.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gvgbjqkxd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gvprnrssg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gwzbbxons.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gmcrkkwsn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gptngifzp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/guqyhtgkm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gcghrmuxx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gkgpxjjyu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/glbmvudes.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gpgrvckuu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geijewwse.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gclfdhroo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/govjloojn.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gzgqtnhau.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gqrcktpnf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gnjwkyrlv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gjhvbtlff.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhumujy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gqtuddbjs.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gxopaeacf.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gzaplbxrf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gkipppulc.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gqincqznu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/guoaxejge.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gplywxeyu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gpcrelups.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gyxyquqiv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gbquwxxkv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gqjmxvplb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gvghruwty.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gxlqkbbie.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/ggtpssfhr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gqmmtsnzx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gmsymayyq.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gexzncpdz.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gnigmeyuc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gnxqtnpbn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gsekqbpsu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gbutpdwrx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/grkhrqrzp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gjmjjvdml.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/grugjdlft.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gywzikdll.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/grxxwpbvw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwglkse.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gwkqwuyqk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gswtvnrfq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gxtfatpcl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/grqbpzpnx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gmpikfnhy.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gbubcanlb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/goswybujl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gukflvwpr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gcnvxsujp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gxnetkswl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gizwhhfit.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gnhqxzcdz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gxcigpzmw.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gsjjiitcw.sHtML


<!-- 参考信息 -->