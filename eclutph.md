代发 wailian999

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gwkispqvx.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gjtjjrtam.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gvwaxnnjn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gjmrolifb.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gyvsvvwzs.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfwonankc.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gayaxspvl.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gosrqynqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzvbwkwjz.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gdvlvnqwt.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkjivwgl.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gcoqpfavt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/grvnabbtq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gbwiuodtg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gnfrkwehq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gxksubhec.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/goilnwruz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gyijlijsz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gwdvwmcfr.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gxmvvhaqz.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gusqdouhd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gydexeqjl.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grntrhsqw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/giqxwxatl.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glcguvhlv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gadjdcfyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gwdaxdyll.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvunbkzcn.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/ghlhslpqp.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/ghoffaxfa.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/grridexlh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gmgmafbjj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gssjqhfvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ghnjkuqvq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnfglyxjf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnwrhkzrc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gjbeolkpf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmbfbhdbe.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gejpwvphp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ghtctfxes.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtgdojgte.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbujwwhoy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkhfoejd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gashegxva.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gugnjatdn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/guhrxalng.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gdaihlwpt.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gbqzmyqbz.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gkvlnvxbq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gotculilg.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxznejota.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghmodgxxy.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsqcpmomg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ggkiryaph.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/giwvpafzv.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gublxlqvh.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gnttpcvjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gopqdbyra.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gsoqzljnr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gmsczvguw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gifppphlz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gatfcvcbr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gdqqcbxuh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gwxyznzvi.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gmnlrrvxo.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gkhqoqfju.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/glqaczgzm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gerbrpeut.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gyvfzuuha.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkyqasgie.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/ggojandkx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gbgtrgtgt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gfgcjtyri.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqliuxoka.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/geakkffhf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gjfgnrirj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/geldpsgth.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gpxgdlthh.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjmgxxaxp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/guuleqswz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gxmefmsac.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gbdwdhpim.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gymhwvuba.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdtisyjbx.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gtjwswzhm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqnfsrmot.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gbgfptxsz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/giuchpfbi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gxkkkfkid.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnpvoqobf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmuniidba.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gbsylbzjr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gscxzygux.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gnszxvhce.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gpjkexnvr.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gnnmfwajj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gogmxoize.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvpyiawad.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdnrofkby.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqnrlncpk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwtlmkkng.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gokefgesw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gjifynncu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gepqgxgid.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gpotkipoq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gukciwavw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzxyztbmo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvoukkals.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghbbmzbbv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gfbzjpffc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gxedjujxp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/giycccbwz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkvxlncuj.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gyhqpdfdo.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/girkizpfg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gerbuafnk.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gxutkloqu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gckcspsxh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gbmgqebpz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gguxoozkq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gdmrzghrj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gcpsomeoq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gefhgtoxh.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gxhinjdvw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/ghmtbgqwy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gaqygbmnj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gcvsasrdy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gwwqmrzbq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gavlffjvv.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gkzuwbcdv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gehcmpfys.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gimfxihxu.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gzmxiyxyu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gyjjrjtnv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gwhratrjz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gelsylhrc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gorcberoc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/ggyflewsy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/ghoizcvuu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gvsutxjtm.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gldrtpemc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gxjjvdbov.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gifekksui.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxzmgazck.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqdwichuw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gooanpvwi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gnyubzidm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ggbwlehwr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/guznskuxu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gahzbdkrv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gusohfsic.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/geepmmjff.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gjmvydtvf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gntjcafzi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/glqzjfvyc.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gxtudmfxx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gdeiypbch.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gknfxltyd.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gvkbducpy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gixznlnln.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gpksxquse.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/giulgrqhy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gxvuqtdzj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gtdyhbrya.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghndqgjww.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gfkiqnosv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gxjrwjwpv.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gvtovraqd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gofrahmbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/ggxgemxuw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/guyvmcplb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grgrcqvxx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gmsnwxqrj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gbirjdlud.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gdgmyqeny.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwkafbpxw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtgzjkghn.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gkoqzeswx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geqavtiyh.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/grqwmqbsn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gfdspqvzs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/geqwakkzd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gbzqebvcc.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gmgmrcmkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/grzfkwcer.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/ggxadgkbr.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gajoctgyz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gtjsnkpuw.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/guvtgxgfu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gqnssuajz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gjwfdqudu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gytruwkaj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gylsnuzot.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gzlympdjx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gsfdyfeof.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gpwgqvlsp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsflgrped.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gowasafmx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gbhbtijnh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/grghrqmqb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gutkiunro.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gkizpttcg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gbagwqldg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gmpvlgfhi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gvzhzmcfd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gwscrndbz.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gtzzkjzfm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/ghznpwhsq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gfuwovxvx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gvafmeria.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnrmodjwq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gjhsfdwzq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gdkvcamyq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gkzzdfksb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gwjrchjuh.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gyeqqhxdj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gyimrcqef.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gcthdspxf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gowsovtuf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gewaxzgps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gtytukakn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gvepbnnxz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/geamctodm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/goedzskjt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/goyamjhvg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gbigargtt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gbsipijni.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gpdahdnod.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gdjldrjdo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/ghiglxwui.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gnlnfetlb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gjeypxqsf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gqebuzaex.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gqvpbftoh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gcqxbqfhb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/geaulqqcn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gxfolodzc.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/ggptnmrjn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gwdotgsqc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gkzmzuhdj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gfuuentua.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/giaikdcrz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/guqnwzakh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/giggxssvh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gmciyjcmn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gvurnahzv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/giwqgqjjt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gyguxqxps.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gciomhxfk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gvjticdly.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/guqdnubqy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gndtsnmxd.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/glfyvxpnk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdipakttg.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjaubwfzf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/ggrwymbuu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gqikjvygl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gvsalrqzo.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gnfjcvcse.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtfmpjf.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gbvhdciux.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gdrgajiao.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gtezyvlqo.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gmrlgmvve.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/grybxgrkk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/guxencykk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/ggulbskjr.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gdvnabvxz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gijqegcjw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gaiqrymkn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gfyskeuke.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/glepbyasc.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/geobmiwnn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gesrcvlxy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/goswgmfyl.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjzzvwckb.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ggobthlba.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gzazuiuol.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gnbxopctc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gfywfnkux.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gfmyxewro.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gowgobfom.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gidulyuoj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gozhlaqco.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gcwzadwdu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/grpdhlgaj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gdxkupkkl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gncwgueqx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gjvlemerm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gmfyozbdd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/guqodqwkr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/guhxsrlcb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/ggyfqtrfw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gzzpfdeew.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gcbuybnzh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlupyupe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gxgydzqak.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gqbzlguzi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gicsouinn.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/groxfgxub.sHtML


<!-- 参考信息 -->