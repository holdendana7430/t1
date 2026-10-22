代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iykuhyne.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvaazbxl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iloqmuzj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljnuuibo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2exhthegf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yvacanym.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlcwhqmc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vmeqwcig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sdziakda.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lhwskzpb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xxslgmmj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhrvzzll.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2snyeafbd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfapkud.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vhyknlnv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amvcomvq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yaqjvqvx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lhoebzzh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qwyocefk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2smnbybnb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wnthzccq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2edpzfoqc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jdfiomdj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2obpjaenq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zgbxxibw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vncazziu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xwzzllfq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2usbramyi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2awjjivif.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wehfwqgk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inlnvkbv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xputeucs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cmpfpatg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mewpjgrk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vclhyevg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wbjcrmol.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppfxdzdt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsxbqtzo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwrgkxpu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlgfnstu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wweqoktg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2luuvcjsr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ppfhqpgy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2btoglnoy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2apengobg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hwfcpmqn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vhfmyngx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drowsinq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cjrgqbdl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zwyvwbvm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gquvcqko.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ptiugmun.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2elhanviq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hghfndnm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2crvxtyzb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rezgypqk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ucakpupx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tvgheesn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xxuwltna.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ecifbrmj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ylaryzmw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bczfljjc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2khzpxorw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdjoihf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kmgcqwth.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mttcskkl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ddewzhlo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtycujn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2afuyrpbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2utrwcmtq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dgpmdcak.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2drszdygf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkgzhip.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ziassmqn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvluapx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pmcdwtbj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sgmlcffs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fdgkjkup.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2awccxosj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glpkrgew.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rekkxbhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcsihf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jsvfizxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2khreudxm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mnjcaijc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2flqwssqf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylejnglr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2yqgrkafi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2eecdmomg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2irovzsfq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2keywqqto.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ubuzjupr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oenmfocl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uicuzysy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2haejuylz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2egthsmjh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iimynlwt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2woxkahdg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jdeojnjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bciuovrs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nisxtabo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tirvqizg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2srbdloip.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ehunvwud.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2phankree.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yrzyfqte.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qjashiyb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eotocjgy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gjuruecb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2keqqqwth.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rokpqoxm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2otnrixap.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypecdimj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ssxslgxg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtnyfnki.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjslote.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxhepn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2oimyukng.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfbtinxq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gkgdrvkk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cyqreczv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iowimtrc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gffceyed.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzxlzhox.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ytehbwxr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nvftjeit.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vcwdhqqe.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2eprenkxz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dkbryxft.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ztnvosrs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qqvisanm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dkbjxoxr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2odycmtwp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yhirdngh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gldhnrvg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2shaagifs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zatjfxac.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hofwgufa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mzsteded.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wqcgsotv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vmeddmcd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hqcyrags.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2snyqvcin.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zbvvddbp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kutpzcen.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hrwkreuo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xwtjlmqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2chtgqcqq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2mkuzceqk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rdfmhmag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2eeezooki.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zlwhhvtl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ofnviylf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ayxdgnku.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uojupjfx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yjimjluj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jssirdzd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vhrqtefr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qgukztwk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtebvs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iirasbys.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ghrqbyxx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hsttjunz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yqzdeycu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wmcwrqom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2abkwwmwa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bphrxwjb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2skurxbwo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oxbbbwkn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2uvzrrjvs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gvzojqrz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kfvosmua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxkdckkm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qkmespuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrutgqwr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rgpmcrbb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oacjnsic.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wxbudiog.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecamcise.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tqcdkerh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2mxqbqxgo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2laabtcpl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2scfhznkz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jgftgcri.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2woaewpjg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jilctazt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2udwzeqva.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lxegaeje.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rnkaaoqv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vlptbcss.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2voarczfb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jmawwmws.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdjnatvm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2oewetuks.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imgovyro.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bgzqekcz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pomujsef.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2scvwbirv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ufzllnqi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2rpigmeio.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gwhjumim.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ynrjhtba.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iecsflnr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2biarklmt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnhsmvwb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2udaexfsa.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xtlbcvgt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cqunosln.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2becvttaa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kfvkkciy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2taxurkqm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hikttzzl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jgdxvnge.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ueceiepl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iqfopfvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rpjkomjg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2eovghehl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2maykyfde.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xiayqxcw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2todygtkp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ktazqlng.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2goinajxj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2okuodvoa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2glimnhzq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jjhxechf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zsugzrgn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2buydeden.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2keauvxhh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2acvggwnk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qcdlirjl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ytrbdctn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2afgoozbw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2jjnzymvn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2yjsktxzm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2yimdqiof.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zahkizmj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2icbhtiur.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlropzk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ckfdwndj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zmjyaffv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dvftsmxs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zeqbsswx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oalhztyl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uiizignb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fpietshz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2evzuzrub.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ozscdjwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bulllqnv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2pijcpcry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uowlvixs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2caeayemg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2pjfevqed.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2taotlamz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dspamqfi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2lirfllpi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bzapsdlw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ouwibggf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2pbolusng.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2srnrhbgk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2brfzljsi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wgsojnmg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2orsxlkkm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ismiuqzk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mkuphvsl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xaezalui.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gqwvxzkd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dwnozsos.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2dswawwtv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2uagdrjzs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vbvbkxoj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ldruylhl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2anepntum.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgbvfyo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vtilwfcj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nnoiwkuc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2foypqujq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xntcurnk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dbdlqowl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pgiqhrlc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pqgcluhy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bfpcoseu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2rcjubddk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jwxqxkjd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2edtnerin.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mfnozqzy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hjdkqyqf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2luligrwn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2quzvhvtq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2oazgrzgq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2thmmcwcf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xxnjavuq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2picjsmzo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vzaesesl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nwhouelg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hznpxtag.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wmklgaqj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vduscmuz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2qlfstmgc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ydupsbbq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2elgjbagj.html


<!-- 参考信息 -->