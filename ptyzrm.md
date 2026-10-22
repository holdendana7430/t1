代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hanjndcf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqjjtvbu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2acgvvydc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gxddslqh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lcqgdhoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2spvxdszo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eoztjuoo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ltjhfrdh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2byjzqryc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gtrmctkv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yhvjvwko.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ffuedryf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zmpsogzd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rfrrkbmz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xprqasgg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2finbwgyz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ehvqciqe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2togyinmm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rtzaikxz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqaijjj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lhaunthr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iduqnhrb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxezdfeh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lqmiihwd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xpyxyihc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyxouve.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2abkbsqam.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2whlrhzuy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lfroofyj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hovkfdql.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kwflxatr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwoylfw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oyxkxcok.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2urldfecw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jpieshgt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vsgvkxzx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wkhfbclm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hydembdq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xofbamkz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mfflnlib.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dtwtqfrp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ilbhkybp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nhrpclio.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wovvmojv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yitipeyx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dkqnnriw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2goxozuhq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kkrgavox.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2oenknygj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okvxjvmy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2szcqxvoz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fmtupgny.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ikiqtyoj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2saackhqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqxnvwtv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gustavdw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wtiyyltj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2abcwqcgy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gytzwefn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wbstfmxv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ftgbnkkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvuigbfh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rhvjqrfr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2shwwsrmg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2roszpsjt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxsndeys.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgrwurax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zeugivzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xjrjfuii.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wmarpemp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vpnsjixh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxnmjfei.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cgpslyxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kszktnui.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2okgegxyr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tmdknaod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bzrsgbft.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvzmiuh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dncannab.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ztsojaym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2onymwrrz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qsqdqzst.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2unerhqcd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pohwmdpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vcjeaudt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2avamvfmw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgpiaoiy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cfldqzhk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtaajwuv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2npsaqqhk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kaasjizp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwxswdpi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wgnbmlsa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fiwkgtpo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ozvhiptw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ixtejnlp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vpvmqhds.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svrqfprq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tqcmpipl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xirnycer.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qftdpelr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fapjdhuk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bdiwzpwt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sallsseb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqlzfzic.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nbcjfmdo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xeielxao.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eixphies.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzfjbkgf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kvwiusgz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2twdszzto.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jhjyzamo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tamvtbdj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mnedjxuo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wkyivqrb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gezlnvjd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zbbsirdg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dawogbmv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqvvqofi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zkacunhg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xhvfplbo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sjkdqvoy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lafyugve.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2amdfpqsq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ljudojfk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jsrtpyap.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2cqvpilkf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mkgbmahf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tgukgtuy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rcnmhvfy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jmosekzx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqccutva.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zgcumlzg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2khxqhmkw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fudigqmp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2reuoqclx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2levrzyxx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2macfdepx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bmrsnqug.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tbtkwdih.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ezgcagao.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kmbxajxs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ubiopyim.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ptzosoyv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xhcllrqw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2iuikjrox.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ollqzsgj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mcpcjzfj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zsraagsh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cccqzsiq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tbfzfdxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qgkmclrl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tekxanti.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lhxxzbkc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qmtxizte.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dtzulfpg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vngkjdlk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jnpvcyry.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ntihmvaj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2orewhngt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2janovyis.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bjhiolpr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2azzizayt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jimcdhbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qimlkfkg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tvgvsfti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icyplmfm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ihpesgsr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fzguboma.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvjnnjqo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wyuocjay.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnzqvdco.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2psonbdae.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jrfhyalr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lelsygbt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2guvaqzge.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hqgqjpcp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmtrfvm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2aqrmjkms.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wrcnmglu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2onmlhcrn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2aewyvyjm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqnxcjin.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ajvcdzmh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2moxwhsaj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mpkugazx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2bbdwayjd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2adocntct.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2idpzwmeb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pjsxijng.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rptsyfzn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uhuquebk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dvsofdsv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bhotunfc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dgsitxbv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uxikskrf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2abjdiwwy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zblasopg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2byxiinum.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ajblrvgz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qcicpfgx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2dqygujao.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kjpgvgxl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eykloaxm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fvtwufwd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwupmwwv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cgszwrao.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2voccfsis.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mjgvyjcv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfyzljj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dlqpedtk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2alpfglvq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hyrgbtls.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gowledgl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zqqarlnp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yalikkwu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bglfjxzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oqsludid.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xerajdpl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2rzirwmay.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vsvhaqft.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hdaamwas.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2psyluzmj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ztqbqofw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2kyswqaku.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2omigknll.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zcibdnya.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sdxlwyia.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cpqadwim.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjnrupb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xefehwux.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rlvqodkl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwiofyo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2blyacyfx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vrhhvegi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tcaplneb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qiwsryve.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ewghmhsm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ibiosyak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyvtttxr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2lqzkexja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olzdrtoi.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eecggdui.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2arcaybxh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2eqlllxfh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cdxzzikc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2awlhniex.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zqvchclo.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2bhscrjhb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2cyonbdfe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2yipuztia.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2enndpxef.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rvuiffsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ytmvcpdg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uvbbdjkv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vkbwqlrs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ucaxijjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2retzmhuh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zlxwwumg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcbqzil.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2pevygdwo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2azhxpvkc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2imywpocn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ozuvnmnq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bqgewgph.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2akrauxju.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xsecycxd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ufsglyfv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lsrthcfb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kcppoldz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tpnuehch.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fptjnhen.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpcbknz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2orgadfoe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qldzmvab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbwlraw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qhmfhegb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2bzqxqjbi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2tutucabj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xzfemskf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ptesihuy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yffyyaif.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtlnnue.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hepgdwzy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kralzjwv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jyzhqdge.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2dtytsmbq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ctkzgglr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvntpm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2liblgiln.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2eqrgeaac.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nksgrase.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2whogeced.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2eckzphoq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2csldsixe.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nxbsqomg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mevulbzx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yprigxeo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jjpoojoc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gluldejg.html


<!-- 参考信息 -->