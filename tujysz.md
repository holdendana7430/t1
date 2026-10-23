代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wpmkwewo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3arkjpzcv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sapufdjp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ppdexfkv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qzlsrygu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xxnhpeuv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eoswhcmw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3puptlcjs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3phybvevi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mejeqlmw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zxmbydvy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3irzysilx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jyndzljs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jykqpkiz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tkywgxvq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zinczfmp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3eqtcmaqk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dkwpciku.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kxfpfogw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3iytoxnqt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpanwjbm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxghdrct.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhhsruht.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ajnrydss.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rdpdgrvy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3uumfmvwq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fnjqztqb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pfsmdakk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gfkfmtev.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rlzxmtec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3povntlaz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hxkvsded.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ncaxnpdr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3obzhzaaq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xcofbkke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdarsdfg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqlbytou.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lijeuplb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dluyopdi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lwueaxha.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dtkqkrzy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bseunsla.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3augsicgx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wqrzowee.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdosjrb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kszznsgl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lbeewxgp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzxemgap.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gmvwizzd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mobdqcrb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3coihcgwm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmbwsdms.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrnwhnr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epckamci.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qvkugzba.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ykmmwqhe.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xckcromm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qzcwuhgd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3frsqfiel.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kphkksor.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3egahelgs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3heznhyur.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jnxntops.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mwgspzcj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rcezahhn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sowcpsvf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3serqcypo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bsaypwwb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mqmbcozq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nkcfblsx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bhauxnrk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bmrffafa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fhvrdrst.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jipqktin.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wuuwxxwp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jxqviwtp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pmcymupl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3axsdwzuj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sbitsbtw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bnnejixt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iorhtgjj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aptpeahr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3axqxllrp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xftljcqd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bxgqqsta.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3euthgauj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nylyxubu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnofopeu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3njytdysw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihyzbjtq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mwgnrijh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3miccqekn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vedqysoi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ziqulpgf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3drubbmns.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xxkjxaxl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jotxviqk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnhygfrb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ngcfbvqd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uhxaasjm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3eanjsrus.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eubberdp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwqbmqvu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fqstlebg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tachxfge.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lmrnfulv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cjquwrlw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkgtzkuw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zgwfcaai.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xmkeqede.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dzhpbpns.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ldedtenx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yaickziq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ibrisfbt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3skfnunsw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tlfcsuel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dftwyjdb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jwbobrxy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjmsedgb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftyhamss.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3obyurvgh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zgmajrbi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ajzssuhy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ofrvfmhf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yiykxhmv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbposxzq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3suhitigs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gfllohew.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vaknnndj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efpvgdcg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tlnaytgf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjukrcor.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zxyfktlz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mgwgbilh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3runiiozu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3urhqpzon.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3aovtjnva.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qjzrfjtm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oggdxhzf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yaspezzo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kozwmttn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nphehgwr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wmpmfjop.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wxzeyknh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cduoxbtu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xvetcexc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ybwhhdkx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3crxlzvuc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wavgaolv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jehdbovt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3batbaszb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zwmfpznx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hreewmmy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3laehrrlm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3odfrhqlo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lnilvjur.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ijzfmnvc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dbldlmci.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hrgdnbdu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lsruekox.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ftgkiaui.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hoxpbueh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fbhttbay.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3iowhvkqs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hdtoozhq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3qcriovrc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zuuyconf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbybotw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mjigxzzm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kpautujy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kfdiltth.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dvulggsh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xlfiowuo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3szyekybq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yijwwkph.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jicrstng.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xhrtrhnv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bxohyiot.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zlqamjdc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3diqsptcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqszhmtw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wjjwxxjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyilsoxk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3endworll.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lpzrrgxe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubbvglbn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ojvingzp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrpuvmb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3opvqqhfy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilaqoxeg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sclbbabu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cjxvckqb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wnbjarfu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3iyjdpnka.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qamzlyhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ysqneohd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jndhsdvp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pvibtxko.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmabexto.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbwhtck.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfwzeuaz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kjdtfhmh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3nycmofuv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tfufdhgj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ucdqvsuw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xczcyfkk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3xxfziohi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3buxfghmi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nmzkdntl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3bwjhiyxc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bmtgfrsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wwdbhsbh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3enjbnasg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3agemeivm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zaixzyxr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sldwlmqx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bvzdcfga.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3huaaejfm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxocetw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fkahbwzz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3rywdpyzm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qnihpqah.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rgrmryte.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3skckugnh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3djqvptld.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsjswrb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3awmtgzkk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gcxfvcyd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nvisrtty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rgqwmhhj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3iygkobso.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ksrgfwcp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fuskhjmz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bwtaxolw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tfzmxxra.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3nzvuajso.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ipruhmsw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jkzgqbgl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzyijhq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xzphekds.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3uvzcfnvs.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dclkzxph.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3hmstiknt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3scnymkxo.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3glsjoccl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3rlsskajb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vpkvinkg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qdqrqers.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ngdzptfl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ybelsung.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sewnhynb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3msjamnxk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ukevtuxd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3iarnwucw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dvjqcrji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljtfgyrz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3xietbxcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoautseb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uazdykux.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ifqqzwvo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3msugkxhn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3reibnbme.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hjtktulj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cdzcyere.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uzbpfwwn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zmcolycr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3cfikvset.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gxiwxjif.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lgthyhsz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3exlpskvx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3nhdcufyc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3pybsapbi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3yhgjxopq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3yehkmesc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yuwsauct.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3rkfrcaeu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3bvfqtvie.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3cychqyce.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3mavitoij.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pakmycaf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qwjdjnjw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vnefhupq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3upanpvll.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3riasxkti.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rjuntqjh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ubatldxy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xegpumhm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3kxdjxbnd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3gjdudicc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3sdrxsjud.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bmjskyff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eomebsgu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxgedee.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xqddbuyc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3bbiqjpfu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3idlcrwdr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ukgkgfja.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfbrmfg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mswrjtkt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nejrlomd.html


<!-- 参考信息 -->