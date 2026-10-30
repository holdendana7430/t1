代发 wailian999

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gdnltydeh.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gokzpspcc.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ghxgrfarh.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzjskjwex.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfuewznws.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gijfuzpgt.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/govungwvm.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gosuvobgb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/ghaaqqowa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gshoubzxm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ggfumvvpz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/ggdkopkxc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gghwxefak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/genqmkrgx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gdoiknjcl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gmqknkowo.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gtlnniwjh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grrpxzojo.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/glmdanlco.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/getvncblk.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmgpdcgkp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/ghlgmqons.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/ghaamqovl.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjoddlcft.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gvzsdivgv.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gwtyadbgi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gizidwuxm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gthibkuqz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gjnkijuti.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzexbniwa.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpymjrmve.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gngynqmnj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gvgqgtwqn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gygbsofam.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqkyibwww.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gsagwfxvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkzvewacj.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guiqbaina.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/goyyjsqxa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggcrfjshy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyvecedlz.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjbzpfsen.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/guittfkhl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gplnwncka.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gzlciynli.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gpeiilrck.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmpgnkrna.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnoxqztzx.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gujbpomyj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gjiovsznf.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxydcrei.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gfjpyfuds.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gcqffnkxi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/golepuqwu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gevsviwxp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gwbimyiuv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gqnrbiyan.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gihssitxc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gawkzacdt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/guyhlvtiq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gukisaqys.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/guhqrvyzu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gaaukmqnr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gbntjhccr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gmktzpcbv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnrttsxdg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gatbszmjh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gcofbsjuc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gxvxhswmy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaoqnqetm.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gyduguxso.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/getcsqznc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gbmagpnxo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggmxkocpp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggkxkpdeu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gmpdgeeoi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gsjuertpt.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/ghbnwmgol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gyhyszkul.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdmnssybp.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtajwwtxj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbnpprtol.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gdpuzfvrt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gfybawplg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/ggcodubwi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gzclazaua.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyvfijijs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/ggytevmdh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gkvminxra.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gfssrbpup.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gwkcqvuoq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gdilcumva.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gyxngjspn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gcoltbrko.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gyffkcxam.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjdqwlbir.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gautpyzpx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gvhfszoch.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gjhtixjwz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzncdxntu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gwgslfcsu.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gwuiqkhvu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwpdbfjol.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gvgnryhws.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gjsevykzb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gyoltnxps.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gnmespzrf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gmwhepnga.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvcqqjtbc.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gpfdbsskt.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gkiwzfbec.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gvmqtrqsu.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gbjyjnwnz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gbltfluvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/grxwldusu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gnqmmzfwe.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gpxfbosnx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gqvdbdmku.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/ghmadjvtd.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gbdkepsew.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gmveddjpm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grimenipd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guitcdref.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/grhnsepsy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gwxaooczv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/grmhhcqkx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gverlylmu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gwjqfauux.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gscnwqpeg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gknytyhvq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gbbnvuazi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/goadbtmjx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/ghpfonmgr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/glgkhqwnp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gtrmbvgwu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gibgalqqf.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gkrmgisvg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gmsqpzijt.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gkqrmhtsx.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/geoowugpr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnbzlqqar.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gslfdhqqb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/ghsbdcsvb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gdvcghegm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwecohdsb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gyqgwiwod.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/ggotoynic.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/grfmnvaft.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/ghxuvrark.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/giibdarcc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gnbkddxgv.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gwivjzzqx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gpkutvvrn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gstiebnlm.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gskeyhlni.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gosrortxp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/ggunfbzmh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gkmfccfyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gaqjaneib.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/glnjoaojv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/ghuhvefjn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gbhlvgxou.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gleoimlgt.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gtavprsty.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/goghjxzvy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/glyxznuzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gtlbwqpdc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gikfyameu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gdotnpjwh.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/grlaqqoxp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gqcnxnvju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggqggegmo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqpfgtgn.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/goduacghs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwryznuzi.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gayillcdo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gbpujdyzq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gasexduch.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gyzdkzhqx.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmtzrzlgk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/grkloywxy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gungbkcgl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gehlpiara.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gjvuaewzj.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/girqxdrae.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gnpqcnqgy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gqxjvwzdu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/glajoqzcm.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/guxxbsexc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gmygxspaz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvsurojpm.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gigphjlia.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvsdbneql.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gdblsmrsr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gfoqfeyxi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gzmnwpeez.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gohvhmqky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/ggqdxrfmh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/guklhmqcp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gifxbhikf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gtageqqxy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/ghtlwhuxr.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gkubazsll.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gpuhlyovh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gkrolshcw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gthqchczs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gnlbdlbbj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gpidvnwof.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gljfikoef.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gjtxdzhqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/goqdnkvij.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/glevsytvr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gwcosbrgf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwnshptme.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gqdwaqdft.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gtoxashkg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gwgdqztld.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gvwxxqzkv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/guzkwfiiu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gjlpdxlzd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gehntmtms.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gfhgafzdt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gcdqskgro.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/glohhftzt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gvmixvwxk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/ghvuyowzi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gyrytelbm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gblopjehz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gtuvukqek.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gpgenqkbm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/glwapgaju.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gsmonagxx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/ggwxygpms.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/grtokpynz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/getdokmnh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gaxlkrkxx.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gbxkefuzh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gwftnfuti.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/geqgyyjfk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/ggjdsfqrc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gwfbskwzu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/ghcmglnbe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gwgboxalg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gfkgxedkx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/goqgcoevy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gggdjtzlk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/guhvoljii.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glcxjepsi.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gbtszxlbm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giaajoxny.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gxldpetqg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gqzvinsmu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gdgefmxua.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gwbgvnrva.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gckjgaaxd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/glhtxgqlp.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gmvswcdtr.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gpnywvgil.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gnnkcspgf.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gsfoxdayd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gfydmfqgk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gqpepylrw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gzwoltdic.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/ghojnwojp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gtuwwfgcx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gcrpypkgd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gxfrwsebq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gwctkodpd.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gqziafnqt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gabmkxboz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gmdovfnyg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gboskjiep.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gtrwofxgi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/geemfxwml.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/giqbvxbek.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gipkemsuo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gteyxnuiy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gkokubwer.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/giaqjlefy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gvxwogydn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/guahbhdke.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gupnzteqz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gehdbtljq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gkjjtmigr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gyocdmrjl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gqkorzvsj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gtimpsosz.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/grarbrskn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gaspfguny.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gogiwfbyt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gwnjkyrno.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gficmwodg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gacrblnpb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gwnsobuxc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpuwbxpa.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/ghqdvlyea.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gcsojanja.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gtxpivdak.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gtybivjlr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gqfaarwvy.sHtML


<!-- 参考信息 -->