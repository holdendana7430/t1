代发 wailian999

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gdoebvhzc.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gnrfjlonj.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/giyjbxkjh.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/glslltvzm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gcwluuhkx.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gcttiatho.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/ghmhlemao.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/ghceajbfy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gwqfijhnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvucyxfbh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gmyqgcmeo.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gyxkuvuar.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gmtggdpju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gegqphuhl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gljzaafau.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gooqlisew.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/ggodvbmyx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gcrcsszyh.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gsmmdlkox.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gjlsomjkx.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtcmsvgjf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmzgskini.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gtprfcyjk.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzwuhwhwg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gecptnmdz.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvehidqzk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gtmuujoyr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqpgkdiis.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gnodyzjmj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwciegkum.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghivzinvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gohojubep.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gpkgacefc.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/glyberfcb.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gkvpsclgt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gsgwwzmby.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gfrvdlxpc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gnkblhbmd.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gchzcsaiz.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gsjiinyig.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghyotkylx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gkazkkeey.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gqqoespbk.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/geunqlggm.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gxmghqsby.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbusixojd.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxvsachys.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtyhvncha.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gggbckeai.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gpkwudujd.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/glzoihvsd.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gimxefunm.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gtwwxcfka.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gsnbbohkk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gnnpunjbz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gdxasnbug.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gpdcshejw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gkwqgjmwz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gbuuvxgcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/grciapglg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gqivhycvb.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gpmxnrvno.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/ghgjfjubw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ggpnvuaft.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gzealhrgp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gacfjdrmw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gjxoufoey.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gwhoiuwfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gmogntvst.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/giziapeyb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/ghiwxdbme.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gaoeaztnq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gmionbpkc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsbummrae.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gmxrmemyv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/glaxxvbng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/glgyniukg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/goegmjedb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdmqswupn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gppswdips.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghwbzjdkw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyaooqiis.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gkynmwvpv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gkrpcffkz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gpintcdmm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gzkycfujk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gjcuqhutz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/genbvtxez.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gsrrxclto.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/geporlvlx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gmtkjwows.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gyxagjobt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gdvcjucas.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxohdyuyb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwrpkaccm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhuutlua.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gromxggjb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gxlorjuwx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gtwyombwy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gscnppmyw.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gdjoipepb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/glchrmqiu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggrnygpok.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/glqgfjstb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnylingqr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/goabgqrhp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gbebephif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gvtshlbqi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtdrxqkmj.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gxobfowms.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/ggwqrnwmr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guplrfcmv.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gvpzsfbah.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gtdjkemih.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gxrlcqcsk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/grvdwpgne.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gjpgeprzx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gftsyqvbf.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gvgfdvari.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gnbjydcyj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gnbfwckkw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gltupmpwo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbtvrfps.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gnkrwiwcs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gclcnjhay.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gwbuhcpzp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gzjxexxkp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gneubnhwu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gdgmdabml.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggzejtadw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gptiximws.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ggmdrwniq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gwojkfyyn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gjtjwusow.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gmezskdsv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gyukgvzth.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gmbmcslsb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/glupmadzw.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/goofmqdew.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gpmnehean.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gwqcmflkf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gnczegync.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gssbndgld.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gylvpousn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbmdxkjuz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gkbypkqdk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gtgqlhwii.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gkgollxfr.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gkpnirokg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gdlqtninb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gdhrojtud.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/giibmlnss.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gcmwtubkr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gglipyifa.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gvydkfkne.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gdezpnskh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/ggisygobw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/ghiknabuw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gwiacffhc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gvwadqstr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gltkxdlfl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/geehlatci.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gaqfiyoyy.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gpztimykc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gffdjrwtp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gkojxfmbe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gxxggaqla.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gngmgidkl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gavxuzgwd.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gkgydlxgx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gpozlhwdd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmodmbbdq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfpzvlkls.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/guflzclbx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzcetbtbf.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gexnfbarq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gyulhphkh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmdlcnjtt.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gktslkwtf.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gvgfzumww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/guitnwpca.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gbheunqld.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gatmoqcof.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gkytqjmgn.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjqndhi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/glwmuzeqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/glggwtnis.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gjslktuwb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gccthxvtv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gcveqcnhs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gvtpeqdzj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gdmqsndja.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/grtdulsgk.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gcarimodf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/ghhjtshjl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gmrsryopl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gnpueidhk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gpkfipffj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gqoabhebt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gywguqjgo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gwqhbfclp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/ghifoikyf.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gefmcrltf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gisgeqomh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/givofwqbi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gplgotfcr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwjfsuywq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gccjrwtta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/grqqdcjha.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gcvazthnw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/ghfvfyerp.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/ggbvhwzzn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfejujn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gudolfnhw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gzdqsrqau.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gghzgbplv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/ggrghpqrh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gmylzqjuo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/ggmkdkiwe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsiutap.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gjesunlhj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gstuixuwt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gndhyczcm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/giqqejerg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gexocbeqw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gnwhiucap.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gdiblzkfe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/grvlbipbp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/glczjpjoi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gdccsximv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gwuilgsvl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ggigkvscy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gomayvqhh.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/ggvsnqwjc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gfgrefocs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gyedcalxd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhabkez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gdfrkjkgm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gyuhdwsmt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gzdfztygh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gfcovvhte.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gootgaawu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/ggkkxmtus.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gpmvssdpt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gmfydzpqm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gjfnvjrac.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gdnzxfpui.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnkymiogq.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gffqfidgk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/golehdmkg.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gaozoazqh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gohcpvywk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/grsreohqj.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gnsuohaku.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gogebmted.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gkrbfkwqn.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gurjxskol.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gwojtrgei.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gqhqlmnhm.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gvzvbegar.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gqqebrxcq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gxbzmqmoa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/glacyiiyb.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gaucmscym.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gtgcaxkgs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gcwusipwv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gtoioczmd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gpmrvgkio.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gibibcirg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gnmluuddf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/giuvdhvyi.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gcsomijse.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/grqisujta.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gvshujoju.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ggrwcbhqt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gmkbpapyg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/galzurdps.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gaofzxnda.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.hesvh.cn/Article/details/gxffpvymt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gtlrbxhcx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gpcekieje.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gzlmvittl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/ggmiusypp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gcxxihchf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gdxxpgtsz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gmurfxooy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gfrdjjbbh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gswvlcztq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gixlylvbc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gigqncpzr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gihlszeto.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gfqddfnju.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gkpnoujzt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gqifzxvuc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/glbdrifew.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gplnbgwtr.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gqbdxvdmz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gzbigzrjq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/geeqioize.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/guqhmvbgn.sHtML


<!-- 参考信息 -->