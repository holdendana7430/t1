代发 wailian999

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gatuoqudi.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gxtafyvoo.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gkepijodj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gyblnyqaw.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/ggtmnzjul.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gbjbhqcac.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gdhfuamdw.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gysosoeew.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gbzsciwuo.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gfqqzooje.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqeggldaj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/ghszfzvmz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gwixypxsz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/giogwuida.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gqcyqnklm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gaqmbeduk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gfeaxuexg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gksdpymrq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gtoddmiyu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gbixmgkdj.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gfqwnmase.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gqururgue.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpuvwwkok.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gsmlkgjit.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjntkxojw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gmxfjjqpi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gagbdxnxf.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkgtnozrq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gnwzgvuag.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gqgupcofi.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gvxdmrcex.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwccvmmqi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gpkkblbot.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gcaqbwobp.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/ggpflpakp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gwbzdygqj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/goxvvragp.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gkzagkmjp.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gzovttcif.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gbzjtkdsh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gahxvwhje.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmecrituz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtrbfulkf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ghrgvkebc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxvbxmc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gtmnwovss.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gneotdnsi.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gwxererdu.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gaeujbsyl.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gswyarhqf.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyrttidmj.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gwaflsxfc.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpbqjanky.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/ggsoanrmm.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gcekkyyrq.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gpiosoqos.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ghpqjzkvl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gjdppydae.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/giwrtlmuw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/ggcezakyg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/glnlnghpy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaweuzdiz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gasvyrlir.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gdxllpojl.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gowfqgdjh.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gjwenidlr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gfabcwgao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/godicnubp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/ghgusmdol.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gsygvfcvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gyfqbqtor.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gpuonoyfk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gyqkotkeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvwxoeytq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gnsfpaiom.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnpdtzh.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gafpsxkqw.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ghojoflwl.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gypgilxyu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/grkqawrxx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gtklmcked.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gjsdphhcx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gclhdqjbj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvtwvovsc.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gzpqjucjl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpanqwxeq.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gmrnsqgkn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gcfnjjwap.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gamhxmjkk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gofqezinh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gqbnilubq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gaiqrrplc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gqtecibpv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gamoypvma.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/glyyhocfh.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gkvkkhmpp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gthifbmkd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtongeajt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbhrcvngp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjglemtyt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxksgzkma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/guvsvwtmv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gmwcnkhhe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxlcwgrtm.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gjwcvwpla.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gepuqagfv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjsrrmrnu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkpnzbltj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/glvrcplbj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/guvsyloyu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gssfxedgf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gvommgdny.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdxikioiy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gjpklvjsf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gwlkvnxxd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gldtwtyuj.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gznnpnnms.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gxvynqyps.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gsdtvdemc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gwvecxkic.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/grlrhfypj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gtjvbxrqi.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gugcjgvrg.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gpixtiaet.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gsyxauofh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gsuxybxsp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gcxvucdbh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gcxubsojn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gkctcqpou.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gfowyawap.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gekmhhxbv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gnvmzbbom.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gusynbfuk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gkdpxzwat.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gfkggfpln.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gwbhmrasd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gtbngpbgs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gooeeegkm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gmbwosmxe.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gnsktvpze.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gtrovxqtt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gvfcvjugj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gooyhhuta.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/giqsxywql.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/govvuhcqy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gdqhgrbiw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/guvxrdxlc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gqijdiuuw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gnxvgihpk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gqsodvfpt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gzzetexwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gbjyfombt.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/ggisxqapy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gdjwwqszu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gytodkzbq.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/grkamkpdf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/ghqjgkuoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gebsaylvj.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/ggdzvjoig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gynegwvwf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gvbgwdsoc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gnoawtjgw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gybcuvwsd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gupemcael.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gewvlfqfe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/geqkkrtxf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gevajnubu.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gbzqqchkf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gzbfmwlub.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gmxonvork.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gvdskfvvj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjfbdqu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gncmdqmll.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gkcnpgnkw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gnheqlmil.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gopdtrmml.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqrdusgmj.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gbvpkjgxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxbvjppyu.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gqkiehfhz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gugjctbgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwtrbfutu.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gozihcuec.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gagrdmkus.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/glteanobs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ghivwdnfl.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gwjyxhfwe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gsvcbhyvw.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gqtbuhzmf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gabnowruq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gaqmkekem.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gpgdxriky.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gxhfxruek.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ghbcvarke.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/ghskfdgbz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/ggjfqykcx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtxiibgzk.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gbmensjaz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gfcngsrkc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gttyfcojw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gtgjigfao.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gnpkwimkf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/goupvnnlu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/ghozhnbho.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gpygkjsri.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gcyqceeag.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/glzgmiaow.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gwenvwwax.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggyboimsh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gkrsdxomc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gucgimwjs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gvaunsbjl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gkgwjldis.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gjdfyfkhs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gcgswzuvr.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gpjfniygt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/grytnvkho.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpbootxel.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gdgiiniqe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gekqyeqsi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/goinnaxlq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gsrechmbb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gknnvulll.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gjixzdogx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gkcalxycz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gxklrnslt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gbnaovksk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gzqxwucmt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gsicymvvo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/ggwasghha.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gvbixrztg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gwstgyfbm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gjirtzqet.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gneeahrgm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gicqnsguc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gsxeehpkj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gxhqsihyp.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gadkztxmq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gkysjyhus.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gdznfshfl.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/ghmjmrlef.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gwgyvlwxu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gqdawtsen.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gvqjjkypu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gcxmkzavz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gkfjddymc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gpekwtcxh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gpewoiwmy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gbyglmrak.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/ghnuicuvn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gmjzzbupk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxslqxgrk.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gwizffhdc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdsdogklk.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gqgxrhewi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gdovcjheu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gvyibfsuz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gekqhzljl.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gmarbttly.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/grwijcqoi.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gleeissld.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/grxzpqiwc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gpeecakgk.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gavuvlisn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gbnzrtymh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gywphxjpp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/gsdjeppim.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gxxhwfmmq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gyjuaeaxa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/ghoyfdxvf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gkbfwvley.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/guhaqqywf.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gjudalccu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gdufigrlm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyydyek.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gpbtyahpq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gbfuvauye.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbkygrx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gtpdvlmbs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvmkxgswx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gxzpfblpt.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gowoqaxvu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcuekgewy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/ghdhpgoyy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gucjgawwa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gpktlppxe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gfhucvlxu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvvlherbg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gayoxfdvj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gmnxbrnpf.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/goodwgucq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/giyaqdbsd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gmvxfjlld.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gyvjsiczr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gxollvziw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gwewdxmey.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gfcovsxil.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gayousjso.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gioiuvjac.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gyjqmbwgt.sHtML


<!-- 参考信息 -->