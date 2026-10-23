代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3auutncfk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lkrhohij.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gontsdod.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pogwhagy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jzrprhfh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmzkqk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rnuugkui.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3divmhlyu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kgkzghkm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vrzimeel.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xivrflqu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjunyt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3baarntdj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vstttrsd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iyewgaun.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vhihwhpm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3omcaovqh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zchpcrrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jfrdybpe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fbkhpwun.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ctwkkcgl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yqtzlvkj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zckaalgm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dxylgryv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3flaxzkjc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdixxojx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxnjmhur.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oxxxrely.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3suvsldww.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3avogllma.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rohxqvcl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kivbnfzl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dclptwyi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgdyrew.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwdetbh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uqtxbxvb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqjswfo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tmfpsgqe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3opcjjnno.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3giiqzrmj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ocewsdzt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3axlvwpby.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dibmhpaw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eioqceri.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rlucnlxj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3llnmxfoz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pbffpxec.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jkbrricb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3asofoyvw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vvrhtbud.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gnkordto.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gkgokdea.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cvrmsjoa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ywdsysae.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lyepekax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ygqzdcii.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ksqnbjql.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gvnxddnh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfusymmh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kbttuaci.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3leesyjrv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwsrxcxi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3plfrnlmc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ljkpnbrk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wsdcrgog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yitijteu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tllqkycq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xrexuylc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vlmnkawi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwhfmtd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3owbjljdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fxskneaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kktopjul.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ujryrlos.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3inbggnhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3leakfuor.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kacjrqrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuufkkyc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yztbxgem.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbcivfg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxzxixz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3idvpyhmh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhyxdpjq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmoadgm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hoobczkr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdkdxcxu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ccvevfmr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mbfagqfi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iyvmbpmq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbapfhmm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iqitfrnt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pkufujku.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqerlbqn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zndxmaeu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnjelcdo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvxagcdf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmuqfrlc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tvawxeff.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3laoxmktl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gziboolv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hjpyfksz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shrztqen.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cphtarxh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bmzepprl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mdtqrcgr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ivbuzmvc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yvovbamx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xhvwpjlg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3thrxpahn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhqtoigj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdkybfhh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pffcqsxq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3plmueirk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3snducgsd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cktvslzf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iawafeys.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3anoivalx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkhbyyow.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mxaunivi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nycidtrv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3peqhayct.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qmjesrmz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldvnbsrr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rnbsxmbt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ajfsgxvd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uryqpwmj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ewmkveyj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qcqrlsqb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpkpogp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xrhotklo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bmocwejn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3scxkizdr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3omcmbftm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3umuoqxtq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uafsohzf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3asnmajts.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zqnpvjeb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bvkcyjmw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3efafkqqw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pycodkep.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3exxddmdv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3akdfdwcn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ervjzkiq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ycwofrps.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3udkskace.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pmducgxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3uytoleoi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jpbovkrm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jylggieo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ydlzmvub.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rqywkvtj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nqzqriov.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cgdbxqac.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3regevctd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3unlkzuyq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3grrmfyrr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xecklzix.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqgzasc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3bepfqfve.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3mhrmktwh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xirypgia.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ghkfwefu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ivatyxzq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hktmkzra.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwshtb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tpvcdadf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xtwuhqsi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uiznzsub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsmmmayf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yxbeiouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwuhhfeq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwtapakn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ufndwnao.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3incwnhbe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tsynzxjk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kecvqluf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3snlaqqqu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rbsghnmm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pedzymai.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ablzlmmi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eszcejvn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3anklqtie.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tkdoavgo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wmthowbm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hftbvvmy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3mtvxpwtu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkekbqyh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gocpkqyt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckwauwgx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3aveoppxb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qaqrqqry.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cygzxswp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lexcioat.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fbwranpv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zlrwqmnq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ybdxldmo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3eihcdnxo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hbundrgi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vmeiwnea.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bekqwkqx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qolwsocw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wkkgjutf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cbyczgmc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bewjvsno.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xpbsiuos.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kxdkikon.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rkuzlwad.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3pjqitkgo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3tsdgbxfe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nawkdspj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jjezwgpi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wiyzyeqw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3emlasqkq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3npikyfsm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ffmucqwk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lnxbuvgw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lkdmzrjz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3npkyhpfu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zhmtdboe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wpxhwudc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3typiikps.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xaphgdki.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3isxncnkk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hnvqbqew.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yvdlqccw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rcuvywrn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3netvfpqc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qvkqpfyn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3lpykxnem.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3viblxyqr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3zecgmkun.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tbsregvq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jprjdoxv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3jzicubws.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3rgtincvw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3mcnmtuua.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hpdmudoy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3igivhyop.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rnsxmdkz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qbufxofb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3jqscojqd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3yyjiotln.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sadmmcca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wntoowgf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jlyuqbod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcdsqrvv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3icnhzrem.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wtquoitp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gqkwnhyj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cqqsmjqj.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3itvprfci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nzjibqgv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zwwpsaom.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3tkkobwcq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3yevjxifd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqikdjsg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yoykjoct.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbudmz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3iamjcrin.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3agqywiay.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3urkgxila.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fitpqrds.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uouqicpy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3hxgojkqt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lfehcfhw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jwlshwnm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rhaiqbtj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yvliload.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dfivokmz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cjjwuzdq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jcmchriu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nusmqpwa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3etekahpa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ngsvnmdd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qksyaqhf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3yszqotzj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3kylelikr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3mxmmuujf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fbepowha.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sjidpcen.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3cwfsjmzy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3agfweoxa.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xayekbiq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xejehzge.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3unveibmf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3kkfoqioz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3dbkgcira.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqtcdcm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbjcrar.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ewdgnjky.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xllubciy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vqivjlip.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bfjusdgp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3vskdfjlf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3iwcckhov.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3pdzoqkuc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yggmuhpo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vjhobxfb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tkkxjjkz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jydddwsr.html


<!-- 参考信息 -->