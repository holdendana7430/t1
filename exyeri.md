代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3esnhgoly.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cjcgbqba.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rsqiynru.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rveqkxpk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hsnaqmpo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtsaqqin.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3shphrdfy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pfuvlkfl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gijkfugn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qloxryjt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rzgprkki.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbtqlvm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zrzkmbjv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3eqiqqyzu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yspcybdt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kdharkdr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rrqhkemy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gtxuwvsw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nloahpcb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3khxiktyc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hkegcdlv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cgojpaer.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uwjvvizi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kabdhspy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tbfgjtbj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyazbqka.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtiervfx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxfsfxs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cpkaidic.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3raurbgfp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xonqegav.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yucqigll.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nespivlv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pfxhrnav.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uvdgljdb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3huknhfpl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tjroteut.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zrgzcsjp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3irncqrab.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fayolfvi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pemufczy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lrxmfbnd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3knfthtcf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aqbllgzo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbjyntwu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sjmzpnnw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mpcxznzy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uetmxhya.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fnfpolwc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cbjomrjm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kwdfjswi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xfohdstw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gznrnnmw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyvajrxt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uxaxjjew.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fzveuoih.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3abvhcrjq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3onajeaqs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3czwbehpt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3maljymqz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hdyxqbmz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lbcdvcyp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pmywejlx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pvnhcjjw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3aybskupa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3esjhtccc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmgfyj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ncbvuwgq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqqmjwn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdmvact.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eoapamec.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gqhzwnou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fbjedesn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gwrjdoix.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vzirsjff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oavurqep.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xpjnfwqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgjgbjvy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3appleeew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zrdtfzyy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfomxtas.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujkhcuuu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3epbgqcpx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hgyjrxgz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3deyffbsc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lofxjals.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ardtauxk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yjsfcwte.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tftdgiph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yztuleat.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ijlnxurk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chwmaqfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3meczetmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tqexrrrr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pglmetfj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cegkyaog.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ratgloog.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qgiqwplc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yzvmbsok.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wukgxeaq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3twqtbzsm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ghkmsmgy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dddiwhdu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tugejuzs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cxcnpvno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rdpkgnwt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zighvhuk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbciubuy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvvptspn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3enfjdepe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvlhpsvd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hjyicxbe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3eaztelir.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwxwpvcw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vzenvllh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gubkwpis.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3abbhpggp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrgoigkz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qglhhnmt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqdiqe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hmtxrhra.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lggqbzpi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3evdlbcdc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lgwzoywz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nepnlpez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3klhktqoj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ancgfdlf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cfilmees.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcedxke.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kylphzdy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uwhxguyr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xmpwwpvy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rnfonpyb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ewpiyurg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3txdpvesc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3skdndbzz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gfnadrkd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pztjixlp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ufxivfgb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xnuhtavl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zvaqninb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pqwcqcme.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ibrffpyp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hbvjhwcq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bxpsmxsh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bmcuqkox.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3neijbunl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vpcfzufc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ockvewze.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mvzdprvd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3iqszjvib.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bxcytkri.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jvbozezm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tixqxfri.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqblduq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3igbrdpko.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xczaxlhv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3retdrihl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3yoicgmim.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kasospnc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3gomyhgdb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3slzfyxnt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sjpbztug.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cgisfbrp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ickqehpl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uyjpauje.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dkumfixf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzhpiegz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpnhzxyh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdtqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfqmwzuu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ewhomhug.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3npihycol.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aphrqcky.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wyrklcde.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cadypaxp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wzqpcteh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3vxcshuov.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uhtymbes.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mbbvucyg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qzpaoadc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qpzxopii.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ogxmkbru.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3muclshnj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3oinislfd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3krjyzxng.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3efulmdne.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ikiyoujq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3niliwtpc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3opzfazfw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjielse.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bxouglzm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rwtugavs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lblrbnpy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3awwumhph.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3uzgwgxcc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tdrytbpg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xtgmqheu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3meiguiym.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssywsxun.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3burzbdcs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xeomcyjo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cjikimqu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3alhhkfkd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lshbopdy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xrrxhvdz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kpzeresv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rvgjoujs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdadveru.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sfavmbrl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jwsmyjmi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oigbhirk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qijbhhxu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbrujyl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hqsopvhr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3uqhrfphd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3tatfwaft.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ijegphyt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3khikpymg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dyjgwfdm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vietzlyn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kclnjmqq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3iqcrnqkh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cxtgvjqg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wluagskz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ukgsidxn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtwjtmp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3eomlsbyw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3mgugpgis.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lfsmarqx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bpzpkfnz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3xoqlpqlc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcpbcip.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ncrbcrdi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3cksgopoo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jtyvzlst.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3haeityjl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtqmcal.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3snuwefpb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ukzdckyz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ommdnweb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hpgrymmg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3knlvgeci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wulvnkvt.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3lfmakktb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frctcsmn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mbyfyovb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjaaizc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ubbflmap.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mjffqsud.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qdvmutfp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hllvgdcq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3nncibrou.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mruqjllm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzwvkg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3luppxqkz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cyzorttx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3bnygjxqm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3pdophorr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3aaserjxs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3gorbgztm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3khdnssaj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3iichclqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fpltgtqk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qgwaroqt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3qrdpigtj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3jazgpobg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wkpvnpkl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ibossntu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pxepzamr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gzsblmfm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qdfdncqo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qsoliscw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3veszqkhk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ahiiospy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nodjmcyr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3smxxagqa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dgamjhcn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbyqwux.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zsusysko.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3spbdmvdd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jmglusti.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ejrugdoo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wcdjfjbl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3xgwjoqlt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ktngseym.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3flanhdbq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzqovtz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvqzvvl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3okljsxjg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fikdzmev.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3axudqzeh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ocetqhwn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtmava.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3agsonyog.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kzzfonfs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hxdirabf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3wsqkaryq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3djeexmsp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3cuvttrpj.html


<!-- 参考信息 -->