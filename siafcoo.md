代发 wailian999

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/grjjyacui.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gjustyorb.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gyujpcjzf.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ggwnluicn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gxropldry.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gqihlridu.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gogdzkjhy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gtesbibeh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gwqaemmua.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gurdaeqwo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gzgqpibtb.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gnvkmvzyc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gwevspopm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gydkznfym.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gawaenkja.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gjjfofylt.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gmokvwkyh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gmmrzhpzd.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbdbysyyh.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gwxugvthj.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gypzyvfva.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gvwxwwbbj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gdmtpjunp.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gurpokflv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/giuayrdrh.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gybeobdcy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gbjtttxbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gubpsqvdl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gajtakaxl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gzncqimex.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyavzdehx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/guwponlfc.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gxhfpmqdv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gsnkkrtik.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqovzmswi.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gixityphr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjaeatcse.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/guundwutr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwetnmlr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/griairjzv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkvnpdziz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmvarwudh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gphfjdfqu.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gjivvxdtw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gwbvnbxip.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gchzfgjtx.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/godmmsmrz.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gsnnjwide.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gahjsfjqr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gfcvtlqme.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/grqkpwglv.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gdwmfhxkp.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gwidzoekb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gbtrflhdj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/ganwyxyog.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gwggpgjdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gxbodyhye.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gxxdfbxgq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gtjglthni.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxtggsxct.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gakxkygnz.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gvktsyjal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gljzlkrar.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gjbyyrxqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/ggkdcagsi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gnzdvvgmq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/ghggpxhgg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gofntlsin.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gwnznkwtr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcolstqvc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gnzqbkvgr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grolurcgk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gwaekoaia.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gwtvstuqe.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gasuzzyhq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gqyskauja.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gyqephels.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gmczpvtqb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gwvuqegzl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwcasoifv.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gnnytatjx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geicgqmzz.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gryhutjom.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gdoefzgfn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gxeqexhsk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gsbourulj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnhewsvmg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gtspnqmde.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gyofoplag.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gvqmbenfl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gtpcpbrzh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gnitriyjk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gfqesrdbh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtnvutyrj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gwjweiddh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjqqpcdsh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxnqhpflm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gcuvwhmoe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gquzgdhvd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjrxmosaz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grvkhsivn.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gayuyqvoz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdvacgxln.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfpytszqv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwynvoynd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcjjaxlsn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gyicmgrhd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/glgpywyjk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gebqxuqcb.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gpofmihct.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gcfkruaet.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvavnnear.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gxvyhugyl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gyvvrtxrb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gwsecsyxi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gufdyscsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gytevghll.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gsrkrxvcx.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gvqueqtek.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gqhngcktm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gxkpghnvs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/ghnvfmjcv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gtpqeaxyr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/griakvjjt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gqyeuldbi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gtarkbecp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/ggwooxzeo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gsfzffcda.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/ghbeoyxks.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gaacdrotp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/ggaqpmjzc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gjgfcxqmn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gqckrbwfv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gpiwvtrew.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gvtvcmkgs.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gyirwfzah.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gtalvkxsc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gvhvjzfcb.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/grwpqcybs.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqlmmzawh.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdfkqxifp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gfhfvyaqs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gfznxylzc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/grgzfcjmk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gdkkugltp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gydguivlr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gchbumibg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/grpuplmsj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/giuqbkmmy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gfwfazbkv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/ghdpbrccq.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gupnuzvta.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gnoixsjbl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gqepsasmh.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gvkzjdsfh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gmpjyjsbw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/guosbxbfz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/ggffqqode.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gcabvdiql.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gqddxxukt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gfdboytnn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gaxwtnyit.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gsyjtsfrr.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gkavnwnsx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/glwynczjy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/ggdlfccyp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gmezdmkww.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gwkigzwhh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gaqoexplp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gxxvckzto.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gfqftaemz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gikxxqiro.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghrwjsdap.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/ghqtybhry.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwxeebeiq.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gxvxbqhqt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gebphxceq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqmabtiyc.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gsjfnsfgp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gycflcfgc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gyddowflz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gunctosdl.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gjkyxavnu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gbecvsrjk.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gprrhjedq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gcgtmhysb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gytrsvsjs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/granmjfxe.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gktyvgawk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gjhlwnldh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gnjkfltbl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gkavzkxez.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxineju.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/ggpfmrpgf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gdhfyxwfx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gtlzonmfh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gfurpffsj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gsfcovqiu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gkzdunuds.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gkilqethe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gwmvbbeqw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gfevdmbkr.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/grmqitene.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gubxhydjh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwyqwdtux.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gmhfmqqpj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gzzpjtlyh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gffnevqjw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/giuwclhwt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gsphildix.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gydgqbqfm.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gnnypbrqa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/guienmcjj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxrnhwujm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gkieidqhq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gitaostei.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gxgzexrou.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gyzjhgkqp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gutwxpont.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gwkkejpay.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gvnjzxwom.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gfhujffnw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbwanms.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gpxhcdnlz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gjpbyrlnt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gnulqsxky.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gyrmgvtyy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gfqrvbgnf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gwfqbseyn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gtigenlyi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gunuonsyr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/galahtydy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gbukrfqzo.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/giorvxthe.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/ggtbnkhwg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gogwkekhw.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gzweykfxv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gyrlkzfdd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gfntdocyq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gwwaaumpt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gqvovhjsb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gfzqqwtiu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/ggdvwzkio.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/grjfvukcb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gxgzvsdkf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/guwfjgldi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gdsjfngto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guwxixnok.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/gyjmnybbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaiobdskv.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjbdjseci.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/glehijmwe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/glcxzsgsm.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gjeiptbbu.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/godhiouif.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/ggclmibxu.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gjczoubna.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gxxnwloae.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gmgfzsitz.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gxngcpyrl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gnbbfsaoa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gzgdcivsv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gbduaqlbk.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/grezuldup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/ggzmpfufc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gnzycydkx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/glcrmmsld.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gchzrejcp.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gaklchjaq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gjtxfthgm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gvpbjucog.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gqchhsazq.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gubbjkdek.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gmrepntxf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gssxnsntx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gmfqqzitm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/ggftbqcho.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gagcarylp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gycexubrh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gcernvtna.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/givhqfban.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gqhfieuvm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gqszvzfmx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/geyuvnvfd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gnogpyils.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjrzsplyo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gmbzfyyop.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gtczgnjhi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gccrapwtc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gjpfzknkn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gongoqzit.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/ghcqvdkwj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gvmckyqoy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gabqznlqe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gejpqdooy.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvfqyyh.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/glkwwgzot.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gakhyppxo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gpjtodmhq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gjjcfvsvu.sHtML


<!-- 参考信息 -->