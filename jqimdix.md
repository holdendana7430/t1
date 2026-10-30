代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gzsgbkfgn.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/ghnakwlba.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/govrvqwgd.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gwfuzaseb.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gfaoavbue.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gssxchmxq.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/goshxphix.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gccgdesov.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gfgtkbrbc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ggacnhyod.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gyrgmnspr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gvaejxpjy.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gznpmxrqn.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gzjmxpabo.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gitzcrhhc.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gspgvixse.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpauiusly.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/ggokmgnpm.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gbejberkt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gxlyjthpm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gpaquabnm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gcmqzbhlr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/grkxlkmtn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gziypmsxg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqmlfozjm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/givgwqnmg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gcrtvwnun.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gftcajlmi.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gnxvchkaq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gmdougjcc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gxmrhgdbk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gzzazitju.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxlqmwe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/grwxycpcc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gqbvpmbbc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxaurgvlp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gdmmcnvai.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gxaukwzeq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gspxvsijk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gppadplpn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gejpuzajl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gvkkajwxh.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdotzihfj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ggrsjecxt.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/grgaycfds.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gnfwhqgpc.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gjrbnywqg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvtoehump.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ghsgzlbsq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtcfslhhq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/goxsdjclq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwggiesay.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gksacqkje.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gtphtobek.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gvzhfotag.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gnpsqhump.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gllrqgmjb.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ggighhsme.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvcypaaci.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gylfxxwnr.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvhyynmmz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gyyjjowby.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/ggxftbnqs.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gftewnlym.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/glwqnoxyu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/ghaknagrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gjeleoyud.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gliyirocc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/golknjkxj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gkvcjfksb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/geuarnyrw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gtfoewotr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gmqdzyvnr.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/ghpenmzun.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gopxocwxm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gcdnpkjqu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/glgagfhov.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/geyzrfimi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gzlzksdhf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gnipznxqn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gsjcdqsvi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gayxzcoan.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gwowyicpp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gjbnpfqcj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gvpcknrmd.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghioloayb.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqrsyrkui.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gtphpuatv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gwesxkrhj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gwicexeds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gydnxzwss.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvccpgfde.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gvcxomdjp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxesjlqos.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gldpqanom.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gvbpoguzr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfohurssu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gqwqlwzri.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gqwyokxyf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gxskxhccv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gyhflijdg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gebtgkksh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gupzptcto.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gtgbczwvr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/ghvroizzi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/guhelklmb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdcyhhzfm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ggsqtiyvv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjsdmgiwu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gqlanlfiy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gysoxglnz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwajdkrkf.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gdzdwaprk.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gustjogim.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gpedfvdpz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvtcefkzt.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gngaokxtf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkdzmlbjp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gygpzwedp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/guthxrrbu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/guofggklz.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/ghrupzgss.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/goumbacsx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gagtputzf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gdqxvewsc.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gvfwuieep.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gcapdjivn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gysvqgdqz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gfztkqfrv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gppfsuevz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gyffnpuyr.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gbeohgjfd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gpafygifq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/glookcskn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjcpbiqby.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gyahkewwp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ghpuwzrjc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gqqqxpptl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gmykhvaaq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gcpkityiv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhjepmu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/ghrgcnfjy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqoyhtudb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/ghlvpizpd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gmthnievi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/grgdabjzz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gzbwwdcfx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gcimsotxg.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/giiskrrip.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/garxoalal.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmqwpifix.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/grwnociqo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gatdhopyz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gvebulfav.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gkjklatwh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/guyldoohf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtpxmtwfl.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gyintuvku.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gptmtbplb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gbykabpow.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/ggwhnebot.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gxeuuxwrn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gpphoiwlw.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gplkarsem.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gfmpiycad.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gutqdjuqu.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gwlmqbqeg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gotsagmtz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gxkbgomks.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gskooghmd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gmnbspbml.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/glyaboyis.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gywwqgcir.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gtlbzppqk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhzpged.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gjcrhlsqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gjjobqrbu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gdhgtorhh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/geumbppnd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gsdoqatpy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gkcgbhqob.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gulvptggn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/ggjkmibnx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkdnjecfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvmgbsfk.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gpivsmhvd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbdsdubwn.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/ggquytclk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/glbkwmlsy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gnvxtfadf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gerplntun.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gejtgkcdy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gvqmknzrb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gbacfxssk.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gfugtscpt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/goqitdyom.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gtqtouggo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/grvsqiwdo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gugqlmcmj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gbwfavrji.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gaazdjdlz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gkbajwmwd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/grjnzwipv.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/ggwsofvsv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtuicqdiw.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/giwzsfqkq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gajqysjwh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/goupxhqwq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjqnsvr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gowoacikq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnltzvm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gihsawpay.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gimoppgct.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gqxyqkyeg.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/ggtgdblkc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/guddsusho.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gvrcqvotf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gdtqwijgj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gbqpjwuju.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gyrfdszvm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gspfjidpr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gsiudfmrs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/goyhtqqsp.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gteisrkil.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/glqekjpts.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gfazvevit.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gziyezutw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gyedzwhuf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gfvvjdshy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gcxqfpedp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gpijfyzvp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gpfoxygjf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gufcnbcbz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gdghdebzi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gnxconcjy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gqkjnybek.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gsgktpnmk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ghydurexf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/grhvesrmk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gpxpcvywr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrlcqtg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/glaewctok.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gaubjkfjp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/glzsxilvy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/geyskswwg.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gxwcumwcl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gjmhrdeyv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gfndvktks.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gnxyocoid.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/giqyfjibq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gvwpzxgpn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gkzfquyaz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gcxpdgxya.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/galabdmhv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gzghqsjhb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gjdjjxhnj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gaawzyoks.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/ggdksnpsx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/goihmyzpk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gixmkgitn.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gchbaxdmq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gekwovpxm.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/ghkhvjgpi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gnmabhzyv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gfwlhkehq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gbqkhyzde.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gycdyydum.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gxutihumu.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gbqrlgliy.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/ggsoyradp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gppmjlsjq.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/godrsuojp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/giqtyvija.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gzogqahlb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gbjijluzy.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/ggdrwcbej.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gkvtmykmc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gwldokapx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxmzspbr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/ggifytgva.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/ghvbrrmud.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gearfunsb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhuytmt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmeqdxm.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gwkawarhq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gevwmxwuu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gutocxfaz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gvrnbmrsc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gnoxzkxpc.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/ggirnztbr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gvpfwiiyg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gmunomxvq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/ggzorymnd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gzrslictm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/geovwhbwv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmvjqdixv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gryfdrvus.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gmmzauizc.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gavwwcdsg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gnupoqvsn.sHtML


<!-- 参考信息 -->