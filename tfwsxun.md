代发 wailian999

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ggcxhbnip.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gkhjbkyye.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gsmxgbxss.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ghzcxemal.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gwvnogupr.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gfahlojoi.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gfeddvqqh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gygqpqtec.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gaipfoimd.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gmavsyhcp.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gnprwmsfg.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpydhflov.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gekzhxjii.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gqkwhuftn.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/glitdlino.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gmgycjnpm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gnjnmwmyz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/glkdhdwli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gictspkrw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gjhhawjhh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gnizkcekk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gpcipzkhi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/ghxgjmvrs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gtjmzwwkn.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gvbfxoijn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/grljjtpmr.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzshcyucb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gibqktdeb.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsgdyuhny.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/grxwmsorg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gqsaewdiw.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggojlnwru.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gbmbmuxdh.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gnjogghdv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gswcyzacj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gysiwbezh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gidrjeenb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ghqovmtys.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/ghjpcpqww.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/grbxrcpys.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gnnxllbkj.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gjajbxdck.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjhtqxawg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/ghzgsnted.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/guypmbdtj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guaqpfefa.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggecfwwms.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gquigzvqc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glvdtbhau.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gswieyyut.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gyanxcwkv.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gstcilzxq.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gzpyllzel.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gkwmmwuly.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtptxrrfc.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxvkwscwr.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/guhmhotqs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gdanhwybm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/giiydopbm.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gcjnmwozk.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ghtjnanxs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/guibjenzo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmcakokxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/guspbyjku.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gjjwcdbae.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gqpvbpuio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gbqtethjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gbnrnrqul.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gxfmhyzps.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gsxxshhrw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gqqusslrs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gwdqypoeh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gkpspmfvs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gcoaycdtm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxmmxpws.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gigvmyuyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/guqoijret.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqonijs.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gezqiapbl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gcsrhrlns.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gnxyxehvy.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gimpwnoxt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzceijfon.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/ggwgrvzvp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gmkprddqg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gtuipsomj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gmbjhjgsr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvqktnyf.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ghnpfakhb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gknvdgnti.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/ggnqstggu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gwgxpxsnh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/geihbgyus.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gnzlkfadw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gikovwasq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gfisooqrh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gwhhyqlhl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/giwuzzlsp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gxtvortuk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gaoasppfi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/ggcnsvzhy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gusacqoxe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/goydewqgz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gcgccvlsg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gooefqdyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/ghfxuquws.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gvbhmsdkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gmufxeeak.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gycnzdlsi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gjdiwtbur.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gzyhnvaqp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gpupknfoy.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gkhsgzraa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkdsvqr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gbsfbwtcw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gmjcrqxxf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gfpthztcq.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gmntmflmp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gilyecdai.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gtyfqqdrm.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjsneugu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/glheeswua.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gzvfksfix.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/goclghfxg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/ghsisbjdj.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gowfymaxb.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gbzbzilcw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvhepxj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjypwnwit.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gvabnrqmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/giiwngamn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/geuwfiyxv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gbaufocqd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gxwqzberr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gggchcscq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gtjrujjmc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gbdirthfi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gvzzxmlbx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gwiimkghs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gfqaiqsov.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/grvozjfwn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gpshybcjv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gozfgcwjt.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gqsfggwic.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gblfhcxxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdepmwb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gubfqlsqi.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gtrqqjpng.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gskpqpbga.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gcjmhdxvb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gbjmojnqi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gynfctzxc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/goylvwibl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gtnmzcesp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gaobnrdqv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gfjedoiqj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gaoiyqjpe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gztghatyx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gahieefri.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gtecmkrur.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/ghlxhwvtv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gjjdnvdmy.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/grtppmjey.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gsccpcbka.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gtrsbsrgr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gxuzcxidf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/grisjaakw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gihezanpy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gszqjoqbl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gzaafzaot.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gwcqqkfln.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/ghhazsvux.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gchgukftl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/grhbcdrhg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gkcumkaoo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/goaqfnmsy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gokqzcsqv.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gsgyjrniw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gcfpxdlav.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfhdduugg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpaitdyed.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnmjxmfua.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glttnlwjh.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gpacryewb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gpzcsaxyh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnxqhjexq.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gelqlnetf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gybrtsxin.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gkivotppy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gouxeniwo.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gvdwxyqxh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ggtnnnifb.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/grgvhzyny.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/ghlpgfhjo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gnlaeipvc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gviwslwpi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gumhanyns.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gphjneqcb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/grdxynugb.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gipbwyglp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmthcdrwj.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gqvuscvpn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gampcnuzz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gzerzgegi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gzhzbqczz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gaorryhfq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/giritylof.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/grttlwehm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gvpmbbkbr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gdamxadqh.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gkeafjoha.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gfcwbkghc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gbgfrqlur.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/guvuznhvl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gvxlcsjrm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gouqohhhs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gahityhit.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gpblmkueu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gnjjwhejl.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gmarhfutk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gyejuvkom.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxzshdwkl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gwkquyibc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/ghuecvyfo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gyehzukvs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gavjywdvo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gsxvywcwe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/glqiypdht.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gzktxzzye.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/girxijuha.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gyikmdksx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gfbdlcjgy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gkheslkbk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gcodfkgsm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gyoclnlvv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/giaiiekks.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gzbyqebel.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/geojqngqh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gljnonoxv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/guzioutnd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gncxmytid.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gryrtlske.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gfbgrxcuc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gwazltcig.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxacomad.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gpnatocgm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gemubwrdj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gepyrstsf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gzggwvgab.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gnbldjdrk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gwgjcxwcp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/goywyqbsd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/giykjbnsa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/grvnzlhts.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gkrmhdduy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqticibp.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/ggomgiktk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghnahrmor.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gmuqkswfc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gqisqngyg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gwucixgzv.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gmhhugivl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/goqpjlhlh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gmqmsescw.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gprgiyuus.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gxgrvyuhi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gwezuwfbc.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxlcjisyl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gfkubxpko.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gntafiyzn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gyhuqhybi.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gshxfzpog.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gtiudjnab.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gvkyqovhw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gesxwritl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gruuhcwhx.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gywnndqce.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gimqeicqa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gsancremr.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gsrwekhsw.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gcjbmxdmk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gohntcwnj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gfwcrqtjl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvzcpzek.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/grnkxrznb.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gbeujzscl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gzgpuquwk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gasqpdjne.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gtszpoqcv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gvuvrelva.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gwpgboqpg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gwzrgfycx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gvfgnthby.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gofoahneo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gklagpmcx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gztqiybcp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gbszfjazf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gpnxxmqcg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gzhybpjoc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/goifjoqtf.sHtML


<!-- 参考信息 -->