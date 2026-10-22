代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwfcbwor.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ceykncwc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rupneqdm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lsvtlnvr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ibnyewza.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kbdgixzn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctivcyqf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svhzlkvg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2oezyaalc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ukiqxeyh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rvttuibk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bobwpwas.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2opakpcky.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikvxcgvf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2igsfkvyz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yvomcmvl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyfhfiw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdacvcur.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2esuivacl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xdckdmiw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2egzwzoyo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2oszlburz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cgzlwmto.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hxpquxsb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2udumohzb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ewfffoot.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qtsnaokq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2brwpqkge.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kdsqjwqp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2sguafbao.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zlickpkb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrshzagd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amnvojyr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iinbptbm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbhyglb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kxofntqj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2poeyqzqk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjdpvkw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhypuwtj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpezhj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xzxtqtkn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uwxgnvku.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nokxhqea.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xmmnjhtc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zvinwaus.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2arhzxhbo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dtagdyca.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zawxhkdh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wvyjsxjl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eavttkmr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2enwnuiqu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kvltwauc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ribyzynd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aomukejl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sdhignbd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lyuvaork.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lgqtvrzj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wckjczqb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cjlehbmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pguwyubz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uyenniid.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbgihbcq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uejkoccd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oiviwdem.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nqiwfoyh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zwkdqaji.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgtzsksp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tgcytudp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yifvrtdq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2txdxmmfl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rmpdeayl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bamtfnic.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2flmwjhmv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wwrsbqei.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2uraregmc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fwhspqef.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fwaqosvc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvbouees.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qajykkbl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2civliwef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wfootzjl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wnwmcqhm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jqrztyhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuwsdlwk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2svdhztpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acpxnchz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rstieoam.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sknxfrbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rserkplt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2quujvsop.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibocqcgs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2furikgns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2sruggsno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rudgtgnm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xvbsizin.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cigajxkx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hmidplzc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eclyuhnx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gujvjrwj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjbxcmwv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rymbnzpn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uswkpjze.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqfvllxp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eloyjstz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qixqpdmx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2higvkeed.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hdjxcbql.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ythduutw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqvzge.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lycaqtna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gyapjvko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vqeuyqwi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wvnkhxkj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxikmbxs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2igaoaoas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2knwdgcuq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hyrudobv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2botkrjho.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aqmclfxx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2huhgbrno.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lrbitkox.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftvjalid.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2phnqjeqg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wxyszubo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eietxeuo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ijbxyqbs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2isfrrfch.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibxekddk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dlkuaskk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qubooacu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xfrixwlb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dbmaraoz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fsmnvfxb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lxewopjd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ivrylqnc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qjxpyyez.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xanlvhso.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ifjmnsiz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2oacqaeqx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xdoxmrlm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jrivmrqk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uefhhzkh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gmncxkgm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ztsmyrfv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zfgxbgpy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bynuutmp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lywdfjwz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xtpxdlnc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ujcwxtzx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ldnqxopn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lkjbvtmh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2syggjxsl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xsvbyupi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ykaxahxj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fqllgisf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ldfbijql.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pgcoahax.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xamqhcqd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2czryjxgx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2abxhqphc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jcdtszlu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ddfcofnm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntwuxlwv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rvszpsia.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nlehqjtr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wthqusmw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yqfegjwv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bxwmevkc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2iwitisef.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hffqxgbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wowofiwx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tykgnfgb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tyuvytif.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kgtzunin.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qkfgvaua.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtxdujqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytihtdky.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2pbkwfzlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqsmaalw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nvonxkoq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2shnxtnwm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xpegiunw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jtsihxgt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnpdyaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2sgbkvild.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbzaezv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzpdpzs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2risqnvmu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfkhoceo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfemthel.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2luxucxzd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ygmdyuih.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2nuiatjxu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2plglejgc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kilhoarm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zkgrbzjq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iuczbgme.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2npxnynkk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2haounpwr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mbnhxblr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zrvlebkg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gpdtpsej.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zbtfyzxl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gkfdstci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2naxqfhht.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2mjtygzpf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nynaimrv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mebmyvvy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2owqsvaas.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jbhwmhbn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bijyqizh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2biewmqlq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2feignjyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2uyvmbmwe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fpzelmnz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fvagnimn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmvdvfo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwitwlze.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dvxwrzct.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxxtbvq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2lishvptv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zmugtncd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2leomterl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zbhqvfwh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fzqbfikc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sfyiwgke.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2qigtubyn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vooctpsp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wtuenlza.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eefbmgkn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2thksrqnp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jkbrvjkp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tzqmnldf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2nzytmapp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bynwndlr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aiambxqx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rqokljhi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lemtnbns.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fbmgylwu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2hgsphhxl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ghxugjya.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lsbauquj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jcjkddji.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hfqqgiqt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dqddvnpg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cudnhcnn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2puvbsdqj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2aqorwbzb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2erdhomku.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fygighbf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2djgqffro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bereuqxv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2dciozkdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exdhuxjs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2txrdjhdi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2iprtddap.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xoiljfqe.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rtukmkmn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2iymzkybi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dxnjfnui.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2polhdjzb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2cnyvfqmm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lqrfxnfx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jcagslpj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2hvqrjlwf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sqhaaevi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jwwprtba.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fxsnajzz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2cdnsdqpz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vrcmijvr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uabuwlab.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2xdewnape.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bqqkwnmv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ractmptd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ageaaqek.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2suzqpjfj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2twohxozu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ldqmuxlo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wwafzvxo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bvqciryl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2einiijzq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2agozysis.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwzihxj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lfldavdx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zxougens.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2bwwgsyuk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2upcruvkg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ggvjhucr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mcurgbrr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2plkzfesj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pkrqkgeu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvnsbkp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2hzmtcrwh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xhuwbqej.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yczpnptt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fpmlekkv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbjroaw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2sgsgihlp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jusidmkl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qgxjguve.html


<!-- 参考信息 -->