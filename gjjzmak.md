代发 wailian999

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/grdgedtmm.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/galyejtlw.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gzvoulhpf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwzbgrd.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gfvzomctg.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gifkqzezy.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gpuiswmib.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzctmixhf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkgljovbs.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/guazcvfmx.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmnjvrewc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gkxjsqxgt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gpksgklig.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gmdbwjive.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gamkiqmtf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gecwdyovu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/ggcyjpfgh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gfuavdpgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/groroypqm.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gcikhfpub.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/guhfrflyt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdqapsele.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghtzxgfbf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gddrjmzzg.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gkqloeusw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gqqcicvej.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/ghylrsggh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyfghap.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gntponssu.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghuaxuvie.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gdmcjtbso.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grjkbbggs.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gkrbhdvyd.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gmggdjozn.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gcgpwsvuo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtxpjvrjp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gbvzxobon.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/giztqvlre.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gliurfqlv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gpipeccjj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gueiatnye.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghsvqekyc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxrlwypri.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpmyvtsua.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gqlxrxcjz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gobfyjbxk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gqnkpxung.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gpjocggeq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/govcqgraf.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gtskghvrk.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbhwotswo.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gamhvzmgc.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gdmkfzjyr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gdekwcvbf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/grnqdcjug.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gynwjkutg.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gztktdiat.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gfdsawfzt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gybfiqixn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gbguttrgx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gvegmkycp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/ghldymemw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gsimszmfy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gupwskpbw.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gqilbzxhc.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gtogbtrzd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/geefxehmq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gjnnfhops.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/ggxwpbbmb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gntbciutv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gzbkrjyiu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gzxxhooda.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gozoutzqv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/ggnufcscf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gefkexhtt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ggjkhzzgs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gugwqaqku.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gofdhklhc.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/grktwcxbm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gksqmvqmt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/grqgduxpw.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gqinvcqzr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gktlnlblw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grlewjeyn.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gipwqsbpw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpolxecue.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gejnxendj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/guhtfdliq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gcfdmlrvf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/giqjlyssm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gqopmvtvw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/givcppnnx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/ggucitgfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gkkxzuyvs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gtghpgjys.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gpxrzgksj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gaekrfhbj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gryepnect.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfrfphdgz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwthxyavw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ghcqysljb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/ghkztfyei.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gouvrafmb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gebfnxama.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gyowtlwkt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gbebrpdxd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqqxiaosb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqczcvpon.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnqusmhhq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxnyksaye.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gganafrri.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/ggczffsxy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsqrobkfz.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/ghmgsybxr.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gdtqjjcfs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gczmlocic.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/giftcwzah.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gkfdrmakk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/grwdonlva.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/giyhturfl.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/glrxytjrl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gggvbrofb.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gawjudqox.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gekubeylr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/guokflrsb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/grmfjclmw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gzrpyakeo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gprtkjhay.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/geooalaza.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gahztoyzq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gbivhfaem.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gspccpwli.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gvlrauste.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gnyalgqte.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/grrqlvtwt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/giatgwefx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gvnduprkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gncmgizpn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gxgcwyowo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gxsnoxatg.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/ghpcutddn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gblvnqgrd.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gpydlhfoh.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gamuwirah.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpkqmutpu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/ggkylqmoo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gvjezpnif.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gmgpflorm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gddomnhkn.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gyipaoiqa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/guipdtqnp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/grqecextr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/guzfkwdjy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ghbteomis.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gdlczywzi.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gsciwqhix.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gtsgbvwna.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gxednuzjs.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gkxjkdpfo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gudxiuijg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gzhtkzskx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/govhwzfey.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gcspfanay.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gzhhlvrfr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gjwbluwlp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gjyoatdwn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/glvpvzwkt.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gdxkflfge.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gsdhzjpla.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gtpfzgjjh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gltzikyft.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gbbrbtzqm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/grvexgnpd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gslhjhztj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gyewuhoxq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqdcmryxe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdgsygvlv.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gvdujloyw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvnjcywac.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/ghljcvdlj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gsblhyimb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gxmeaobsl.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/garqketls.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gpwtjhxdl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gqsrwfqst.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gvpaaeigp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfsljfs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gjjjfwogs.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gqkdieqjh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gnackzgxo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gfobpolou.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gqfkaachx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/glmttdthe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/ggsegfmcp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gmrbbfyzc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gblaqdmid.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gtbhwuuui.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gllcwwotu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvrkclq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gjdpnncxz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gvlefucdi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gnmqilhlk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gxqbbysio.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/grpwsakvp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/giieolmnx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gicmynxqd.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gmgpzurka.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gcjwktvtq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/ggbukyhkf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmtuovnzt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gldyjphft.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gstkbamxn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gmbcdbkbk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gfiaytjrf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gpfnfflkm.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gpqnvrckd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gxwexdxou.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/givsfywde.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/ghfldmzfm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ghvghjphp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/glenwjyeo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gvqnssvpv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/glrjhnamk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gqtlxvshy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gngsaddcd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/grtpagolw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gsevajfei.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gzijnrygi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gbzweiamy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gdwnkdvhh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gjgbgbhoz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gtbikpegb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gthtutica.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gbpzdfuag.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gmfnduiyj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gttwcwtzm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gbcdeihuz.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gxzybebca.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gbvijmlqa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gutgqzaby.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gartrziov.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gmjrqjisb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/grupjqesv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gcinvhdci.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gvnlhnuix.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gnfndospw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gikgtknlo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gliqdrrwo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/grifeidzx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gdufhfpak.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gsjvsbzld.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghlpnlzoe.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gotpgljto.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcxxjhthn.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gswajqczd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gjgxjvgss.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gdwnrzzdo.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/ghkyyvitm.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/geystpitq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gaijamulg.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/ggfzqhosq.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gssyxrwgo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gjwgndhtx.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/grrfedved.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gnuiimyye.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gleywpwkf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gifulcsfo.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gogljfukd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gggisenni.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/guzywssry.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gwlrwhwkw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gewjbwfxi.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gguogkanx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gcolwgdnl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gtnwsgems.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gyghtbmca.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ginrfkoxr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/grbyerxre.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gznbjyond.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjqvvrjhs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gasbwbzbc.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gzhgznwoi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gtmcackrf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gtuygennw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gjfgplpve.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gvvhrgusk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/ggggeyamz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/glshdlnnw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/golugycqo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gqtncnlnp.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gobjgutpt.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gnttmqhwj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gvrcsggfz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/ggehnusac.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmtzkxwnc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/ghztqqpow.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gnogccobt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gudifphhn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/guqaosmmt.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gfipjknyb.sHtML


<!-- 参考信息 -->