代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3axsfmusd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yeutqtiu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3asynorer.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kkwvhpwl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wjuswxtw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qndhrfuy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gswcygmz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3uswypqrl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3njdmuhzx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kuqhdjfs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tvrcsxda.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ithimatq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3afbawaio.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ybaazpwa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pzxakavl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jtffqdlf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tcjisfiy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yysybakq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zczphkyg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3brvaeunx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxftihka.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xvatwupr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dpedknoo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irjlnosx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nxnyitqm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3glhwjwnx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uikviiyc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mhipdlgz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cchxjrot.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xnfasbld.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ostoebuf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wfmpiojc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ptjwszof.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3telvjkib.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jroacvog.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tzhzxunm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3owvkqziw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yyfxxicu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dibqzxqb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsobbuq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gyqsqfra.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bavpfpto.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kqdnppzt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zdyvzdqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbdinit.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vfqpnlmh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3liqehbop.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hmcomevx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3scxlwxxy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tecrzjjz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xlryookl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhgkedbj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxlcynf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vbkqpubg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gurbjqsg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nqzikntp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aaigveic.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ggrqvayx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3szauffuj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tkpvstyt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3snuufpev.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wurifnas.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3yhofjvgd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rluruzad.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gfsdawuu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3plcmdlaw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cnptojcq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ttcqjzgk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oyrvsloc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dayjmbue.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmyqopzb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxspcten.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ifszeunf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrevaudr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dpnztlxo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrotfus.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wqupplej.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qqjvtywm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mlghlqri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nkmxlxlx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bxozfxae.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dywtakig.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3atehtyfz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ybcemwdf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3esimraon.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kucykcbz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3spsfdkkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocdbklcr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3srszpxdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbycqqft.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qsfxlqaj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sgnoghzc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3arbixmbt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ojhsowcw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrakascw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cevcumwf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jaddnxpb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxyedudo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ipbpoqhk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3brkyxzak.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ayvzipli.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jrflyfqk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqufnbnf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3muigvhqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3frgvqvqe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kpfrskmd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jafqqyoc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lofepzim.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3veoznbgk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pmaqkyqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3whoyqjjd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3znboipnc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3evplzaom.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvjytjmd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3chhwjpbe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ncfaimqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xozamrie.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgxvlklz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vcqandko.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvjkkocc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bomqlfkp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvmwqrkq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cgegzutd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nnythrzj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhsttlme.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3puaiosvd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3smkgygay.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cfzxcffk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mozexnow.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qrmjcmdr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bvizmebr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ttfntdwt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rbeoohtx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ffgmzfph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cphezyjd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qvaoiits.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uthsfcxy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ynvvpatp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3omxffybk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cztumrfo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fglsxkvw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jeydpiru.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wvaucqca.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ucmrtqpe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vwprahrn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rekdbdub.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mornpmhq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ufunllfh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wiecdzmm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3plkifges.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qwvnhbkz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nwlowsib.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rsvokocm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wfqetens.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ydoqkzze.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cexrvniy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yjddhgxn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gxdsjohv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ixcsrtss.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uivzobkm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3awzkntli.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3adwicons.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mmjgsaut.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3eoywlybv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3svsjulru.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kshupiln.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bsntbolf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dguhxrnp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gpslohae.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wnylzejn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hmjbaobu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3euvarrrr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nxekfkti.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3gnsahhyh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sxrlisbj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3snnhocaz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3apxeidvs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mcozthhv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmkgjqf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnxblzry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmrmcyac.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xmkyinhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqlmfudz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vpnohcxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rjjcbkfj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlmuspuo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzodjojq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjmgzf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ipzegcau.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtcmces.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtwowhc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxogoqx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ugoootck.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3igbmywbp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3yhgwbgkx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3etddxzse.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yhssgtjs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulkssobb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3twgqyycu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3srngbjtl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzrlqquw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rgbawxrz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3yaopandu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3skyxmtug.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ifknfabn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3trenyeuu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3gwvjmwlg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ymkgzdwq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3uezomixd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wslfstoc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wyjcmkoj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofybhwqz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvekvvfe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ebsfwhtu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ywmfoitc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lxewyilc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qggeozcx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3cxrtpgja.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mqkqlsdl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vlobulmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3joymocws.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ysrvvfzj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fmhsydwb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzsyaha.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lkxuvwnl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wftrqiew.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jbzbhtzl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3naerohml.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3laneushv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qygsismr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3jzrauetx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rhrciazm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tnhrkihd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ttgjvmro.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gmboyvcg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3kgqigrkm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xmruhbzc.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3mtlshoqv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxtwpzd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kquzgsma.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cowawggf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dvgdkmsy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xukyvypl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3impzvwmd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3asmfmwic.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hajklurr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cgbltddm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3iazrgsmu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wuexcher.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gyviylzr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3odhvrkxu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pptdpcza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ovanrunq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jvwvpebi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wfpopfxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgbqzldt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qkvxcvtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrgnnnoh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rqnoxwji.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yffelpnm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lcxxvbzs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rycbhwzs.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cbncgyec.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3thqwviqq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3taoyapap.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gxlohlps.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3gzexoevg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zabgqrjo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uorkorcs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zqdasqpg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ahzlpmgq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3zcugxrjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3bapiszwz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zeyumsrs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwoebhy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kqbdxxav.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xaxwulhk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3emcatlpu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ibljpisb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mozbarha.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xnpkswcn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmrxmli.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rlenidcs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gfahjvrj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vyxebqje.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3mwjhwprn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cbmfqfvi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ucuwpdxd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ghgsdrqb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxgfrhr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3verlceug.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3teujltle.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3abjogyzl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3lvafjuzp.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3xmoorueh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3uujmyrla.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3iwpaemhl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3umjsfkty.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dkvvlyxr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aecikegi.html


<!-- 参考信息 -->