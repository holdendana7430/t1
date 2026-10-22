代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pmqyvbqm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zdjkodtc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hetctbrt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqmtzxxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yxrjdkhy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hbandmzu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsffdr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jkfbdspp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vyuptpdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhcvyus.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rxwkspdz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jovyamvq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqtmsegc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ysnweyze.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fflgjexj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afzpwgif.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ibkmnkfp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lgfolapr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2woptcybe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rqsthtzp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rfjmldtg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uwsvedsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mhwmrwap.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jebhtsym.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hgdrabpc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cyhvowju.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hknhumlr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddyrpcgi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qrvyytdt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpberuhe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2roulllap.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2adildlyb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vtdbqzke.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kubbnudu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qmczahsy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2iywfqmgo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ftssaqwh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtisfju.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkesetsb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gbrqcysp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tdwdvuqy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjjaadgq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hbbdwqqg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hpbpyeis.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2osabxvmo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uqbnleba.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lpbrddmh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mqjfkbxz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dqingcuu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2utselqwv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2smvfrvjv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hkywgsuh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oguvzxkj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2chfzlamz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2funpuryv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vsemtzhu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wbraojaq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jltfuwwg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vhiowypu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pzvwzeww.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mxhvkaxx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dupooegz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqegvuyt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ulysrzmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wysrwuoj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxgrqnhc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2trzmgmnj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2omintfjk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jdycdwqp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2crgvmvpe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tbeszstg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yhtyeuja.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ftqdiatl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwaaqhlx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ukqomfty.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qchptgaw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2eohwidjz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wduvjybo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hfssmomk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nemgihgu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sjgimvwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmombkyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2swgljqvx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hoeacgeq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxeefeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hrmgnpla.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnyfdyd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2golsihpg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pyecxzsm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzhdnglj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2prhxfdtb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2crnaoxna.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2oouwkijt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbmqml.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qdhvadyr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uhconpzn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlutilyq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jnjkehhl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2elqqelug.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuyohemi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2khustakx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sqsqdjfv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xzwkvbrk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2irvrrqay.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ctjizczh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nnnrckwx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsddela.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2oepenwfn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zzaxsiio.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2laqlghfi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cpyaffgb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wouevxjf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dvyghuhp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2natqkybt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtzqcada.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhuorm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qhjtydqd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xmflwfjz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcashhvx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sxlzskce.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yzoqcpkz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fykqszqd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yxqzryry.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2asarlkol.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qlylbfkz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kaevypik.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khjxvzmv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2buaozczg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cebbxhgm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vbneeuyu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wqtpdeob.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hqhuuusn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ujynktpo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jxwjwoxk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2juaedynt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xajahufq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2iegrwiuf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2sclfemrq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2knzvkmpv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ujxoigpz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pxadrnyw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tmaobjlt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2lsxlneww.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hlrabpfk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2elomfptw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lfatgwnz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxxzmp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2sjootiyc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cegyyffh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdvqiei.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2psljjkrh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yotdhowe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kopvaeel.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ywmvuzkc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2tizcjtwa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cotjivzb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2huvzszza.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2uyedigwv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2kwcvnets.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2utqobjgz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kpzrgdec.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxamjj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jscgmhjv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2upvfdfpt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2oaekvabl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2djlpaool.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yyvkrqca.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2twuufulv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mydmlrjt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cwsqxagl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gyndmeud.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ofurnxzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkqnzdxd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2icrnlxzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaxctngh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ynahangs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fnmlmogq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkwybdea.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaygeon.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xkcdtkav.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gavizkro.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbvmzjp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uavwhdza.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hrjdynat.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vudzbgay.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kscodfok.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2zqtclvvc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nelghqqv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pjmobopk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vidzmeob.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lhgtnhcr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cldcrbqr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2thkhyrpw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2zemvhcne.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ztmvupxd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tzmpuunh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sqntzolf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2elataavn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2quehjcmu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jwihxvbg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zunujmdn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vbvxldpr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fwsvduyw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2flijwieq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eiimyjcm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wrfspvmc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lkrmezze.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zwytonsw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qqzyevfb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbrevdo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xtejsvfp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mzjonguz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jwovvhiw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2egqirvqc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lmkaaxvq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2klvtzoyb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dsngmaei.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2osuctxox.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nkuolcof.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2sieszvhj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2uenxqefs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpydue.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yrxfdnou.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kduykheh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uillussx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nddzjbwz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2uixjofbs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2bvyiebkt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ngdkqjgt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fykpexhb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2uatrrthe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ftolijvn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrmpmyj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jwaikssc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fozsdqrb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2hewomlfv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnnqnvg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pdiogrsw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2etkmsohp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xifiwvpb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qtpwohom.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpeixnw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jgvknnxk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rkdwwdog.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fcjynfho.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tomtssxr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2azdjfjrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxlsdo.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2kpbwqzph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bviutmdg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hpozqbrw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2obciirrs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mrdlaxku.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dfwzxztk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxhwdc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gcpgjrdp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2fhfxvoxv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bzippcrd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jzschcmf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bpmcykgb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2smvzohff.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mielklqu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2udialqxp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vmawgrqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dnuseagl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rbnyyscx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bfkuomph.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2mlgxslcz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2xohojqvt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wdlmdaru.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pikafhls.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zzjhtsxd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nasganjw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kpvrhjcl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2svdbldra.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uaadjtwa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2hcxovawa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2yuylhdys.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hkzwbydw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hoamxiac.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwhssu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2qmzmqmsf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2usxjzgnx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2hqeyrgod.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rbavaswz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fdyirhzv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nhwzuwmt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kjcernpq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2kdgufbbe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kjyhspci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zyfexxsq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hpitksuf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iqailigh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ujxcbcjz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kplxgvxn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2zglvtuwn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wllclshn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ckzkbcsj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2mgbcsnjd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qgqmqkqf.html


<!-- 参考信息 -->