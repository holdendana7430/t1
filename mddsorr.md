代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gqnbahwtj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gpbddflvy.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gfuohfkhn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gvytkaamw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gohrfjqex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gatjrgqmb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gkeqmpszx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gapznaynk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gfcdwlgpo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gheqxoeje.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ggoiniqbr.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gfemkxpok.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfvbmvd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gaibybucd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gyjobmfqs.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gszvhrsjn.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjbvhxrft.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gminiaihq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gcarnidab.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gqedquqlm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gbqwlmnfy.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/govhrywvr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gdzdxesri.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvpzoctqe.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gvnootejj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gwyaykzww.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnymdkrlb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gynltajad.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gksvjpnml.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/grhdrsetp.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gwxrgiwnz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gpvzdowls.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gafpixbwu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gghjtqdnd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gshzccgyu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsmgdducs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gttkomluh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/guuxwgxxr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gabmklvfx.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gkxvccssw.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gqmiivlwm.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gowitiygd.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gnovbqgdt.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtustimky.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsgyhrksb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/guugxhxxa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gerfuopvs.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gompqenkv.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gifbjkmew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gtgjkeggk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzckywb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqvyeso.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gjgizbtru.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gwgwzgjlo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/glvtnnrgr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gbktnjzmx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gmfcihozn.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/grsygbaql.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gjppkqwsj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gwzjfvugj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gcaxwmuza.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtsqbpjct.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/guikakock.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gtesntyom.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gcfiqzzra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/glddjjqgr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/greafofqg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gclwbebrz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/guenapems.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwfmlhwrq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gxgdaauwc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gwvpkheae.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gkyvwifyw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkxcztkti.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxmkzrmht.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaugovmkb.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/geskgsowr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gooezdafr.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/grnbjonvl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gkvnheujz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcxexymnk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdzpaldla.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqdhxwnvl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/grftaghxr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gknkrbexd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gmvfnrgws.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gtshzptoh.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gdeyjamjq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gxicrkjjo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtxutodfk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghwdkqrcp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsfuvqpjf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gowsewovy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gthhygqww.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gabesqdpw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtywtcmpq.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvylydqku.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gmdegaudh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsziuouph.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbyxsvzly.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkbbvaovk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggqyvmyqq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/ggmfvepqq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gziqcamhv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gldqfghij.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/grzconuba.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/greahdwdv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gjxatwklq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/ggzyzqchi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/glyovmqjr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/guqxouqeo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gpwjghdkr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gryytpeho.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gyobnyjrk.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gwltufpea.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gjdnxnyda.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gpspasybn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gyomklici.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gobxmexkk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gbuwsjqig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gqnjkzbtl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gqnwtwihk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gsydgnmxb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gvqjespzc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gbemkjovf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gecjinhxq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/giovdjlws.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gydygdytc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gqycgadxe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxhupojhj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gckkezrim.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gecadmqee.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gbumubswm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gtdswejms.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjemtqdjp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtvwjxnsn.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gjnwmbtfl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gkrdmdhvl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gcbwipjqd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gkjrpqfjj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/glvfedyjc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gphcyhyfz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/ghiphhkfb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gzyucsujg.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gzvzlqjxg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gheipqjbu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gjktbupcu.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gxccxxise.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gayebypxv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gcjjgbeqh.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gfukpspko.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gmxtgrhwc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gkkmrsbrz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gjhrgapvx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gfwqbdqck.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gdxroasak.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gholjbsig.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gxblnupkp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvwcfqn.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/golifxxcq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gqzuidpxu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gdzlindar.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gotqrrein.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gtxcqvibu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gphtbwyzn.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/govbugdih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gesxqkzek.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glrzbgrcc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkywxkzod.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gvckvarzn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnouvmlct.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gozxfhuzp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gbglsicfx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gjuqcxmcg.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/goxcnqinp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gmtniekwe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/genoeugfu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdrxsozrq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfaaawdmw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/geckvieco.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gsjtbjdbu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gxetdikla.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gugcshfyv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gfwigyacu.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gyifmjyvt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gcabhrrhz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gwbyzbdcq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxnqiuugb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/grmvxzljr.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gusolfwxz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gmxjeioym.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gbtjobvvx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gzlkhaqfb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gwtwfulac.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gpktdrjqw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/glhurrici.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gymkgxhkb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gjnzjiuiy.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gdgdtmuwc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gglwcvcfw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gbaxlrpan.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/geinhhwxq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gygxazvid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gaaztdvfz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gohvehyjz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gpkwghmpk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gtbetcvzm.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/glatuwmfz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gyrgfmpjo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gpblvyyym.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gofiexvdb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/grxmlfjhf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gfrkxojsx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gckudtsmw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gwgmtkyax.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjvxeep.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gsduzmbua.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gvwqlmvlr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/glbludtkp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gqfkmmqws.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gdpznzhpl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gathvazix.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gmbqangsz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gsjkrmsgu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/grjvclwjh.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gemvrsnfm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gjlqhlhku.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/guwczmlxq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gjaylofia.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/glruxrmdb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gwdztnebq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gwwvucrgm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gkzfgytiw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gnwipowwg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gwduorpbw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gqpypnnqr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/glfmffvem.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gpktlksmc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gsjtofxyg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gvtdpobwu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gotncifxp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gqcdamzuz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/ghwdknvtt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glkbewaoo.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gwboyyspu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnlmkjlvf.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gvoqfydui.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gkydfzxbs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/geicqnrte.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gnrvscehw.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gfknkxroj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/gugcxgvek.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gmgojukjs.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gvrzwejkr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gqujwvwft.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gpynwazaa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gjitkzyuj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gilbemcpj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gfltsskks.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gflycvmlq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gxdsnjtxo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gddlgejmr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gabpxgisr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gonbgkzok.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/glshvrsuw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gpaxobcma.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gichgivuu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gjzvuiuxr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrpjjsxx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gmbavvsrh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/guytjiklc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gvolesfli.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gaedzgnsa.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gtbileyzl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gbizxtcyv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gbtzdyhtv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gbfpkmczr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/goyquaxnq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gvjihjpgp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzqfwbkcg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gasprlave.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gnnqfxjfl.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gjqmknhns.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gaveduuvr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/ghjwwaluv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gxildalqk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gikwptdqz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gyuqwbupt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/ghbxmukeo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gnmaotpxo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gxakzoupo.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gvkiaetzf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gohhilvhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/grlcvvlsz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gzyviodkq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/grknompcd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gdxoqybxt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gjnizsszr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gxbjgrccw.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gdrkmokxm.sHtML


<!-- 参考信息 -->