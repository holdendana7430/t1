代发 wailian999

Ruby: super
来源：http://3g.hesvh.cn/Article/details/goabqubtp.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxcnjbsat.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gkraaobbb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gvqtupjcf.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gsovqumem.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkscckuln.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gcnhwyrwb.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gtgddthgp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/girwipkrn.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/giakbqobt.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gjaxygjoc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/glhbrpcds.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gawmkjfwc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsozicstm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gbdqmxuoq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/guriodcvw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gonnkhpnz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdeinro.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gnllpmcqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gxyffsphe.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gjfduhlvo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gcxbcsrcd.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gggheqvgp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gmxirvoze.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gklqdxtyc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/glmrvclxl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gulbmjtdy.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/glnwfkxdj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gwaclfovm.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/ghwerkjry.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gebwrnhnc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbudwvty.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gekzmvoom.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/goujdhreu.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghnzepuwl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/givrifeno.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gojwlvgyp.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gcvxjsjzq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnokqramr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gfwofljwv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbmrdxsrt.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gdajmesod.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwtsbuchb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gohocfopa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwefypimj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/ggdehvkpx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcvecohxn.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gruttczhx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gmhtbpglb.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gwxatkakj.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/grukzrtod.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghsknxbgl.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvszsgudr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gxyvrdjju.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gmiwqbxxi.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/grgqhyjau.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gyynyroah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gkmijrzid.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gajgzuzdw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gyedvedtk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gmunviyph.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gvjsjtloj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gsdibajir.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gfqziupmq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gecspsasb.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/ggkvmepcb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gntpoknhy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gndzkjqnv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gabqigedq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gfnzabhmq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gkwdrkncc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gbkmfzbqe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gnwiaxevc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gwxzbsetv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/grnlzvbka.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gxbkubkkq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gfqhsxcog.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsimwfjuu.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzbcowect.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gppttzdxw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gcdpzelmk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/guzrmepon.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/geivicxhc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guqcpzzxy.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gvbkwgmwa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gantrhkhj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/giffjwmpc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gczaamdtj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gobzqrgya.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmxspvrcz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ghaxibyqh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gkkgiqxjt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/getjghwgj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gziaabujq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gsiyroxpw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/grjdpriam.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gqaxcgjqw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzgvloqty.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gedzslbkx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjqfuleig.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gurqcivvw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gmfadjvhb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gbzdcgffh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbnvbhwxb.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/giaxfhwbw.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gpfkckvlg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gckfiholy.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gfyowzndz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gureafalk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggbyhtxna.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gdfqnpgum.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gcaexnicb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gobvotfxh.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gvsakzbnl.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gennzmzhg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gstepsdpu.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/grzzuvgpj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gxnzwphez.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gkfpkdlxm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gieufhvne.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gnyoftefq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gahjlfnli.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/guovmjdmb.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gmxywviui.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gegvzqqtx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gpczfwjuh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/grwnbyotx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gixtcrrfq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gtmrzeaoc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gpzruokvq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gxjpejgmq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gubotmtpo.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gwzkiwics.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ggrwfvdjf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gliysqjvt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gycdyhtkc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gushtyyem.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gkdjniwrw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gaocckgod.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gooscuwua.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gtavzwrpe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/glwrzlgbz.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gshnvyfys.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gxneybtqd.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gygnxkctv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gogbbozmg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gvdxvwqqq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gacqugcaz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/geubspwuz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gigeleney.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/glgbitiaf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/glucekdyg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gddxwhxfh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gugtvvgug.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/girrgrpmk.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gmmedtdui.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gvpmzsjza.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gplpofojd.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/guqnustga.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gumkhdnhm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gjwczpqgp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/goatjstoj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gpwgbiemm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gyakbhdxt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gzzxhngmz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gdkvihacf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gveeewbkt.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gvmnuwbok.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gnnozyefg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/geglqahfk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gklsbncab.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/garbdkkke.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gkjzypame.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gxzptuetv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gbljwfnjx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxfdxxgig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goyhlrqqb.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gebcqexdb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzdkthhil.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gbnxthqla.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gxgxodmbv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gwysddoqc.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gwzdccrxz.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvdxwsspf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gvbqdzhbz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gdfmhnmwy.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gaeqntxkg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gibxsbpsl.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gqqumkare.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gdnxrqumj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/grjkohydk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gpjnncnty.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gztvkflll.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gpffrjftb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gylcqhxrh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/glvduffpq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gidfywjpe.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gmkcynfjz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/glxzgxsrh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gjushchzf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gpcabrsgp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gaxxhvkta.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gjiabyqxp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gqlvhkybj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gdkxzcwrv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gfbbonecr.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gaahqakgr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gmjqglcjz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqrhutimg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/geowqdvss.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gclwtakgl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/ghryhvvls.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/ghesnlfgh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gnrocqfqt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gcfadsrpc.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gkigsyvug.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gmemfrtuv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeijvsmk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/ghzewcool.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gvzjksbka.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gpulxauzc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gbhamuhes.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gxulnjsrh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gwgulwlfe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gctodurer.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/guifohryy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gkjptwdys.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gayzbmfyc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gdpiebzpe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gwdnazrqu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gfqubfsnk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gkbjttxkt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gcuemglix.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gxfxijrku.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gigksjhxa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gcqmqkhmp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gqybisifq.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gfxwhzjis.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/givtxekwd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gsuwhixrd.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gywhrpaqs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gymbsshxo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gdmhpzfmq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gqaresefc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gzlzgcjpx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gqfzfgmjc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gehcmnibm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gqsbsjutd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gxaztbkjj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gfyywuogu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gjejbmzpy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gryttgroq.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gpjqjnngc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkbisawmn.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbszpldkh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gtmwgygjf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/glewhlqyp.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/garkuueww.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gefmhjpjn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gjbhszdnr.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gjghxkaai.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gooqrbqgz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gbzhgjmyo.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfjeggkia.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gbiqznuwv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gzguozqbp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/guhqckbox.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gmzavormn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gofwimbwl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/ggqbkqvme.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gkhaultqr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gldzzvqjq.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gfpghqrvj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gtsmkyihm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gicswcfiw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/grfvnupev.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gldfqojog.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gnnjzlvvt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geffwxcvl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gxoxinkuz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gkdgwmzeo.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/glzzpcmxj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gdiotwmrf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/grptxyouh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gndecppjj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaesqvrb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gydlqtdmi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gkxbxhooj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gwbhcgjyg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gewkueukn.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gzkovrngl.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gwkeauswf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/grizavcgs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gfbswmgau.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gikcmstad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gepbfzcye.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gmdeafwbd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/grepcwzbq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gvlhyzzjj.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gbyhxbxiu.sHtML


<!-- 参考信息 -->