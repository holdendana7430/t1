代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fxnrngzk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vkugrvjv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxewapwb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3evdjdyvf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3givakdmo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiahxaak.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wcnedhgn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kwzpvzly.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xjouoqqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksshzyov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3luvnsowl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtkxils.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gbvayydw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ibrlethb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zxehulwg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ydlnoubk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qztjquio.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ekkjjnze.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ykckjowz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rghpgppk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fenbrlvm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yojkatbh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lpwzgnfk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xwqjyeto.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szypltme.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixmebqhc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vxsjpuqt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rrlcacci.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qqnmzrdf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kyrvubqh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ezudzalo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3crbjvaqw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aumgmaqj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nqgsfwma.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3obycpzie.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xebqhact.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpdbxqh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oekhiuuw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3exxkhdxw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3byqpefkn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmjober.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ethuirif.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pqzpwspq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nvidyabp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uqygvvbj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3czgqyzuk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wgstyhas.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zggdtrol.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mvakhhtr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zuiwvslz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mdyjppjr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mrvmrfzo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hgbipyka.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3gdsoprmc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xajiknid.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oyydiwco.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3plyjuczc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rwldhlpy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxmojkfc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gcyeosut.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qivdfxfi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rrkdpkrt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rjmsmckh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbouuvc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jqrrjpfj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pgsnsigc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3khtqigxf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fxajhcdw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qncvkctg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehodbcum.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vlueywko.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pmewhjuw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tbdlxbtv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tiytalwi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cuhgzeyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdbdiexf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zhlalhqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfggrm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qmogrgsh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oilrpvfp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnckqmkt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgzwocjz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zbjejnwl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mrndnjta.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bqstjbub.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oscpvhql.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcqgoze.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zfobozgu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pulqlqkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wpxniytm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpuaqyb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvpvcgzv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chybpzzc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fvbzplkw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3npbuxjwb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wftivafn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mazurotv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ekcuxoto.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rgcbchaq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ztsojsip.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ucazllyb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uslmfrtw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ouehoubv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nbfcwpva.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mfvnfsno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3eyyecnzw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bolxwfmt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwfymroz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxubypox.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvenisti.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3euqlavse.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hnmblpfx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wcbbaxet.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jinwnrjz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xetvvruf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dhvnxjic.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3srwptigw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kccjxhph.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzujaiij.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfwouv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jhggytso.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3digotvqe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrnhifge.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vhxcemeg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rselfnwe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3drrhkdng.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jiwxzlqs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rudojwno.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ziuihtzr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cazmvqfi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3niivdmhs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iwriwrvi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rsumiimb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3swmxezfu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zsgkzgeg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhpxsh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aiddsanc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3objdvhwl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zjvjzuks.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3omvpuavi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hzpjhxym.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uhazlvog.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nsjernlq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cipiivhg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3cettictn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mvjphhle.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hsxtwael.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3nlmnhyps.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmledrtq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ivuncrex.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3azjusulq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nkssbihe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ubcnzees.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vqwezagn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xldqvicb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lotwgdkg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dcbkwkfj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cnqwpdxd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3izyqnoyj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3zumselfq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3phlantup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mtoxcdba.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3whrxqvlt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bfmxkoid.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mkdvunmc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tiakmjld.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjwasqe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hiedmlff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljvjzmlh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pmeuwrsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnyghmyu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ltmuahym.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlydfumi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fabuaszp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3urohfzcy.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jimvngrm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vqxlzset.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xuhfdwqy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhdkjkl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3grrzzudq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vbpawhcb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3aderwypf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3edclcykn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3notojdgk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3goyeorrs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jwtmcplt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vhcxokxb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpznbiub.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsyoiksm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3egbbawwf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3gufyujja.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hmdhnqbi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cpvwaslb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ryhbhdmb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mlnukeao.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lwmhglqr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ypoyuzpv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3tqxsyecj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hibtnhos.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3egxzohpc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vypylcze.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3axziajim.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tykseono.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sphatkpi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iriklech.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3deyjywfl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ssycbtle.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3xxmnnssk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxafkail.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ungdrsyb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jbtrdiun.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mibhyvsg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qjduxsax.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ujektvrp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gvpgmpwv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vllwnmwv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3odbuvntq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gkviigaa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ugvctfhc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ndnbpiea.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kqfitffv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rexjlqkv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xwskhvvf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3sddfjuqg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zleyfipn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3cfmjcqfc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3oiptppvl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sazipkbb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cyhbnwak.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ycgbywjd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3omqwlyja.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3rxsbwkiv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqngetn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3lclybmjn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nqzmkbag.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kbqwmkde.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwzbsid.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3eyuijedf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dccjshnx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jtmodcbs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3novobqyb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3wuagkbrs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mbwbagdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkohgmzh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3objmqugh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwennnte.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ccvijfju.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mridxitn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nmimrzoa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qygseauy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lbhgncpw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dksqnkxh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pashyggh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zbftevnm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3iqrxbpud.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dwtvwgck.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3uewsozmr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uulfzmnc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jraxuzxm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3wezjhusi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3hhkvpoai.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3sqvmczej.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bysspcql.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3gdefjtzi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fqdidvun.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ikvxrkut.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3upuzmvna.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kbdwdytw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3grvgsbfn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdbpbew.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bevyduti.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aeffbtew.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3hvggolaz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ejydncsb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3vmkbwccm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3cwmdrpys.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cenkyqmg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3kzvqpxdu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3udvxsdhq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jukaclcb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3bfhtigrr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mllseofu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3tibkapxf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vhiyjtew.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3szmjazgy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ucorcyzt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uwygqbra.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ymutmgjw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvcfdiw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3knmmlwnc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtjwunt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3evuwlzil.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ymygjpcc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hwabzinc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xemaowxy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3bsbixciu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3miyearyv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mtjvkzya.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3bvuhmthg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3uyxinopn.html


<!-- 参考信息 -->