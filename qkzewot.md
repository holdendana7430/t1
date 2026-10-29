代发 wailian999

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gmalvzfbg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gtdoyqphq.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gxybaqeto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/ghuabwfja.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwvadjz.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmutkhuta.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gwgyetiir.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gluiroula.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gftvchfmm.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gjfqmupcb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfoybcx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gvnairfuh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/godelriwf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/ggmgynedm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gmdgprejm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gaqtvilpg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/goirmcbgg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gujnaoeki.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/girubcgww.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gfzhbpial.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gkmwrcusu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gtealgpee.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzreomrps.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/guwlqjcai.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gqhjtzaeo.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gfjmhukgk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gruabzdzb.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gblmlckxh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gufbonspn.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gvzmmoaml.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gnielotmt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gdxgohqzd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gthphcjzj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gyqfvgmel.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkkfrdfea.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/grcqteets.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gqaqceadu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gahaulkot.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/geqgenxbp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gzbomycxi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gexhfftaq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/geylxrgta.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxatowfqu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnszrgtrw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gziwamyvl.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxasnhnvh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gplbqegwq.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gmotriiae.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gbdtdapdm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gfkmfduta.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjyyeikfn.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/glspywwxx.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/goyzqeinj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/glwdbpuio.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gdncwbgae.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gklrvsayb.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gglgwyqqv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/govoxqkkc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gcuvvxriy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gydthfjqd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gzezbnynw.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gbenlrlyi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gefvqbnbq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gzjknsalo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/grizaqpnp.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gesgvrujf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gmiifpltj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gpuxpofom.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gqxyaosju.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ghfjaljnm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gnehgzcaq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gxeuajxie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gyuckwako.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/glaawwpqa.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gkweijxlj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/geykryigv.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/guxobwbfe.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/grhjumwyi.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmfqkuvtz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gnpcpuuvf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gjjcjmynr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gtqhgrsdf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/grzonusch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtwkbchtb.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gyaeqzyxd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gclhjufxa.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gdhavfxoa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gsagwcgqu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gjkobiewj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/guqewandp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gfzxzbjdg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gfqbpjxad.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gdpjwryxz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gnewyrawf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/getglmptd.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gkngiaimc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gtlqlruop.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzsugjhvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gftfkvsnb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkfcnsyup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqhazxpnq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gmwajceno.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gpxdspcpz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxpavjxff.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gxszzxufu.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gpzgymvqk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gijwjcdvl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gepxgavwr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gozegppbq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwuttfywh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gknisibhr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gudjfszpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbjwupplf.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gvhrijwjh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfdgenn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gkvkfccev.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/giblksnyr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gsylkbunf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gtsmvdvdd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/ggmmlaisk.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/ghsgdhxqo.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gsohyizrs.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/ggpodoocv.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gkeuzlhdg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/ghquywqss.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqypeenjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gtobbedrj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gacsmsjcu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gzcslfnbx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/guonnvbde.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gmclugnii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gsmeibbsy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/ggcsxdrbn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjozvjrip.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gbexxjoxd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/giebqbgjo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gvyautcju.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gzjqldqgq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/ghfhloumq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gzegcgykg.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gcallkeil.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/giaaaeoaj.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/ggmyxpkvo.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ghrrlkouq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmzaswckb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gopwejdji.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gkrcxsjur.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gejejxrxk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gqficmbzr.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gcpdifvcs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gpfybhseu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/genpsuqnh.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/grpnjodnt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gzqduwfrd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gdemmoljj.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gtznfmvae.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gzmlyfxuu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gabnpdwjs.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gfintrdhd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/guqdjhobr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gxrssxakv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/glhzgsecf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gpthiszko.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gzgtdkwss.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gfsaqniwh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gswmqnatz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/grfwqourc.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gomisyrlz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/giecoqkdy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gaugglrdv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gaieetfvz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gkuxzjdnd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gbbzodpbl.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/ghysxodaf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gocekishc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gleotczcy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnmagcuch.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gsmbkzlci.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghsgkojzp.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gxfdxnqxf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gtzvmlbnd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gyglclzox.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gdbnxpyjq.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gehmykpnn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gluepbobs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gihxpvsyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gnqlaquga.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gqdqktouw.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/ghbpmefyj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gjvhhovuf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gjlkprdbk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/godqhuemm.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/ghexudjvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/grxyaxzfn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gmsxgezlk.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gffzwphmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gxuxfsmwh.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gqrbhgjcb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gjhsbmmae.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/ggmcgzsjv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/glcyislbl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gykqefucs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gxlezccij.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gopgjjsnd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gqrwwwssw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/ghxnvkzks.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gigeergjr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/ghvuoqehg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcaqygtdb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gbafqqrre.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gcmmpnejp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gxtttcyvt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gfmtpcvab.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gzcpwyrky.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/guhlqtbly.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gyknofwpo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/ghxqyqzjc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gdbasdurb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gdkisytug.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gftpkmomi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/guiskbdpk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gqkbmespe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gqzwaiusn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gmxmabmkl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/ghnmsvgje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ggwaywmwc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gihvvfnlq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gcvmfrlsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/ggiqmmwjr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gxewvcazw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gffdacacz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/giogvmhbt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gydapotty.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gjdxduqtp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/guznccsaf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gwweyrjws.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gewsckxyw.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/ghcchtgvk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gyancueaf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/ggmfgqxrk.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gvexnwdtc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/ghawlljsi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/ggikmudvl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/grrqxywrf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gomzqxgpm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gofdhiodi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gofiuclsb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gtkjdygpx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gzqumvrgb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gtydcbyao.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gojtbuefz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gniqoybbx.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gicbtqmnw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glosagqtw.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/grxwcpfli.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gdbytfeam.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gwnqnqohj.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gikryqslu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/grjnquhip.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gzptewgsz.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gsfqlfyuk.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gqlcmdert.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gmaujuuqi.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/grlztjnrm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/ghgoybool.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gmnftuyep.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/galybooiq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfcpkojcz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gcxcxwogq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/grkpmxpel.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gmthjbczn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/geahonrno.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/ghnvctpir.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gvcghhxip.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gghulnvpb.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gybjxxcbh.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghlduockg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gcezahftz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gruyoaikq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gibainxgm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gxlbftkkn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gupfjatlt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/ggsisiwry.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gudzffzbf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gztwmhfiv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gfgzmztan.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gtzxfopov.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gefohnmkh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/giercfjmc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gigynralb.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gpczlesux.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gxwdksfaz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gwmhgaohx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gyoxxjcti.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gksiblzbg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gyerkpted.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/ggnafhrgh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gxejplhpw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/getfbtijj.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gtdsniiml.sHtML


<!-- 参考信息 -->