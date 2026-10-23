代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3sfuuakqq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzehjjdf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nqxchvak.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lwfnwcae.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kzlwrthx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpaavtbn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3eolhtrgb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hnxeiddn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zohedqjl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmwwocl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbprvlwm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hogxaiyh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vyrnafot.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hxrngtjw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3noygwira.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hrpjdlnp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3egjvheow.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zxnfrpui.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jdpdambm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vvvzwrbv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uyrodunu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3izapnovq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3syyqdxri.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bvrfmkmz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nblzaxsh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rewxzuoj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmtwftab.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tkctrmim.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ozbzmewa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3obrrtzbk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3yibampiw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oedtcfec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbrslmon.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnmmgbka.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nlqsxsvy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdumkkmm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ryjicchj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nykgjfhn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mmiminox.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tsfxmhme.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ptrhpqsw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3koswpgpu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gvcvyxkp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3curvaarf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nohfswpl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ppyeluit.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3thumqnok.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vcgroozg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vnkcibjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ypocilah.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3azujrlkj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vzopxpud.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cuxornfg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyjkcakn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mmlrxwof.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jhhnzkkt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ldasqjev.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fiuzgurv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ltclcfgm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqnrajoy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gogmpwoh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3quowcgcj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ccxmlris.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3shiawzzv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nrafxejc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nfgdsadk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fsvojuca.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qlakfjar.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mndqwbdd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3crhyereu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skucdtod.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mevtdecq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jfziaqlz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3chvhtldn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gudqrtpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmtgbszi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3duvsokqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jevockas.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mkuqvqfh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bmtralwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrqlcinq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qnrppkgy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dttfovte.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dmnvhunf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nolvthkh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lbcfvlhf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3efeewvwu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vjswgxdi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3abzijifr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mjzjqxvi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3paffjaoc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3meipnjgb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umlscmck.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dglhymvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxpnjmmc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnftqx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uankchqg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pgchdhbv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vdhnwtya.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dckyezfo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gbbederi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cbjeohlj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yerypohg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jmxzgttf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qgeezqmg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvpikpty.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvxvsrei.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gyojvyha.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgqxdzut.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3smubgevj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kkvoianz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3htjdxhel.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vgbmtqjo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdngysam.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kezjkpcw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lbysvoja.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lnzgyqry.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3huuhxedk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dxqdgooh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pqpqmsib.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lftuxfgq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kojirqgn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thpptrmn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yernxldr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nwszkuzr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3stpvuidh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lclorgli.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vrboawpw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3bupnarhl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjndxbec.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3djtbzhmg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rniprvhu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ypcympff.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kketppcd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ddclinvg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jjzcysms.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kivpodze.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jdtpkmvg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3crvhbhni.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3aepgjvyr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pfekgyfg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kaviqwcd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bgbadknn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3eyyaazbf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kxisyffx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmqdmtu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3nnviqapn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tycduhal.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3omuqqzrg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3paijbpmr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mtocnweu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tgxmokms.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3cdyzradj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3layyzsdm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qfohqsji.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjexhvx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zkaghzbe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rltchzrb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kmkfufsw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vevmuxdd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dkaaomud.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rhrbonsw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ywvnfdtx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xhairlxk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ljxidxpo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qzvafkyn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dsrziiol.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpwdbldx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlghcuxj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jxgswchf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brfzpudt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cqhvtgkm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tflynxgv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3grbronfg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjnvfpr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cnmehwtx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ruivhmex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgdsttal.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jqfzonkk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yojjfszy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmtcbdzc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3brkfzsjg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3waidzrmu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3orsjruiz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hmuwlahb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nqhjxquv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmchscld.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mmlkkhrt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3anbfmshv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hcznenkb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owmznmjc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eshniccu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ohwoinin.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fdbfhmve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3votkhwup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3imwbindk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tlchtwtf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ggnfzkop.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxqjdzgw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3pfnsatrb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dknpewqi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ilqpwddz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bmjfpnde.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hlnpzhma.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kqxpouor.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ogjpmtbw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3abcrdlfi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3hxvocemg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eggcgklu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ivcsjtvo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ltbomwjp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ledahyks.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfjrbbx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yvhfmtsa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fghfbwks.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3zsbowbjj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sebnycti.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dbopqzxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3kfijhbwl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bdieclaa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qblbnomo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ujxofgyq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3hbdgvsya.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3goxjsrmi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wkofxwbl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fllhlizw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3cldkrzju.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kuqruzoz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qlexpodv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qlpduyuv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ubnnjbef.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3accsbics.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vytaxvpq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3dojxblzc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zfbgglgm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fpqexokw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bzojgjrf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uzsjylme.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hsxikthx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vltkdkgn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rriytxay.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ascraulm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3axsyqblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpkqjoje.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3lxifqszq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqyympnd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ovglbsji.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nizuntuj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fndatzfx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzsmuf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ppkqhsiw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fdjzxxoc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3tufnkngy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3iymsxsim.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xidqeqhy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3raxwhvnv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mbwhfxve.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3egurmvbf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wdmgmcxa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nrlnkhoo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3guncipog.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3volwhffy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zenjpffh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fmammdyu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3srgcfjhn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3egdxjvyq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3mpulupdw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vgxdtbvs.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cijmqxgu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3objfuwbp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sfpqldxk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3whlmfzgz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kqaukxbl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3vfnjfvny.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3esqpggqo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3diivasxc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3svznseba.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3mwwhezby.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3tkkcdqim.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3jctbnltv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqtipzc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwczacz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3slctxtri.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3peqcaypj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3bvpjtrpm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pwitarxl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwmljjt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdjbvmw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ujmttgky.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cqbripqy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwauieh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3djlgdymu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ffgrwluu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3szojnjqx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dercxfkp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kqatcfrb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xldgwdck.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3fxxsglge.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3pmwssjzn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cgsmicev.html


<!-- 参考信息 -->