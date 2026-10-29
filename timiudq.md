代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gesbqryxa.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gzkoayhgp.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gwviurelf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gzxvvoqaj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/grhzheymo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gnolovvoe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gqehpedze.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/grectahly.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/grelsvzlh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gbcytduee.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gaasfmnvv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghwfbqayu.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/glgxxyktb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gvqsbdgbc.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gfvdvgpon.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gyowyhlmj.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnhhhdjmh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gmmxlntqo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gxfvlvvgp.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfckimynu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/giiqlsezt.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gplnalqyj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/geicydcjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghgrbdfru.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gvrbpxaqg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gprpxpapu.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gxbqsufgb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gicjzhyvj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gjcrfuspv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gdngrolqs.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gnmgndqtv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guwgoijyi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gvxvjwelx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmkgdfkes.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtafizqzy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggjkpobca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/goivoddta.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtjafuzwb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/grrbiviqj.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gcomcvmpc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gdkqkxkmp.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/grxddiqwx.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkjjfmsse.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gohwdeefv.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grttsushi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gpbpftuwr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/giouktwhy.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gmalbfwdr.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/guvcursoe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gzlxczjyk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/goicvjllv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gfkthqboe.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gfcdfdbqx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gveylhszw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gvfaansjy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/ggbtcqhtg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gtpdxroyx.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/glbuigeke.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gflgdtujf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpfxeazqz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gvbdzdvwm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gxtsuduuf.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gextgdtoz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gdjzlnixv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gmiqrnmwl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gyuoylkrs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/guhtaylqp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gqvigwbmy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/grazbuzxh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/grcgusgqr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcaiprjuw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/guhltjdxg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/ggglnfztf.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/guscpvxmt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ghnaxtcav.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glrcxsqww.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gojpnllfg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdmqcyjln.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gxhzzzgpl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/guiqjonyn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gtuowjolg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gysmnkgvf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjrudbp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gfobrzylf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gyuzlkbyz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gozftblpn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/ggkoongex.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gezskhaja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gooryijaz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjofxbtvm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gbfuqczqm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gljwzedjj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghgxrlkod.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gjbuacwjs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gmlamqmxe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsodkdnaw.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gqswawcqe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gmdifuezj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghodubids.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghsfxrbmf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwviwmqak.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghyylmdwn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gdklpxexn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gjzywglge.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gjriwujev.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gxehydgfi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gcropkyav.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gryfbynvb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gleufrmew.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gowqapgew.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gzfulibyl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gowflpyms.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gupirbnxv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gctkyjmgy.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gumrpiqbm.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gabktqvcx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gisxuvaxx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gznjhpdkw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gavloiylg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gmycjorki.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gsjcebfao.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gvgungrvc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gumvdhfqk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gsstxkuba.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gwmtcwfxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grnpmckop.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gzigsekkp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/glxhthjzc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gvqgvqvoo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gtbjpbefi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gxinbodoo.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/ggqjdalni.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/godoqbwzl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/ghwlowvzn.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gchupfpxn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkzhtxqpq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gfrckkurt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gijztynhz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gzfkdcgzl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gvcuezprx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gfqyvuggf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/giamcgnrs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gpjdhoskl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gzihisiue.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gkqaamhxw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/ghbuicbls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gbgqxezxo.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gsyfvtviy.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gyxpyibnk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gaczczjru.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gixhypdgr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gdrsfdelp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gjqvncqtn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjkvmts.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gobvucykd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/ghxhkqjqk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gysrhjtqe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gidfbvsth.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gjcpidaap.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gshsuhflu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gicmbwjxs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gfnkncuzm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/giylnnzye.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/grlnbawvy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gilzbzrod.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/ggisixgux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/giypnhset.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grkdkyeyd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gigjhaxxn.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/ggcsmzqcl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrsaopkd.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/grptkhmky.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gzimaffkk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbodcyqoe.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gytdkjqsv.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtiwmryjx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gpzgiopao.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gxfikzlok.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gayiixpbd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/goeyghlso.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gsiwvelzz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gtbpmzxvn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gsooiarue.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gcqfujoic.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gblmcjcxm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gswsiyfum.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gobictxpw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gnyzfyyhm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gncdpcdmy.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gnxclgpvo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gfftfgvpk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gevriqfjs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/ghhbqhnxk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/ghenzvkcf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gxrllwcoy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gaapsouzf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/ghmvwudqi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gdglhcjoh.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gnbdcenmr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gqcyrjqlk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gqmujquua.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gzhxucejt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gfkfitmcz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gvqilltqy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gqrayfbnf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gegzxpubb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gcpszsxtx.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gfoagxppr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gdwwpabwy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/goqvpsist.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gxepzeykv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/ginspcawv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gmvyqvqjg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gknjjjywb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/guvsechre.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/ggxnsjure.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gxbqavfzq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gbaihuvpa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gxmynrdpk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/glsoxokns.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ggjmhycyj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/ghqjcorvv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gvqjpniun.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gjljtywor.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gvkscuhkh.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gbqxsmyov.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gsavnedev.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/glhbqjvsi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gjbvegakg.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gkkcvwahy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gnxlefprw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gkccpxdps.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/grosdibyy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gaylipnrh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gkgtgltfr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gxqkitffn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gqzxrwtgw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gjnbeuwjj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gffqbefcv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gsbeexnst.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gdxwboxzz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gniacllpc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/glzjyvsss.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktknewib.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/ggvsuiwsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbmyxezhm.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gbbjxbvpw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gfnkysxjy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gbbnewqnx.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gzmrjnxlj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gpqqpaeir.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gchwcqpco.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gjjpqmwpg.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gxzivddqp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gyotjlplf.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/geuddhpsb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/ggypcwomp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gcsrsgjnr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gsqdyetpv.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gtqzomzkj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gjqvqkgyf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gfxzkgykv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gnyjszwbw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/giejvpxck.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gislieucp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gayaierfs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/ggribqkrl.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gayeorwiw.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gummhtqww.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/galmlytlj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gdwpdbcya.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/geleduesu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/ginajicih.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/ghleztobg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gycctwizb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/grlmemvfj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gtucjcshk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gkxshtjmy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gbnxbbklx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gifiobzio.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gnslgnlex.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gfnpwvdya.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/ghbakpcgx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gyuwsuzwx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/ggtuoayqh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gzbbhrpfd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gelycixnb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gvwcbxioi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gqjzmtqah.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gsrnfotmc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gsnnhssku.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/grioqcebz.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gsyekjbjf.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gptnqzayt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gluuyizhh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/giemmpway.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/geblljwxj.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gmepozzvh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gxdxbtrhx.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gchikdzrr.sHtML


<!-- 参考信息 -->