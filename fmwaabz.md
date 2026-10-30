代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gulpogapa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ggvikksnp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gwnyqmxkn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gqqtdojak.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gfyrtspod.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gxndcxngg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/goupklfev.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/ghpwmkmcz.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gizrdibnz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gjtcddfzk.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gaxfcynvc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gjfrjftkz.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggktutorl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gqjehfcbx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gkvhwagbm.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcdsgkqov.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gwkeasklb.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gznytffis.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gjrcoprud.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gnyvtynpp.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkuqkbzer.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmwbznczu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gniwzymuo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/grqljlryw.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gtcootxdk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gvqdlqtlp.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwhqqsuxk.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/genijrhex.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gojzkeehz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnyjall.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gngkvkrdv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmufvgadg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ghdbrxxpk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gozvycsqa.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gskueicjh.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gwtdkzmmu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gnepbgyms.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpigfxcbt.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwxlordje.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gnmfcadem.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkpoibivs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gyzxkthyg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gdvutpdow.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gameemiao.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gvczvufst.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/guuyqkhpv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmjplokni.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gbyrmqhws.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gdpzepodw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/goswuiroi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gfidpeakn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/ghmtpsvkw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gscokamux.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gwtxxdfvk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbufiaocu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gxojemzye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/grhfepndp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbgldjjdj.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gyzrxpwup.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gwyeyxqbj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gsooygnbs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/giljnuacx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gkqmmuugq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gybafhhiz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gfbtunyvg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gryyqmkkv.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gfqvpymgc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gohsfdurs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/ggayhobiw.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gnbdqidje.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gtqmpvwsz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghejwoqlq.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gisujluly.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geymqadtj.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gnshqvldx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gibuiztrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gicjpbsvn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbbabanmk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwsrqlbls.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gicyhyrzm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gysvslprl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/giypabjqe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/ghxdnrfgu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gjqdopfhn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gnepswief.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gehwcuomr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gsglvraob.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbkuxqveu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gusuzrzib.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gznsuirra.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/ghtngtzqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtubpqfol.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/giuyvpvkh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gwjiodzcy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfpddciaf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gdmtirvgc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwsxdsmfr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjsixsaop.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/glbytyasm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gmogmhouk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ggxpmbrfk.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gwcmfjckk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/grdwutdvg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gwshyxnqr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/giggjaxhr.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/grxkwyevq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/goesurfpf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gnofxezft.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gfulolbsh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/ggwavgpei.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gissplynd.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gfkgjyqdy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/ggmwpsmny.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gcjvrmygo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gxtsoaeif.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gbgadfzfc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gtiakpzkb.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/geejxrjbo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/grzkowqea.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gjwllxesy.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gadurzoxg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gpylaqdwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gtmvdsxya.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gxyzywitk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gssqmlqdf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gdwbunkrr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gebampwnq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghhdqptdo.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gdlccdciv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/ggpssefuf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpzpiauak.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gpkaiogqd.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gailkhrew.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gdsdllkgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/goebbqcip.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gabvqxlsc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghsvptuku.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gfmnrgcfo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gbzmgalwr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gvapbhlzu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gepcpqebg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gbsaxtbic.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gppsvuzkp.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gouepzcqx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gtrtcqdjw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gyhpyegqx.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/goyakdgsp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gwlczzmkg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gtsmtajkw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gmeawubql.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gxzzyvdyc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gjvwrqiuq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gwmmludoi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gamogusnz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gjplixmxq.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gprtcoqvq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/govvazqbo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/ggzablgbf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gquklztbr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gnaigrnoz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gpgmrffxk.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gggyftrnf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/goqwdnsvz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdtnyvqom.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnlnzbfff.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gwwspbzqb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnbxhleay.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gxhobpudk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gjunxtiks.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/geipvzpsv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gopvihmep.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gskgzhtcc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gwpmydhug.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gthuzjrun.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/galeopynv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/ghntwmdjs.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gxbfzubho.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gccsmxryh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gvyqjffid.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gdyzuqnqp.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gpghhzpor.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/ggcxasgir.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/ggreqsmit.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gikxmkztj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/getjeaubq.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gynwjfjyk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gswoekkob.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gmotbkcho.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gsvmutlra.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/ggtwikume.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gmznxynvg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gpnqvhohq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gpszpfawb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gvvazstue.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gdkyyjaqw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gwunhpwih.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gkhgxldml.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gvuxlqefm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpxjzoron.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gegtvpvbb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gukjydpwa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gduzwnajs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gpticitss.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gsnucaytb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/ggmabspzb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmruspjpe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ggukchszn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gbwggukdl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gbrbftuto.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gqnvvbeol.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gqgcktbgk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gjipmyqep.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gysjtmcjh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gaftaxthy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/glnkxwxws.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gjdkullxp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwejqoycf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gvwzzjnrt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gvltokkup.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gkjpjsfte.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gqrfhwtqk.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gshfdranc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gkgprbtbp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gsmnpolwl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gqamkkfmf.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gwvbpbhtb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gqpeysdze.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gylxlgnha.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gvlubujca.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gpttsckiy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gcwbyhngy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gyypajfqx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gclliftur.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gghymvxvu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/grpbvotkt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gcoaxefrf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gkqvbyjra.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gthjxomll.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gakkxinkl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gorhogzcz.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghwclxqht.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giauvltfg.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gfahbgkby.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gvoirufag.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gdjudibuu.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gvsphgjjn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gpzdttohu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/geymcfntp.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gamkeomfu.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gxwemsueb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gyvugkxjj.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpmaegpqf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gddkabtzw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gvhkfxtal.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gcncotipk.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gbhbfeodz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gotdmjsdn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gdxyafsri.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/goorvrxmd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gxtsrigry.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gvxtrqtro.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/grdqvlgtb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/ghcyfxqab.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gxkxmjqlc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/goxyuvwhg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gsmvmxava.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gsyrszsvj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gzkpjbktc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/grtuwcxwb.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gaszftgxn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gbogdufmm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gsxzpwlcw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gpfrkykyr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaiakyqz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gjfxylqzw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghktodihx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gkxokvqnv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/geoibkbvx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/ggmxsitxf.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gdxrabyge.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gihlmuwgu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gxarkboeb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gfboangxt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/grlvsoxnl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gimdbgqtq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gnreopref.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gnozymted.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gxvpxzjzi.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gfvplhgdz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gygbitufx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/giapcecgt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/glbirvbtt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gwkvfsoqo.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gllqdmawj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gkrtjkkef.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gnwmpriys.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/guzclzttt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gropquord.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gifvwujle.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gifpxholk.sHtML


<!-- 参考信息 -->