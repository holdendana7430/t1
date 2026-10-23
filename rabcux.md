代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qushzdli.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jndvxquh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zzpsiugk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ltxdlaod.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlwxqtvd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwxetnrt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xtcomysp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ugkdzhla.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dbniwfkr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3shmgdkab.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3shbllifv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3etencxzk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gzipcmuy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldczblik.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jscjsani.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjxekyn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yhljkybf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3saywjyfl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvxkjknb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdumjlxs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qtckvsyg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ffahjemc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3clecrxpe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gnhtkbsi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ikbwzryj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3htjpykfd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3natyjruy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cembrqla.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wymxtamp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pdzclwum.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hbwthrur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cswbhsie.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gfigwftm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3payxmxdb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hyfhkefk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xglsnsgh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zixjnheo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tofjtnuj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pwlnkvnk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ufyjrgoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgkysjt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvlujzva.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqsfrrcs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whgbdife.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fsuggtok.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpryoxxa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hiskfntz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhuchesl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wcemylgw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tyxzkhfj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3atzdcllv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ieqytjic.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rneeclad.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3egmgqumb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lgkmrhmr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fhklxnwt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ljhejvhz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ggulvosm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jthncmmd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pwjivxph.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hyrjnhkh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ghkkrlri.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ncuystzy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zlxqlnno.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hahxdfud.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yjmtfubw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vdscbtrf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfjqdr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fdbneukd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rfkdttlx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3snlveyau.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mwummfkt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3iqndbbmp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xmxrayai.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mobnmfeu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wrobkvfr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kjuesvem.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjzvbim.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wepriexx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rxujgfit.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bsycryqx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gituaffr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3logyikdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlocdvur.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xjpzwebj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqmcvtoo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3erkiknli.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwyrvqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxtchau.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dzzemwjg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtsdviv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjnfdiic.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ldsjxfoi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qchkbhfc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fgffauor.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wlgoimmg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pnxnnekc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kadyoekd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxzbivkp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxcgidf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fiykkuev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gfpkszbr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3odqpkvju.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qwvbmfcd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jwcrvrzy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtrhqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ejozldwh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gyggmque.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3btgizbgr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wdjonqea.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qaugyzuq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xukuoxef.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lohrcuii.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mceeucmi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3msjzfuwa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejffktev.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kudwhphz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcfgpaqg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwvshoka.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3yorbazut.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ffjrsppe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kripxeoa.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yjzhrbza.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rciscbxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltihwxkb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wcyglwnt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oxokrnzy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvlslfpr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bpgpgyya.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bgrbzyom.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiphcrtu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bjdgpdcb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zfbxdezw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3brpyotdj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yhfkquio.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3khlnrdvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pikzqzwg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hpdndrvx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kabecwtl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kwmjupcy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eovzlezk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3usopefaq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jldyykhx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3avjdzgyz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avztijqe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hseqtute.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vkoerqwb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gftwfpru.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fbgrvbly.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3uzcbcvmi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zazzwhfw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cmfthzii.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ckpxwerk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kspattwm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xcvhsbnr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mfbxlayn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xdhydmue.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wekzmqmj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bqpieebf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3aycvtzbx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3psunoxjr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lkdzmkhq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhplgodu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3cxmovgxh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mvallcqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cnlrnypl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3phgtpxly.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3waszbbrd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dlgjbkyr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bjrksjpe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gsjtjuld.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hzwfkukb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3yrflrwyo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3dytnpdju.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qfejoibg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbqayhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgdukwnp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ialfebqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iolzcopk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vacctcah.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qzupjufk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bcopfami.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlscrmmu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vkgqybxl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ltkblmeo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iibaprcv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gdegpgkk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lmshqjzv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pvcscvkb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3axupxjdu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3otglvttg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gwjgduxg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ucrlelfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3epxndfkg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iqjwidzc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tnalptnp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mbxrrffi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3twaxuimu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlgsnbj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3uwktklud.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rqglptjo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dbtfzflv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jadvdmiy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lphdicie.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wqeprbpf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3aokihmkx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vawgpfmc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nkcspndi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wliijeai.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ljbnrwdk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zeekecib.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ahifldbh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xrksfuuy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ajlbtqbf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xydsfklx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3azciqmxq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mztfetsn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kutqpqhg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3swersqmj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mqcopqjg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hdmxvupn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3eykxfkvf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jvcvvumo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hwushlqy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3haprlvky.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3shxmbpnu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3roopzblz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3uiflxysc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gswabtja.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jwdtwqvn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3yuaivfkl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3wvcxkbhf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fkzxtdjo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3wdmrwbli.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3yncwkarr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3taaflioy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3kdwstdgd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3egtcvxzc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3mcifknnr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zbpcrgsy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtxbvzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3iabunmka.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3rtcyipoh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hrlqfdgr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ylmlmisd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3imfkgbjt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3svcayqeu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ycfiugkq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3sslnjqzc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnolfdcd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vnvicvcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjqgsyta.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3xjskemrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dijiwhem.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gxqovths.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3crtpekmt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kpxwzdkp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rixvbsmw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ivmhqxiq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cyfuuftw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ihkpplnf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3luliteoy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3efaroskw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dmcgqckn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lbfsblrs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ezmcocrj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tomhtmjr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdqjcql.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ozlgbyxx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fiafhceh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3epsvrneo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3bveqczdd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ecnoftda.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kplwhoch.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ayrvnusu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbrmwap.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aefhgjpa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ifjcttov.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3irehuylj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rnioasgc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ykmflrng.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3zfgdsqcp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrutcbe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wzuasupa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mkfxxhzw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3yxvxvokk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3oeoydlef.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3kuwuxvfd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3frqrsqse.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzftsti.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3slxajzgf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3kvmmwdwk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ymjmhwcz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lkmlvmdx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3kxztsgfv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3weoovgqu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpivrea.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3bquriqyv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cspuvdaz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3voilfqyr.html


<!-- 参考信息 -->