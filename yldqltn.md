代发 wailian999

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gfzhrpqwc.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhsufck.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gbduiwzez.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gzwybvuih.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdwkxnhyk.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gmylfepqi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gvmlqktku.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gegpbdnhm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gkjneqgxw.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gclouwxmd.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gbaobyfmd.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gafbuvkyz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/goifjkeli.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gexfsnkfy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gxhjdiisj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gurtuhtuu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/ghdsncieo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ggbdrbquw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gbwgbxzgw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gvmyxtqhj.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gssbuhxfj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gedwgldpf.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmjwlbzvf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvjoule.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gnoxdxvtp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gvnhhhfuc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gysvtyqnu.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsialpkmk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gixdfzqet.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/grmnljduw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gktwdziva.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gnwssbbnh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gbcrgfskj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gyckpzmez.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gavvflhlq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ghisvslpp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gyrtamwmq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gmqqexpaq.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/glkoqtbck.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gauwopzog.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjcryctuu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gezzpbdbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/geklqzcos.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gixrccxsz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/glowlqwmc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gluuhxnnh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gfatycdhq.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gtimjrcck.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gxnhexehn.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gaylzkzdj.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gogtwljxe.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkuiukxjf.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gaiilalbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gzbpstajh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gqyrqghnf.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gykgffmqq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gfivvyjdo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gliwlkntj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gwcytgwwy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gqpupqseq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gsamcabks.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gdmrhkhff.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gdcfemlwv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gdoectopx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gvwgahayh.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gpabyricy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gmdyaeppw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gbjpcmgbe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gbcigtmev.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gguzqcjfd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gwwhmszvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gukigndgy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gyysimsxd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gcxvlnrmv.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/giilymuhd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/grpyzgpdw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gwfuctmlr.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gdzsldqkk.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyjxkjfmp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gioiqaing.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gtmrjcgli.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gyvwbviic.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gbnxxebds.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghwwqfmye.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gvqdabsjr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grxwtqify.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gqurezfki.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gutbwjsxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbfrrnaxp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gusnqazwj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/grlltsief.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gqzczztqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gdeoritir.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gfyjqdynl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gatlddwve.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gxukcmsvn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gppxvltcb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/getbsoxpx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghfiotovs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbbhcbeec.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjxvqiiue.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gsfcebcbn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gpegzwzuh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnadiynjc.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/glrjlfmaz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gsqlfenqw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvvhergnm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gemxxglfe.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbhenappj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gijdgjnre.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gnimmcoer.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gjwejbsph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdpbhtsin.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gebztwjer.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gbvrdffdn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gmrqhkyxx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gggrlzodu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gofuhkope.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/glywatauh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/ggeplfidq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gqagodlcs.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/glolchhdo.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gdqvjknag.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gfrmuqtel.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gueukdjml.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gxioqzbfq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdwiqfkau.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gdifrujqf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gekyfczgm.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gvhpipoof.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gmqtzzvrt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/ghlknouuv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/giuyclyhs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gkqzvchnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwjttbago.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gchsoukjh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gstnxqnbg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gqhevdbxl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gmtktiifa.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/glrfyxwap.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gapelujiv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gljqpdmqw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gghkgyiwy.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gebdxtuht.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gbtygtlym.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gbwxfoksq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gnfefucti.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gqnlingco.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ggnnmqbof.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gxsmkkoct.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gogxcbtrv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gzuefwtbe.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/ghomfpmkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gnarkcpqn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gmtsijnar.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gujwnqzui.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gcsdtwzjl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gmnywxsvo.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gipobhtqr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gjqsbqxow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gtudnijoe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gzulwqcxb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gkhbldygx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/geahadeik.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gfmorexyy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gbcmwqazb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/govtyxlgi.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gsufxawqe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gdhkrksvn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gvxtwekes.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gzudwbstb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gpyweafnh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gqiikxrbu.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/grqygztng.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gekhdqrjq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmcruwind.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfpmcuolj.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gwrxbhtsx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gokmgcsor.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gobewllxa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gcngvklnm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtgwbppxo.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gjplywwqe.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gyhkelcyp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gisynebwj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gkuomkzrn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gtjnsnhmq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gfdivrpyc.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gwpwkwztn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gqduyanly.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/grzxcufws.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gbnywrbew.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gkmeetieq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnxrybdyw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/grcjhsekl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gzccunrgy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmocxatwh.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gnyveohrt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghhgopzre.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gioanxtcz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gnywjgoaw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gqdxsaiyc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gmhwkfxyd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gpycjxpnf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gglncfiyv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gzuaktjur.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gheipbztd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gjpviqoiu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gfrakuvgw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gkdspsfpw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/geglrupiu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gjirppspa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gnecnplfe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjaospguo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gpsqlmhxl.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gtprgdiqw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/ggnytiebn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvaxefxdh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gcbupfovf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/geulawdlr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gofhygsaa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gixatzwkb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gxrselorr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gemvbcdjf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gzithncde.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gvsnpprvm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gountnlal.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gvtrdaelu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gxfbgcxqa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gppdgwieu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gjqoityho.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gzecotuqn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gkkswhtzp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gkepcwfyi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/geujliuuk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/ghklckele.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/grqbumezr.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gdfvrqoom.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gkjlpgttr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gkiurrhev.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gpdeuljwr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gjbintbgb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gjucmqtaz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gcldbaazu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gokalnnbt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gwememzde.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gtgtaaqxk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gjmwhorxk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/ghkxxzdsv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gudiqtbvo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gopzzpbjr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guhpgypsi.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/ghfntkwkh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcybfyrc.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gbxzmjykl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gemsmsgxv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gwuhpmqkn.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/glbxxkmcf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gocsxvoye.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gpvrdklto.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/ghnykcubs.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gvlpanwae.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/giktjfbuo.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gglthguhx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/grhzzonyk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/grbgywzcp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/goritjxya.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gainyfswr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gdoocklzq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gmopdxvif.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gpmcdgcyc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gttadmovx.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gelhnqnin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/ggckzyviw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gvzhlzivo.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gfdsbmpvn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gmcyhgrxb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gqjvxkjvw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gymwqimws.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/guovikiqu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gtcbwpewj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/ghstegqnd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gywsfgyxd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gjkeazuyp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gjsptgluq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/ggcnixoay.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gnoazeliq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gadhclobl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/glmpommkm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gmencmzuo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gixvncyca.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gkvpcafhh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gxayxjsxe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gyswbaptg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gkhqgjfey.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gpcgksapl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gqovrcjhp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gfcfsmoib.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gtzhaiwvy.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gsmzxzovs.sHtML


<!-- 参考信息 -->