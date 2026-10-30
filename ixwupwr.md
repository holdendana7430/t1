代发 wailian999

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/glbnxfwsw.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfcncoi.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/ghxbadlas.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gzazuguax.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggdczotik.sHtML

JS:   static f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkczfjdsd.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvacnoupf.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggspdjcdh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gpxuypwen.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gnunoedvb.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geltvgcoh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuxiriau.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gujcfwxpv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/gstxjikug.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gfzcfzqqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gedfonpqa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezpikbxy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzicvvogl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdsjukal.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gncvkggur.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/glbmpnztz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/glqajbajo.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/genfubxzy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrhuyqqb.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxiwqarv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gzhssexel.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/ghifpmoiu.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gcwwksrje.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgbvignz.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gamhxpjap.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gifjbuhgo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gktqlpxgt.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggepxkmqn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gelqauqro.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqqfrben.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gkfzxbmoi.sHtML

Ruby: attr_accessor :name
来源：http://3g.fanxiaobao.xyz/Article/details/gwiwcamxj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihoxwcfy.sHtML

[G12] 对象转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gozludfgq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/glvkybwvi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvojgetb.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxahbzb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczqkkxuo.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gowtapmfa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gucveozds.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gvfdzries.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gseyykkph.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gradzayeb.sHtML

Py:   isinstance(u, User)
来源：http://3g.fanxiaobao.xyz/Article/details/gwaykjqeh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnetgfnvj.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvgvtnwv.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzddxsdvs.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgbzudy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gosqonmvn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/gwysxnsbd.sHtML

C#:   u is User
来源：http://www.share.fanxiaobao.xyz/Article/details/grzcxxegn.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpymjlir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/gvgrvjisr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxoxasf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gbkrogqvd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/glvywxvtz.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrntfpfy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/geatiwfed.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gmrqyomea.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmtouzzc.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmblqauj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtameuner.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgqvdrs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fanxiaobao.xyz/Article/details/grqcpeqge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiclxshl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/gpbeaggdx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gflqifcog.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnriqhgqx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcmyhody.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlskmfwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwczzepre.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gczqtgqgr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxelzcjnd.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gesnwlvqy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjdksfq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gsizqkbad.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gicngdfku.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gvgepqasd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gepsufxqe.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzfxwvjoo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvskygeyk.sHtML

[H01] try / catch 基础
来源：http://wap.fanxiaobao.xyz/Article/details/ghwameqky.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gparlpdog.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhachjyz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlnefxuo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdmunnyl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxzcotgh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwmlnnno.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gqnthzjwb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucbecoy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtjqmakz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/gzuzxypor.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpsjgnnd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjbspfze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godakqiai.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggispibqs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fanxiaobao.xyz/Article/details/gfqbxpoyr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggccmdnvn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnlcxbzm.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gdqzlvgbp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/gheiuxpkq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gltrmvidr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazvwtrc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjcxkcpw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghygyarvs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fanxiaobao.xyz/Article/details/gvoceivtv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/grsqkzunw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gojffuxkl.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdiavqto.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntstvhem.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgazhvv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/glzjsuvgq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/grrtqgkef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonxsbiu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmfxtjdc.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/guswxhhko.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gudlcndbg.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gshjmlotw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrozgzyf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvxtoox.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvqikhkqc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gckewrgmv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjimajvp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsixenszc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqigsujo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/givizumkd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpijzlgf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzslsvfs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/giqtlpnxu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkoqntgc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gaonfmpaj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthkquij.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmixoifp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdixxdftq.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjsnyzx.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoybsrkg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdmmshw.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gmsubdgth.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gudkqpptt.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsyuxmzg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbqsvntq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhhssdz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwgtvjex.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemrlmyne.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/grxjfwkvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhvlgwtm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsghzgdtm.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfwgzvoq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gfygtbimw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/grfqhyled.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gucqpyyqk.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fanxiaobao.xyz/Article/details/gugqvxlgr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/gnjlrdjhs.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnvgbixn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmcuuukm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdnlbsi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazosgek.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziswdkhk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyppacwos.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gosfddbek.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggidcdksb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvutgatr.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhvxshvv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjgnvss.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/ghgywdzwc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gbxoegmso.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfkhyail.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gzfqqvajm.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgzfcen.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginounztb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngknbkvd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnclzcnlv.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjtcrqvek.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjktikoke.sHtML

[I01] 判断是否匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gblgdkzyj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/goenhotxa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gsppnexvf.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmiqupey.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwjccoaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/gqplpcjgk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvnyrsev.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gachjmkxd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdnvmujk.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gvpwpbdjx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gygepcivv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/glvzuwevv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsjvzfbj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnjebuth.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gkbotgwpi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcbvsoxv.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gxpskoqvo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjirtfa.sHtML

[I03] 提取捕获分组
来源：http://read.share.fanxiaobao.xyz/Article/details/grmgtmqyc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gprawnlhi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmebjmzwu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gwsprswcg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmrhdtvl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkctmbfn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gpahdfuip.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gunkztpyz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoslxnaa.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmydmpicn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gokfvidmi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklngvhwx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmhqvsr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gersmncss.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzywduerj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gwxglucfv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgtacgvk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvgfojts.sHtML

[I05] 按正则拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gpilfezuh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgnizlou.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdopvjr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvlhzwu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxnswgoy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvyqqhb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gownrndro.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gmoapvtxa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzxffozu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmaudhal.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgvimnfy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgwnksbb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhywitxa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gqmhyywam.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giapbrzvf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gxilzefef.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcehfweg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpapxssz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdzezsjr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbnvmsf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcauedwo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/gqmprkqnw.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwefjrcp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcjpmgmh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/ginzlllvc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnrcnmvf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fanxiaobao.xyz/Article/details/gxqzphzwb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjihmpgw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gvipyivxt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/glmyfvrdk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gwdvvcaiz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomvjvaym.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmksyrbdx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/glngrhwmv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfxgyqbp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gqpmrxwkx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyromiwyp.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gsmseybfw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyvlqctn.sHtML

[J01] 获取当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqfsswu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fanxiaobao.xyz/Article/details/gaplzwrdp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzhecllm.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gqhfaanad.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkdqlbat.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyqnjmzr.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gcsqdravz.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqhsklh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbnzmqrw.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgsubgtj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdtsudhb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjixseph.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fanxiaobao.xyz/Article/details/gcwuuichv.sHtML

TS:   d.toISOString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguoczlhx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fanxiaobao.xyz/Article/details/gqjmbvtkp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gymdcolwb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsnbiepm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaescsttd.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gimoppguj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmfemxgy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjegnemfv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gnuiqddic.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksrvsygy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/grnhtmlpq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmprgqolg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gleuguxuy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fanxiaobao.xyz/Article/details/glurnelqa.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfjplfjk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfatsqekq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fanxiaobao.xyz/Article/details/gewlcquta.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/glwgttvht.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gvoyvszwl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gpdasemkk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbjdhdf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvbwzrmo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbomqvhl.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fanxiaobao.xyz/Article/details/gjtkswkwo.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdvjcdhq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gdnzstnxc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnxusxb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gehlyuyyi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gohbhkjbj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnefbqgt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/gtulaiurw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gtxdztuxv.sHtML

[J06] 计算两时间之差
来源：http://3g.fanxiaobao.xyz/Article/details/gdfajwcrx.sHtML


<!-- 参考信息 -->