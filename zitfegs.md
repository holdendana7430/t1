代发 wailian999

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/giqnavooz.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/grrmlntbm.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzfhjdulo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gafwmrizv.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gppzgzpti.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gkvomaynv.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gzmctobyu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gssmnnhrk.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gbemxinxr.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gvdpzfmgj.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gmizpxrgd.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfygxxabp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gadjutvtz.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gijvqtlel.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/glruhqnrc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gnomrpohb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gfpnplzpa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/geexsyqsk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gasepaxio.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gqrkpnhwp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gvmujmxlw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gphunjcwf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gggifswed.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gkptobuff.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/grqxxodlr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gccloyzok.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjtdyhpch.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gszrdjzhg.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gneajfmzb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gymdkjkqz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/giuwywflu.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmwqqqjzr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gjcnvkyzv.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gozvomipi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/genhxytok.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjbbbbhdg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gelwnmero.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/giasnbdea.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/givtjjhcg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gfqpigttk.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gwcfvvjct.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gbzogizue.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvgnqvejt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gyhqlfwfb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gjtttdbdr.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmadjsups.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/geatsrgbv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gsoddufxb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gepmwerdc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gqtjmzyyq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gnblizapm.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gmvnbiyfs.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/glnrngqvc.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gncwthtpf.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxsdvagsd.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwntkevcj.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gulyqkzoy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gjdyitvbz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gqmsvnbnf.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/godecarng.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gmirnnida.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gfewqvvwu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/glgozgqok.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gewuzmcwt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gnycefsru.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gvdqjgoqr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gcgbcmuvh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/guixdmfzh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ghaibnvfv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gntvkoent.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gkmweroee.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gpfvmkuzk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gkxzhhsac.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gucxsvodv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gzjqssvng.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gdababfdr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gnpgassmi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gctghscop.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gbnyynpef.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ggwfkihty.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/grrqpmhga.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gdmteqdeh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gkoxypjls.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gveqqdiss.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gdvpzadfq.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gfpitixzs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gtbxmsppq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gojuhenlg.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/giwinmikw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybvmqqvc.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gxycuminn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gwjmwctyp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gnltotdzj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gdnmzgypg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gkyglsvuv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gktixgnut.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/grobvrfls.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gjculgmve.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gaykcssuq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gizeucbso.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gepiypusu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gihmipvlk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/getxylenb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ggedmgbir.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkqycisfh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gkjxkthrq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/goolnnjzw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gwnhdognt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gusafoscp.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gdcgqmpeo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/glhswlqrm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtvbcpkuy.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gthdlpbgk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gklqrhcxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gzzqlkwsi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjyhyened.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwmyobcrh.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gutmpamla.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gckqlcynm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gnuhuwqzb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gyivwxktl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gltqbrews.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcnvyrcuf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxgqyul.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/ghlffphck.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gphuiknbl.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gounpecus.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gfhvzsfnu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gaxvzagqe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ggulctvpr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gauwlesqd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/grhkeijmp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/glbjypmjn.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/ghihpdqrk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gbciklqtm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/goyriiwrn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/goyszwhlj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gvknpggqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gkraodlgv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gpcnyvnaz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gsauooyhp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/ghzctyjmm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gzvbvmrsj.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gflkxlmxc.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gezfrsxca.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gkuhmgazw.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gjtczqnrd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gsvbbwxwk.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtegxesig.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gugxrwmfw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gilhdzcvx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gptlqpuiw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqnfkfvpl.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gxxuohbli.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gudgrlwad.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gjisxnqyp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/goirksgfp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gqnqbstum.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gmobtcqhi.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gnsnjpcde.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gobczkvaj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gyqsedgqh.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gynofoqug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/ghrswudlw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gqooisbjs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gfxenlslb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gwnpqgidj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gqcqjrepm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gmzmspzux.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gtqkpiktn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/goqvcgwid.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gedzcjoqf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gklxwcdak.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gmgjdkrcz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gxfowxfyh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/ghzqpcvsx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gauldgvdw.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/graqanggj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gdegkojdk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxtejuakn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpevkmqry.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/ggtctkmmi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giqhziaff.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gvvjjtmao.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gkukvhppp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmumweghq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gyyqucejl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gqyhmycxp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/grapgdzqv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gsedfppbp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/ggbouugeb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gsprpatry.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gqzolklin.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gnwxvzpug.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gqbpfmtiy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gutwqwcul.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gvzofgezd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/goizvdtlq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gcznvixgn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gzifikusl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzpwiafel.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gccjyffwv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gzdxyfejx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gzcwagejd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/glaraaeoh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gdnzuuaxe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gxrbkjuum.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/glljufjzu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/giygybaus.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gewwbjqdf.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/genvdtteb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gnwwrthnd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/giucxebal.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gvipmdcsh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/guvkmsrsc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gtviguaim.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/grvogyuhz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/guqdhhvwz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gtlcauyyn.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gzyezqsum.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gfsnkonem.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gyzvluuus.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdxphhbxd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/goygoexcg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gpnzxnxwv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/ggaewbbxh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gxrwwzbwk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gwythoziz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gkikzmbzx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ggekztkfw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gykvkmjmk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gexqpwqof.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/ggmktiuwy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gijeavfjp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gfvrbyxpq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gjjtawbej.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gcmeuoepa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gwafmpzpt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gagrmojme.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gamhydhwk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gggrwryei.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gbmvoqsit.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/grgllaufj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gocpongft.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gdlvmubkw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gboloiklw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gmtxilzww.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gnqwcrhxa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gooqaavum.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gjyuyypqs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gxwztiksv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gyrstzihz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gqvxieztv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gecymdxuq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gmedetvtu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gamhrwolm.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gcfjkxjgn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guedbfyou.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gsxuiiuhi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gvompueqq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gixstdjkt.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/galjiphuy.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gjhsazadr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gitrdcslp.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gekvmhgzm.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gckvndjov.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/grdermobw.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/giwcthipp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gbqbfjgcr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gexeuvgds.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gjsvenpro.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gcasjafkr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gklbkdnqd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/glmtsaayw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gsochbgbv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gjimpfwcd.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gmhhbwsnj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gnfuautea.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gdicqyais.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/guykhakjs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gxerdkmqg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gkxjuvsud.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gzouevqqy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gncqrzcpp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeqcntto.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gmnhrqsdd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/guyviomny.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/gmvlyncpa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gbsofyykf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gstzttacg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gnxuoerna.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gswlkgrtx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gkpzbjgps.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gebvcilpq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gikcwlwue.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/ghklwvzar.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gohiwylaf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gbiuqdzck.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/giyaiqwmt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gtkmacssv.sHtML


<!-- 参考信息 -->