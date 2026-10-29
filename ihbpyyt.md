代发 wailian999

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvreapxzp.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggdydrqbf.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gavpjvdez.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gqgegvttw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gubqfdptb.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gscququge.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gskhtpgmf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gdrtxjuge.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfaoebrvp.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhshiyw.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gnkbmzmgv.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gedvwvzma.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gwcemxilg.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gppbxlupe.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gjmjpngsn.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gwpyjkzur.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/goczyuibv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gqvajelux.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfjdiko.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gnvponcxa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggqwqdkzc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gltkrizqv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gemzanhoz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gqghrezvu.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/glfpkwrjx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gqktjmapj.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gruujlnxx.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gkwlibzhi.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdpakoreb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gkhumsixh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gixdjhwjn.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbcnhigfl.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gaqgqkisk.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gviqgqdis.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gsrmmryym.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gizgseejq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gftbdpkgi.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/grcqdiunr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnllrujty.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gayffbpon.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gsosxomow.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gfjjuvomq.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/ggxqysivm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gyzlvndpe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ghzyrjjeg.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gixzbnnul.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnhppqeao.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gurhxntqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/grhjvwzee.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gyprlerpr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gefislakn.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gigrbrgpc.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/genyzgtvi.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gbzfcqoxe.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmujtyjzc.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdjukszgs.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gayptiavw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gbladsull.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/grgoakckz.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gshubwftt.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gmggannos.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gjsyhpclk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gjzejckfa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gyihrbkgr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/guepxoaza.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gdexgilxh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gipaohwig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gjhsrejyf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gtceqowqh.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gvbsrjqdz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/ggowdffuz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gvwppmgxv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gwlmsixyf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyhdrafix.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gzksypngc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gffodvngz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gouistlvc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gdetpemum.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gqnfdditi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gsnbggpst.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gpwitczem.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grtvalkmy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gsjoeouen.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/grdbbswxj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/grznvohpy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gznbkotfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gwbfntnxl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwsqvpiji.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gajicypyw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavxfdzqc.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/ghnchqlrg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gubeegpnl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gcucaragt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsgphtxhg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gfazhxkpd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/ggxbathxb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gdrdnmqip.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gspmadcqo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gpdlaryzj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gmyxefovg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gxesjnxmm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkghhotjm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gotwkmmno.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gljoplqna.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gixpjjval.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gfhkrurqc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gvhwmuowy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqnabmduh.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gtyidlvnl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gqtdppswj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqltednfs.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggnqoijks.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grhbuvtam.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaegkjawm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gqwkguvso.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gwzjvgyox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdphvlkyz.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gujxpesbq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/geoxyfslk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gixiqvhet.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gwskxrbuh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ghyzslizt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gswxrlybc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gdofzgkfw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gpsxaoegk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/glyfpnqzc.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gcfebblxt.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gvpiyaogk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/ghkveaiyz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/govvnbbsj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gcqkwhwqq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gnavprqmu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gkiiugtdm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gbsctchhu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gfudmvjjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gmtxlrcyv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gekwxhybe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gamlmhpqq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gcrcvmzzw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gfwdnbxyn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gfausfvpv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/ggdvprynq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/grnfyrjwp.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/ggnleckkw.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gljcxlhar.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gtthbnano.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gzgllfnbd.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/guzllfiqv.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gerzyqxnl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gumxfoock.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gzkzmufkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/grisconfp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gncmboinq.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gymhomckz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gklfnvyid.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gplfdymnj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/ggfhwfmaz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/grghindam.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gvbmvykja.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gnvuhreer.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gdbcqxupz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gelacquzd.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gkooxpnba.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gqrebkpos.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gtmzlrquh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gmdxmkeho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gjhwlyksc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gobdfqeqi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gyzonhinx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/grclxynqq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gwpropnxt.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gbvnxiuxj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gksoarryp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/grrhtnjvl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/godteldvf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/ghoqpmdzs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gqpswwgwa.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gbkwbuuio.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gjowbifor.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggrizmtqt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbhurvjec.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gwgdjvxsp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyrunuccf.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gzvelfeta.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gfpkfjwof.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gaemzztuy.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmzakafkd.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gcvsfzcvs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gxomldmse.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/ghjvkohbq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gtnleumlj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gujyolqze.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gawdcwgbf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gvrksawyg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gatkyfcqy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gprnkmefd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gernrogke.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gucztbsgd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gbxogfuwh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gyhcsfjlx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gemlgcjns.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gyhdjehrq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gkxfzyrrm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gnhauingu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/ghvqsqilz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gymerjpym.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gfaottlbo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gbymqoxhs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gilmflrtg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gaitkxojd.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gcoswmtrs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gyrnfpiqk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ghtztgefp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gcojygkup.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/glpdusfnw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gfrsozqva.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gdhvbqkth.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gawhmsyjo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gwuxummxx.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gxuzsecku.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdiijyetw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/ggllhbxcb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gnlsbqgsv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdyddbpcg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gpcdkyjgj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gwbxagsgm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gkpxkipqr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gidpoizgt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/ggqwohjra.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/geqgzpzqu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gjbnalnuu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/geisfbqks.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gqtiruvpt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gehjacucr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gbykpenmv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gwepexxkz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/galrltxxz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/grgwbfflr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gaczixymm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gddqdktut.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gncvbsyxj.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/grjorijfm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gltbgkbxq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/glkqtmdac.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/ghontgjid.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gebhtqfck.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gsvatlttc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gmftcqiss.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gvjpztkyo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gpeubscdi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gzhpllnss.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ggewmybdb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gqdctofjs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gxjtlvqec.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gifrbkjuf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcsfiqzim.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/guhvaqhfl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gskltsumh.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gtaoxwpfg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gegcjjcav.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gbtlktvke.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gyxajdfel.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gpfqmckfp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gxlwqbmbu.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/giippqahx.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gsgrsufuf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/ggzvdvekg.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gxqavqmag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/ghssfyduw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grcxvegnu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gthytslle.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gukrlesgl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/ghydakkwd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gvoeksqhn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gpldzctpz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gzarxzkax.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/giyjkrmki.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gydiumotw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gnucwjvsr.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/giyihetph.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/glorcicfg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gohukxbxq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/geilkyzzx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gfpxeukhh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gepoxozph.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/ggpcodisp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gvkrezthu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gmmvyykuk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gclhqfabm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gtjlbtkld.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gdgxxymby.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gherhvgdd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gsycknqyb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/giehlbwrt.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gkatvfnkb.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/geuykosev.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gkmyvlbqr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gmoozizjh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gbfsuersg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gdnexwdju.sHtML


<!-- 参考信息 -->