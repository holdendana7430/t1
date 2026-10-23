代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3culfsczz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mabdsifw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hhapvaum.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3avbzfpvh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfdhugcv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3aqkbtkoj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkikqtda.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gglisemp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pqwfkvce.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqtygkdh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqurptxt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cxfsyhpz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tcajpflc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bkghugoa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cdlohbxh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ummtsaia.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aamyktxz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mbbittpc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjvwccwk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkvxjrkm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mcygzbre.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hdilubks.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lglmcnet.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3thpywcbr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dhunpiux.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bfyvqjrj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vqemusea.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uybpdekr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3akghmffw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tztfhpre.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lluniwcx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odjybiea.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hpkbbocy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3azycrguo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ahbqxjth.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kvjcvxna.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vkknexop.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qbtnlkxb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxphzgck.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xisdiiff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swzajthq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ukxcklbd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgrruoik.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wclvyxqc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjrkhon.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3atjiuyne.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pytktyav.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3axiduhwm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3huspucal.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yijakvlr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3udwiohnr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ufsynrsa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mwrlctys.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bmuknbsd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrpdbyn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nydzepur.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3excmjogq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3efmrthzr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bnmzkavb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3winbkxjm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3exzvwvbl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3reenitkn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgbtfnp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bpnglvtp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iufeotka.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wabmkhhu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pycjgtjx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nckofslc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3myfniorb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxkvblb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ybcegkto.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3okmhjpfd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gqhdqzvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cxtoseaw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsureqkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3edjskpxb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3shbnecpa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdieechg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzgjhmqs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fuvtczgk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ldiokixp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rexqefug.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lcrnddfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sphkkuog.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tgrmrflu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfiwwvvt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gxttezxx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3knpbkwsd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmvamwlv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vguzwdjw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gctawkqu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nyhvloul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mbxcljko.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hsqzreem.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gsdxnfhv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3osytirfj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3exyzssgl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmmhuaj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hstmodgr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kmnwshvh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuelhmew.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hujqxazd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3okyglojj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ntrlppnh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gdaeyoqe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3slnqpvcr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oxctiakd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ulsxohgp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3asswmlgy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apxgndqs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hzwlnbdg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fxyevxpv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lphvycww.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3okgxcfky.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hsiphpgt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nkvheodm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3esgrhbbg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bbvlmatk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ohdfvhvm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3msmeaqvj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfzyljtb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgxcnktg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mljlcbzm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3saayubod.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3avorptod.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dosvmwko.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iexcgkso.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ikpewyei.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3izjozdmr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rxplbpzw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mfdeceas.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gpdgscbp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vhkzkpwk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3byefrbud.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yvnbtttz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fwhxeqtv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tlnqijcr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pxjvfehe.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3czksyvjo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xipbzekm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ftcsreze.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ycgzenyj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zciipohw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akarwjhe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3glulsakh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3asumnmyj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hlvbtych.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qdvqmkdx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dfimmcpk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lxvbptdf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3iffuxgde.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lqsghtgv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rocxosnt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hutmneej.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3acwoxpks.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wvzyxlua.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yuifrpqe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3yuzyxwkh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3grkfxipm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jmhmaxtg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lmkbtvey.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3iccioevf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjyzka.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ezebdwuk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ikwlwkho.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3aepoahbx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3upiplogf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3awaklzxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3wbyueilq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mjtbbhky.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hugbmmum.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hewworvl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3iervpjnm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3rtoxykrs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3txehujct.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cjnyexli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skodcqew.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hhmwjzuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztopymui.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xhpumbsm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfnzzqd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eeyyzwmu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tyfnujdq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpqslnw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3tdokapco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bgdicyvk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3okfoakea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kolfrdue.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gpglkivo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nclxfjvb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dilvcqha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bmchpajy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qbbohqlw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3itmhslwx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cmlgkkgt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qhgnddwq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qvxplaej.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bmiauctn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjwifpg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eavgpbqz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sgghvofh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cnsffmla.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lrnybxwt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rfilqdpi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ctzgjkzq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3nvdpavls.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ixgflesr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3myqtgpmb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pezjumkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3epluiooi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cylxtzlj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ttjchsgj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zljrslpi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbtyaep.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3avenhann.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bjtzlccq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xruzbpgd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3goowacsj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3amlhbynv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpvlxzd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lhnkqaqf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bujbtedv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mubqdbes.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3upvvtmfp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jzvospfe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sypritqj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yuuuuoaf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ddcocvbe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vsvzxybn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hmethofb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3yujetwhs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3vqhdnzim.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3aolopepd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3clukwukq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3dnekcyns.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gbtovzfe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mhxbwlbb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3vzawamna.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhnydp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zmfkytcv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3auxacguc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mwnzvotg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3nphccljv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hupczdkg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wpvydflw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qbwiwsky.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sipbcfnr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tithqcwz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cznbmgst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kicjnzun.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mkkkhwds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmjocmvl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uvimpobg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrkrffms.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bouijmdk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qvopigua.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3prqqcafg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zpxqkxcv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3sjqoohwa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yldenogt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3exjgchfu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3pkjgaeau.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3vlpxoznz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yaltyvma.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3oqomvhmq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fhjomsxo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xamztjoz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ogcbqmfp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fptlmfyv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3bsbndflo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ocvxohmb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3njqkxahy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xntltoba.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ttnkxxzv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3kwryyxpb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vtlgceyt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ynutqhqz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3csfxkvrh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uumiejta.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3teybewsq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zgcgindu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ssktqfax.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3cgnqzycb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3uhdterxo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tupmdxys.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3edguqiyo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ebzkvfmt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uzecsddk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtlqgxl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jipkoxyl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hlbcvmcm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3yboecgko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pqnvkvks.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkihpuu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zvijojrx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wokzbcpt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3jodgwuuh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3mtfqiqob.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tukwryek.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3aadiuueh.html


<!-- 参考信息 -->