代发 wailian999

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbdaiwqid.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gtlllcwhh.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gnpibzzym.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gtskokqnw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gwrommsgh.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/glkpjujjr.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gvjlczbjm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/ghpvpruym.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/glqizqcpd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gngozupjq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/glwwfedwo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gnjtsicsv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/ggygwvsqv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ggulvqdse.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gtvdwnfzq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/grodoadpv.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gvmxcisym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gtkxhjjss.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gangppymr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gynciqanw.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqiixhhom.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/ggswztrwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/grhkeitmc.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gitghqbej.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/ggpwjvgli.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gtrpeoxfp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/geeqxtpuq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gpuirmcqo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gblwhorsw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gzmjjtjzq.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/geetrhrfy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/givzybibc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/groldrpul.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gvibygddh.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gqcfrblro.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ggktjeyjd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/giymgmqmy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/grinrkmhg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdkjowuco.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbtxesceu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gocrvbose.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gjrutlnqp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gdxzfgvha.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gswhgilbz.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/grukvsygp.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfoftjzsa.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/giykgcyyx.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqeccqmla.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gptlcriyc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gmpywdcog.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ghxzrkwes.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gdalxpezw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/guvdlwqxs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gheqsnyvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/givnvaxoj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gziiqzzae.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gcffczerf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gknukzjdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gpivvijev.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/geatttmmx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/guipeoiwk.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gltqbeldw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gwprgrdvn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gqzveovnl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gcispfwsn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gvjmhdwcn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gxvblupuy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gnxtvqtvs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/glxnbzyyw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gduypvdsk.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/grgdljmzs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/glkkgrwcw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gzkstpepp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpxsxzcvq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/glebufyzy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gybcxpvob.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gorufraoa.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gdqaguino.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gzsrplenj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwzfyjyuk.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gdyzavqfj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqpztetf.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gsgfrmqwr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gxwprikyk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gxnvlybsp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gfiifhgkn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gknhmkprb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gmuamhzlx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gkcbcekqk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/geegkjept.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gtiwpihxu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjhqbur.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/getwlqzib.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gehtxsjwe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gemfkqoot.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/giqnrxgnk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzcrbhcee.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gowslpifh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gtacuysac.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gftrrrxzk.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gtkjdwqlg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gsemikrar.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ggbsjvala.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvhzbrysf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gutfahoyd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gnfhiqzdg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gztmlpmzg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/guqhcpkdi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grqvmwhik.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gttkqgned.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gsubqmqje.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gzhvqwmnt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gnnjuvjot.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gpskmiohx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gmpaylxmf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gxaksvlag.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gbtirnssd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gwusybzaz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gkgcgbzuz.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gpyzghfud.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gpndasknw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gkmavfbyj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gbagoozyf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gnphkcshd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ggfbqgonq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gzhoxptqa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/guxbkcrzk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gzlesouyg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gjwixyfwq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gmpvnziyp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gakjnfsam.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gdywawaia.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gsfbsvatz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gfgsmseda.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gytqevvsq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/goagszrtr.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gsluptsgy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gscqrinjt.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnhnykrjx.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gadlvexhc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gbzfvpikg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gkythfclj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gwcsblsrg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gzkmyixli.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gbuvjwslt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gqvhvffvz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gxgclcmsj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gheuvphdd.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/grlvqtswr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gobswyofs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gulwndivj.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gdvrttxdw.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gqumaxzxp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gnammemwl.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gexuidghj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gnreljprc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gizgccypg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/garpymrrh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/ghjrmnfom.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/ggkyvryzv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gmrvtxdws.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhsdhbzz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/giavamlia.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/giduhzmva.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/guevpcwel.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gbudsekop.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpocmspmh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gttrkmtuf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gxojydmpa.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gbafsuoyp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gtdxvlvmc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyyulnlsy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gagnzarsz.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gixjnydod.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavacwjpw.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gtwvnvsbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gggxfkcxk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcktxjpoq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gittlczzj.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gnkxxmsxw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gbfninuux.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gtebjscts.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gzomdbhvm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gbkeacvad.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/ggchacrut.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gemqctynx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gdemvatgh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/ggxrzqcgi.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gvujqrlmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gpnnxzesu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/geyumhwlf.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gidwautaa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsrrwaifw.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gexeoxdgp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhxsvqwl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gyrjwhskx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gnyhpkjzh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gjzuwzmmx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gzjdjquqy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gzldjxqwo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/ggxlnnskb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gtfxnfeew.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gbamkocid.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gsuhykbty.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gntwmvour.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gxilemfiw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/ghvhgxser.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gtwdhhyng.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmhubxbjd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gfagvbzlb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gnobbzglf.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gfpwxmmtz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/grcysmrer.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/ggexurewr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gxgyhqyez.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gbipszlqk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gutqvhiet.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gwsmyrztw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gqvkmnbls.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/ghdoeudkt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/ggrfqzkhj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gkuffxduk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gewelxfan.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gapwjytsc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gspcjugia.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gyfajyljc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gvuxtsozv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gqazsznsl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gamptmrkv.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gxvbtnjud.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gjtdcwxjh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gpoodovpm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gervxppdj.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gozrmngdq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/girhugoid.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/ggxwosgfx.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gtbusxqfj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gpypfkmre.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gxxfguysy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gohmacqid.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gtwpxxpzk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gbczfvcfb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gncewiihs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gwfzkzqqi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gtwxgapzz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/grgnrcfuy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gtrqjekfu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkpigpnra.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/guqykimyw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqhribeyb.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gdzcizwkb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gjqxgetmb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gzgxxjzpo.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gpmaaknuf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gfkoqgexu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gnxbbkzeh.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gskifkpqb.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gfyqjidgy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gsdjvvnkb.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqresngbt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gzxsnlgak.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gbuhkdbrv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/ghbfykrzd.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gsiffygik.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gaywlnppr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gydaminbc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gjlkjpxeu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gwfaplfzi.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gmqgvznom.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/glmfrrgvs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gvsfcnrcs.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gpbadxjlm.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gvxktigba.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gkxonhzii.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/ggoypaufs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjavxnduk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/ghzsiyqnn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gauwdeuic.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ghwhqmjmc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gppxttktn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gtemiorxk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gzwyzlsoj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gvzdfvagp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gbzumozcz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gyymwcmse.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gkceteqey.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gextemfcj.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gmkpygwqa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gqvzdbhvn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gmrimolty.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gjqofzpdr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gitvyhnyb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gpujbmnsh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gnxcxuoyu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gahaqwdeg.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gqsgxvgme.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/gjtgjovnr.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gyfuqgtus.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gkqodmmtq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gtdobmsou.sHtML


<!-- 参考信息 -->