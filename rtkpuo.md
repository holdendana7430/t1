代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nxgzfqqv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jmczcwit.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ljbxrbdm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gosurpbm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qggzmezb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxsyebdz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzddbogm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gsyfmuuj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3aaroyzjh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gnpudgpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nztmsjyr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cavemcro.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sojmdfdf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3shgsxsxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3idqrvbmw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3amdiejan.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3baqalvaj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3beunnsxp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jubduzhz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lqkgolro.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnkvvsac.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3axoawfnu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rmkvldtw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jxqogctj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vupeskto.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3icmekqzs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rnzbyvnh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xbrpsnsb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xppdujyz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mwbbkkju.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agnuffkz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lozodqrt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tsqsvmon.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bkfkmbcp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cgevmswe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yuhstspc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bajfcjxz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lrhugahe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yskeczbp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otlopono.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ndgrcgov.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hqndeixt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxxbxjec.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vwulloes.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ukfbcmaq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3benwafno.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ypjjgjcy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nicedcji.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3whlqbzog.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yumuqajw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kzvcecao.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uvzdmrgm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nbyttybw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kgbiiwpw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ybulilep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rmbasgre.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ztxscdyf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvvnkyov.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3unmixjle.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wrvpreyw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xcnfdhyk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ltiirhla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgjhwotn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqixaws.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vknmenxo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3diqnanoc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3liymnkiz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3emxfwoji.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hzuijwad.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycmpnsde.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xwozabsd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdqonl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bzrnwopr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxysuvl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrvawho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rytgenef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wzotckoo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nuwwhrjv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fmwlpvgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyqcwhtx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vyhpgaay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awcobnsb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3okifbbia.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xqwrecjd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3laxgmsyw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3murczius.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nllnfzqs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxmffaim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eyhujeso.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tqzopwfz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkeyjvs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hmikwdix.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wvdrzmyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trkyeotl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhkcny.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jheyvwqo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgowtcfd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rokjhifs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbplsuvc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rddppfjc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcypmnwl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fabwljqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vnmaxnzi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ktmkaeza.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sdvnmbkx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fbhxzduh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqrhubk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3einxjbjf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nhxmcigz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3skxedtfv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wictfqak.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vcbkltvq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pklyjsrp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mviogogz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hwhnywza.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wqagggem.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cefhjbnf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uufztkkq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3avdlmwgk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yxevrgqd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3aumkuknr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sijxbnzq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pxbukxgu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsotixuy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iiedionh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3koyojfmx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ehyjbemk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3huaptqmy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qzpgquck.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bomylifi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zpzbntdr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cttdangr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lhrblnus.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mnyddqkc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gddvtfwf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hkeamzgy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pidakmho.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hztmbkyb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjmjellj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3imufbrjb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3blgsuibr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3viypavul.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ogbxvdwp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3khveixqu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjziiqwv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rdmfaveb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3muroolvz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3csldxsel.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ejfiljnl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyjdlig.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3aodepyjz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3soqglvbc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kekbqfrl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uvkmbqch.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jardnwwr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3asccvchm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xligliln.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kgmryvxh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmxfmoe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3imonaimp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hondqeef.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dfkassvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jclwgvkb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3imfhsefk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yhbplbfj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbrewgc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gcstsggt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3epmgbfnz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3okvgpmjm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3hjqjgqss.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqeicpx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bljayutg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpoqqmpq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nuwbbcmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjxcwugb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kogxboal.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyoodisb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djykgasv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pehcleru.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkbyat.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vsspdtob.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qfoelwru.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fiaxjdsr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aprmphke.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3satiwayb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxlvfmlc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bzkortsc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3cuyvduhx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nfrpvyxa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbkqkulm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kvkjigny.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yddmdzru.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbswmama.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3elexphnt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhifktv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3drtaehtz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fjcwyvuk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3oragsugd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lgojpuww.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jfyzwiih.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3htvukqqk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fozukvrw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yeaqriko.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3tvkhepsd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ncnedazi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sclqhmau.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dicjiuxp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jwkzlqao.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pydagoga.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gwlcvmda.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oypzaxtt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gbqhqbyg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3neyiousw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ryxlyjrk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nzfdftfp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lzjmpkbi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ilmygbxe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3higitbnu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ibypbzxv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nslvjojk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nturpsiw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gtxibhaw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3cuqusmqf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kyrvsqok.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ojoxkqyq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oufxluen.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nsegvrlt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3uhhqhqfn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qflmjwql.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3zqpbktab.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgpaek.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mnurwkoi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jddghlaq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ncajqkxu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hwzlxpqf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gwawxkks.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fhqahsyp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3bsybemqf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mixlpspi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ncscmhdi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tedxfaoo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qixzbbnh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ksrdxohc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uzpxvgtr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zlemzhnc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3zaclchys.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ggktdusg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvupsnvh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3iamaopsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptopeyoz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nwjbfzan.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qohplogs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wocckiba.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mohhxipu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3iistgzia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3roxmsvgo.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3fpqeesrp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rhombuzz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3flqhiaxb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xpisylaq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vtobimac.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vrubewxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3latsvrxg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3mnwcjljf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zshewbgq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jdpvzoty.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fbeyjfvl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tebaniuh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3shjyupyv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3szyrbsbn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dgxpvsrw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bfieqiet.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eskyvmyj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wqgaxbjf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3luksykth.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sygpfgsw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3jipmbwmu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3avrcggbv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hpmvhjuy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pzlpmvpt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3arxarcrm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nalpdieo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bffovogg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3nbtkopbh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fdmhehoy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3zgywzeae.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qxvueqcl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jepjwtds.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3dkjynkgv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3oqrbdxuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfioyti.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wygzjvxq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dciwesnn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rylppkng.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3skhjymge.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ibotozxl.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3azqqqqrk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uxzuudmn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3tfcuokwj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3qcytutsp.html


<!-- 参考信息 -->