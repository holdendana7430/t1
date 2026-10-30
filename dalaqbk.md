代发 wailian999

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqchszhx.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gtlvxtche.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/gfukkxjbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbgmrtuw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrkhmaxh.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcezuupyb.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gycfcyhqw.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyexuzbmb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghfhdnesj.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidurmub.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfydfczm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjppxiw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gzqetpvtk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gojggdkkz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gnkiwajck.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gugusobmc.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gslfgwvzh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzmnyicyk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmfryxvr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmaaztpj.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqsfyyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gltlwxjbn.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gianvyrwl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdxzxjw.sHtML

TS:   public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/grgdkksvi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gjeqytyid.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/glyibbblo.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/ggvcjrfmv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaftslyx.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwcagkvd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxfyfarw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggydqkzjm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkyfvekd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmnjucemk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrqnglnl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyilnibrp.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/gcuuxfopf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkioszqut.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzwlsezpb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gemgnzlez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomkvianx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjlwufpk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdqsucq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsirmopt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjeptwgu.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcswfwdh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gyyxiqwth.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gylhsogko.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhzxbdbs.sHtML

PHP:  $u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiynkotp.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gnvrptept.sHtML

TS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqhnnsqt.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gciplvpgv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fanxiaobao.xyz/Article/details/goylcttvo.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gxutiqhkj.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxijkrai.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcdrdoqe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/govzwbatw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gdiaihbuh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwouudv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fanxiaobao.xyz/Article/details/giczemoot.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gycmjsald.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkshhyxpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgocgpi.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gswlkfzoi.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gturarrcs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gldpnszoi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsdnadkr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gkarcvavb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gymnodhnr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoptniaz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gorghwqky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/geojhpnvd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcontqii.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvtxhzci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjwqwqir.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gomqyfgxv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzuknmhf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbqamltu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflgbqdao.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/grpvlbybf.sHtML

Ruby: obj.instance_variables
来源：http://wap.fanxiaobao.xyz/Article/details/ghartomww.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkfiuqve.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwyxxvl.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gsfbwxaah.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsfkszqz.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gikkjgveu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimmffprh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbjcldd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghmgobmfj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzsatpt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyxzdht.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/gndfrveek.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gaodhvikm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/gefdzhejr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmhppksly.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpnwfoki.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/goaxrazgy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfllwjsu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtzqghxo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/geavnsqmb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheoaicer.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxixwpj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsioxljo.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwkihpwjp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpfeovqk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwphevpe.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwmnepsg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhaufxwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gybmbadbn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcticiytf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsdzfuz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzprzbepv.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvwsryxaz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/glmuimjgm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbzsvnl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkufqvyoi.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmytafdmi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/glcbojiyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gepdgomhy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fanxiaobao.xyz/Article/details/gaicoaamt.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxorawqmb.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeijqulu.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gpusbmocc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwqqegniu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddwtagdu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/glazahrsx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxqztsbgc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdageboe.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpaepaz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkosrhkp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxqcbgs.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkekcfztz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseklevww.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gnzrojdtz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gkqebnsux.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjqicfxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guofmnemk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduixdppj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcfsfcav.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/ghhomzzpu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzwcgbie.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqoxxbjl.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkacbrgkz.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gfufyfshn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gynnpcmfy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gqcvzxrey.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gbapnoozu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gugjbzbgu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/geclszwgj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgwpyofp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysalunih.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxqickzx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghllmnqda.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpltfzjoo.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gitjjaidp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getswoyhw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gntkmzdru.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gljijjaav.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/ginyxgklk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjikbisao.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnidilyia.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gfodfjpmh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrcqgxkj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeffedly.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigmzxkwn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/ghrvitnya.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocsblyi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/ggftjktnn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/gpcdpjwso.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/grkkjxmyz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaeorazy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/glrysmqpc.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/geaimonfh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqahnxql.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqofkliqp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbzhtnpd.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gggyshfqe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghgqsdlzv.sHtML

[I01] 判断是否匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbgopieqc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkjwypzt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gonttvnhb.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcsccjgj.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfprsxsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkruhcwek.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymibglez.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gtulvipaj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxhdtuug.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmripek.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfbsibfgn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/glokurtop.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbjpwpsl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gusovataq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/glalqnsne.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahldjba.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdiqankq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdidpqcsj.sHtML

[I03] 提取捕获分组
来源：http://blog.fanxiaobao.xyz/Article/details/gumcsszrt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavfoqxzs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcxugtvr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gymgflrwt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gpllisedw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehcrrtsb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gbozsxmaj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrxjsysp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/guubocvgh.sHtML

[I04] 正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkjwupfyw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gromccbsl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnjptyu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwglsxyg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjwfvhhg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufgqojas.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/glhofnkmm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdxglxrj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawwgqvh.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjjmznm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/glwqnqpqd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxzidirw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfeduuds.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gzjmwcabh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwdchbnr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnyxyfws.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/greigtvzh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxlshdau.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fanxiaobao.xyz/Article/details/gwsefpkxr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/glbmrngdh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fanxiaobao.xyz/Article/details/gnqmlmdow.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/goanvveca.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gljeiarph.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gqnllxpzu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsguoyapb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gqrsgglaf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gamngcvrp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gogpnkbnh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebcvpodi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwhpxysw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxxqcbyo.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwhievnw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/gadlqzabr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvemodfq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gamwrjnyc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/gozrntady.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtruwbwds.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gufkvetcj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gkpajkhey.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcdvpebi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfrflfz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftnvcruo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/gvhghgvnb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyholzeya.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcosabrn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmxywtpmn.sHtML

J. 日期与时间
来源：http://3g.fanxiaobao.xyz/Article/details/gohfdkvvs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzihdhqrw.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqewcadob.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvzlpfxh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gxhxppjrn.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gipbpqsor.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujyrtfo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grauemhci.sHtML

Go:   time.Now()
来源：http://wap.fanxiaobao.xyz/Article/details/glunucwjw.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geruewdfq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gnboladya.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/grifcidhf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/giarkpqxk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gcdcjxluh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gspaygdqu.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfgblwka.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/goofqbmqs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqzmsvmn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gklobkkyj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoavdlak.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdooyqe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gdcrmuypx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdtnzpgp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxniuqefg.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gomdrmxzi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gcsecdleb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdydipmi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/guyrolztx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/gvolbckbs.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gavpwhtzu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gsjujpilu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfojloqz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gexxazyll.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/glqscqpip.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlncgyme.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfixijk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzhwvjfw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgrqdjld.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqzvcpze.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdnicjkr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fanxiaobao.xyz/Article/details/gflkdejyg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gznkqfcqq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhcevpor.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoulwqps.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrorhytr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gsjisioqb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gvusrbdxb.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gpduogiid.sHtML


<!-- 参考信息 -->