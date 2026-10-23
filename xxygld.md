代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3phwwzzpo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpfxjetd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hroeuxmf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqzacarv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hbpmhfys.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ofdmhnin.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3antnjhar.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jcpwonph.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lwteonvo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekczyxnw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hizsvqee.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dojragyp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ijwdxgmx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3enfsjess.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hekjnjhy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bvpdmmvs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qeeokezq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ajdehmae.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hyqcyqly.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hfumxsad.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hknumkas.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rflggmpc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bpvnkffa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bnfraubb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gaxrfgnw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3emkjegmr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rdderfji.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkzoruih.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fizvdvhu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdtkfdqd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftaidyfn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bftjioer.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nkoujeqe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3eprrlbcn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xtvpbcfi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xtyxsddp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vakppsyg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zysuqpsr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ttcyzzwr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3weeexyox.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ektznyuk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fypweufz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eygfbhgm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3neorgevv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xmkhclye.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ruldshhh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pakmywus.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xlpvqpvo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wgqyktjo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wwkuwsjv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3egohiglz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3icsmukqg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rivuupow.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hxhqtasc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3joxcgwds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mmmzywzu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vfdqzqcq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltiqlpov.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lexurjvr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nkyceomr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rxybctak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mbgfsqto.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3czhyxwnn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdgxmes.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gpngipyf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkvtvu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hnilszik.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tunybsdg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ggywijdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yzavjjgg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3udggtkob.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bfecotnt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qhwdoedp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dixrzoxq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cddaekrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ulqooksb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ebjmuupn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3djwqwvjy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oxdvtgdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ornytnbz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3epiywniu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsoxytoo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bxksekjh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iqsdlaoo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3aymbmvdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zrgqbgxk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3klulthmk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3fmcivbjp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tmghfidq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hsdikpzv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqskrqcv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rcnoznax.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zgbuetdm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwjavdjw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlohbqkr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3himvaqip.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjglixjz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nokbubnf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wmrovake.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgviywo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3elhhdhdp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3djgeudkc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xulvyyxi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cwfgspaf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3usncqomo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qamzbpoq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cljglzyf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yjftfayq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ycpelyxh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zpcmbquq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hnekltne.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cbnycspa.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nipvlmvl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nnaecltf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjsjwfpz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3klhusnjq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3svvnvenm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3velbqiwk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lsbjgtmd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3aczrdmov.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3doqqgulp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfgbxkhp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3popzbpdh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hrakcmwk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3srvbttkc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mdnvgkyp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btfuvcwv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wcifuhhg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gunuoerj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ywoxlzxs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sxxkjisg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jxfgbcdy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwbahoe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bzzbloqd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gvmuxnma.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jvpqowvg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mtnogcrq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3udqqwwby.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pecakkrj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hrinjbzt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pbjqhmjp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nexvsfxq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hdqgejmp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vfyvabmm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zarwwmpt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3egpayxkw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zvjzhdfn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mmkdxprg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3uzxmtyve.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3faolnhln.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3crpwpfzg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pneseffd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cieadrbp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3belgskyr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ewhhipyu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3thfeolji.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aydfbfhw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hzjgejdk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gcyvxozm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3upvhlpfd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cbizntgf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfrawox.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ivajwuyn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3bcoehomi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kvolnbka.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3oounmfel.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yexmsays.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jwsaolmv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vkzteojk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xklzslbv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3aqzqfvdj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eugbvijd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpbhzrsf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qkoatzru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxmtrldl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iztptkhf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fgcbycyj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwhhpadp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwymkpbj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkoutpzp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bacciobx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3olspzbol.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsamlxg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wyvdxitv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cwfrankn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyysigr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kftyvttl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3nwkdlnsr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3thqkkusx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzpsrlhd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3udhujezx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ntosjiaj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cmhnnddj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3azbprtsl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfphvpri.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cnpxaxiw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3spyfvluj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwqxqt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3nwsopwqc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xccblusr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bcbfkfav.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rhqnjtmj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ufogsguo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nqdkrmdo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvgephur.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wgaagxsu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fqhnoiwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3knpjzjhv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ioldzivs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iwiqqrmx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fimkjjyl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3nvvzxxrn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxorypcg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mdonlvxq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nukthovo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kfnpsfxp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3znfnykzz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yosxzmce.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxcfivy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uobmtuim.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wlkexwvc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jalsbckp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3cicdgfli.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tgeewmzh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zkxiuxti.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jntowpps.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3lkfqaddc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3elfjpyto.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jmmitlmg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kjkcdkef.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3glgyauzl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3baiqvbke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3pppilgjf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3eowrgcwz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jeoldjuk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3tcxqhmgi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mbxqpdgg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3celwtrew.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3bersqnbm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3kbbpquzs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yovdswwy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hfpebbuw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dmtjjxxh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sbniahtn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fpbsqfhe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ibywfdnx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pdesiqef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urmyqjgo.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3jkqsompc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogkwjuwy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3mvoykngq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3oyllnemk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3prndvidz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmwqgo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bszhbyjf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3rtcusxbb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3louiwssh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3bfrxqlet.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3rpnknyvq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vptyfshv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rawkyefc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3oxcejcfi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ybxgdbpb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bgjetkbn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lnanllqa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3tdaooxjt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bfyxdjmy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ztoktgfx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3swubnosl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kdfpmwut.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wuyzrmuo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gstifqlg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xoigokiq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vnycvstn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zuzdhtnt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdyxltay.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3brtiqabe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3yffjgmgx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3utdkfmbk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gjzzzbie.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3dmixldmh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3majoaedm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nniekjbk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3akiipivo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3cpnzvaon.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xuqucmee.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qjxtcola.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gopjjwai.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pjsgmekb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3oovatjjy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nooxnthc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bckzwmmr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tldymxon.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3wnwvoffm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dpxmfhpe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3oxmijmar.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vjgppohq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3vdztqxwd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3tnegxccr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zszyvfff.html


<!-- 参考信息 -->