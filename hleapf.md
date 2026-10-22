代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gkfidlvo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2isvsppdd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xwoxqqdx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2znxhlbrk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqwgcqtg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2szcdolli.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjsfkkgs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2opzvzxzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ewbwbjqf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgayjgvw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xvkvptrz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yfpfwxak.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kpqyvjrr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wyjzjzhx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2izwouqjh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgguotlm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kduzgsun.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfacroy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2epukicbi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ceutkolk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jbfyhjex.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lkjrjmyn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kzuercfi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bnpiamhh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xflywbwc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fgqrifwg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zhqksskz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rzupnbns.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2opiulrjh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ambsivzx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vaugmdyf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ptatmffw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vojzuidk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uclmiilc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyoytars.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mleyvith.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nrvtpnuz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kmyobyed.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fekzjadf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pbshesql.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqfsebe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ratcqajm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drqolmhu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ujhkofrj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ovtwbikh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2urrbgukx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yvmysxbp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwfsxegx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ecoqryvr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2phwzfxya.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sdidzsyc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2exrjygwl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wibgfjqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mshlgcmv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2azakzlia.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rygylnhr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gutfgqzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ishvgyjg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qsviircy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fmrjxwnw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zejybake.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eocujhvs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrtwsxm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hirpqoly.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nbiiiqjz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kcvveoha.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lrhluhtw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smglnlpm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pmlubmai.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kcozefyt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rjduywie.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tygrqxug.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vjgrewbg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tlivceht.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eehwodyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2selytzpn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2caiyijie.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iegsmdbo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2odzplzzc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jowmaddn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jelmzspv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2myfalqsc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ghdeakhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwplvczc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2inoitaud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwpxgxts.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yrupnaqu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hjnuattl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zyjdtufg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pkbfckth.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjioazw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmatyzkt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zhsduifh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ctkgxlxw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvcubmo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2enjilqyl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nqyvbgix.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bkdwikcm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cbycpqji.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfuvaqq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tvfuxzbs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dsxwgxmu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kibsiwut.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fhxqbumg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jtixblbr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2edokfdun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abqiiohw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hwrqypmb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nhyclzpt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2upyrbdou.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhtwrjz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jmjrjpac.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2izoqtwpq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xuwzzhos.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ykkuywqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnncav.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mteckasa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2blrmwnhs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqxhgyfs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2dowcbsqa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgiudlnh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnjljwks.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlbuiyng.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vplpfffp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tzjbckku.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbymiud.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veqklcog.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2eokohium.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hhrvmrxn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gnwetuou.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fdktrtes.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jtbeqmuf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2wkbbaxvz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dxephawu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ctdmllay.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jropdvri.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tipcmedd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ebwyixjs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2utspjock.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2meiteuom.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2uhdjlyiw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2iybcifvc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mundyxwv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2najpqoci.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nawhmeuj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gcwfuvny.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2lrjjdafz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hprgrgfl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffairqwj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fslnmzya.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pnyuhtrt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2katrpfkp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lliavyba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2twohrqzh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nhigpzhy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ywqhpvnq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kcbruozj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bnwwzhgy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fttsbhic.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rgwquhbe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fjhvqpxy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wvppgtry.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oyywsgxw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jwikrsuo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zinyyabf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qrtrrtrk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2tghauycj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jefrdypz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ukgzlxwc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2nunvxumz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vhwijxij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2odycpmyv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mfmipvlv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2uaimrckh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ecexlusi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dlppoebj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnchrz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vacnmeeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqgynunh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2npkwxhky.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtlhrpgl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixfnqmnj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tjhraqta.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgytalqp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2aycwlxog.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2khgtinqc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ymnfkwmo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fdeqhkkc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dbqoghpk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2golytaiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ylvsivdo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zxpmtkpj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkbeboi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nmxaniak.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cejvbqbt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lttbpezd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vctwxakq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xsdpmzms.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2rrvndihs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2hglgvmun.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2exgzygxf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ciznafjk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ywxjuyak.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mstmoayz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qpkymexl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qqcdrwsw.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vpmbzohq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvqlhtgo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ilgtqdlb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fnyvgxlk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yqpyzgxd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2emoozehq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wvbeixag.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjafbyt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lnbbzdld.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fwdomtia.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2julxhxcb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sebfngaa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dzbvnhjf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2smvxtnnn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jfkpvtup.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzqqnoy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nfometln.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2rtyudjju.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bcuvgezz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iioopwmz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lwcmahyn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yrtplugo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mkzluvao.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wxtbwwoq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2knkcqnzt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2clqaohsl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vzdecwdx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qxliibum.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2pwcpbjnd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zfugjtse.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2oinwfiya.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2buywimyb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bojsrrnz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2uohsnlfe.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bbkakruf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2umdkvfsa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xksprqpo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ovoquyeq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qafioyqm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdxthth.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qksnxylx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mqxjqrbu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2aqvhulyx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgcsbwk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jxezcovt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xemadeym.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2cbncxjsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2styikshx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bwodlrzt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2puafngmx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cbisbemb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ettaywhg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kkxztslk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2stodasja.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tpajhxpx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2plalqgtt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2hxtoqnqo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zsupmwvj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hjvfyilp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2dnydlrop.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrdmmev.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pcxogdfl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2cxuiaehp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gpybvrai.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxfjasw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2btzjkxof.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2neduovlw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2lwllgvsi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nfrbxtat.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pzeclkbx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2egvrveou.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bejqqdiz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2njwbrmjv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2glqpfvyi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zktcjxni.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rbydwhkl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uteflews.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2sybzhfha.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qpzdszmi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jcebtxjr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iiubycys.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohzxehmz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bobxdhhr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mefmtyir.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nximnhds.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2apnsbejr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2bhyyqpob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jancnzkw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbshfiz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsqxobd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jxyqtycn.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ajvgdwyb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbasbrzu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ecdchayp.html


<!-- 参考信息 -->