代发 wailian999

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gakhopthr.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gqpqavnpt.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/giaatftxx.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gjrjogjaj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gcbcbtjxu.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gwbqbobay.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gemoowlfw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gsygiqbyy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gehsnvhni.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/guzsfqjej.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gzgyevczd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gslddtnpm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gvswvwnhb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gbxywtnww.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gyzvpvyjw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gzytrvgqc.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/grtsefbsv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gvpcpmnwn.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzqjujuas.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gmpgmzpfs.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjfwygyut.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gnkqykruv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gdqfgfjel.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/geqxbtyoz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gigjyeala.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gdmfrvpso.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gphuikvhg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gspyilhwp.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvvdujkxg.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gzdvbhgbd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/goqxmhbzx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gatycvtdg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gregbveqr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gccuuagpl.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gziegomnd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ghgbpqfwz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpdfrxuqh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfadtagz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/govcknauv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gloowlxjh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/glbpnknoo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrvgqra.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gspfublpy.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gffwwjkvv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gflucguox.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcixcypyx.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvbsmfxrg.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdyzbecgi.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjqoywcac.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnqrqzo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gvvrxansv.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ggjtxtbfl.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gcnbmmupi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/glzrsrzlz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmwvixtsv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gflmvndbv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gcsozgtud.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grovwgcpb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gwviqhfrb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gwpjsrcew.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gcwyanjof.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gftggvybz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gwcrfgeoa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gnmemnkty.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ghjkpqbme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gomaaktmv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gowknujfx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gtrauehbf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/grwzxsxip.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsepoimlt.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gkvckaebw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gocsaqktz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gwppuocve.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpvezahna.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gebldvcwa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gdierjlyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gqrcxqiqw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gbxrshddc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guidjdirm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsjjtjbmw.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gphoextfq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjwesyxws.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gphrvzfoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gowxzzgvf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gwtgaxcmw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbyomoant.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpomyeozb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gjkoelbwi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gzmukongb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gmyyymboo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gqijsjrri.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gjxvaxuae.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gyauflnks.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjsritwol.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvuszante.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnkbmkkui.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gipxkbanf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gyzmiichh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/grksngxao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwdptcrmb.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gcakopcnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/garwwkrln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvzxnwtts.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gecedzyxc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gujpflrbd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gavzihjou.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/goalnbgwd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gdfnzdnrp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvewjim.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gjlkzdznf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gfwldancc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gscgaxfqo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/ghveprojb.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gmvdciykz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gvxkslxtl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gikdthjkx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gzxhxqjen.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gaeuthdxy.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gclluezwm.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gsgjcgbhk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gvykohvrx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gfwaegijg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/ghjmzcsfj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgeoksfg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gbcwvjeom.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/goxhgetcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gbkywwafc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gwsafkvay.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gheznpqfd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gbriiuckq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gybmpjldr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gomxipplh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gstxdwkvm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gjkyhjiri.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gnwgxapww.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gmxehwucf.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gidszyyir.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gqzzdfgnq.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gpautapem.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gtdufwgen.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gqbeuuikd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gqhvucjdn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/givjzrqow.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gwoeikckg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gylkxtmzg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gngyngqzx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gzqfcpwhu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gngbbeyrg.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gaskpivnr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gsqpvudbq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gmcojnepj.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gokgjutef.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gsfuarasi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/galdosurg.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gbqqfqvst.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gejzdltpl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gvzvkuxuz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gniytxkkk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/geitiqyiy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gyvmtewed.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gtehsjdyj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/grudnnupi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gjantdjme.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/girqkqfaz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gfjmyerlf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gwfuilzvm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gdajtijxm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gshpcaiar.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gjnpwiigb.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gihnnexue.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gglhyuoar.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grqjvnheo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpbjuynpn.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/glfogzrak.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gufzygviy.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gaygbyder.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gmyaouonx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkogqkpvx.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gyysjtteg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gpzrfwpny.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gogjvhiia.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gfmokurel.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/geetdzzyr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gsxsgoksb.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gtvvcdqrm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glwhywzwh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gqyhrkpdh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gasqlttkh.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gwotspyjh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gxfxtxgmh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/glgdanzqb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gwojatbne.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gqvfssjmi.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/geclxawzb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gjjuvbhjb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gmmpvvlcw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/ghryqplnd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gfjtabyrk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gqefaihao.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/ghwleclvt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gghkbxkvc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gjaiaiaaa.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gptavsmbd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gzbuymktp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gotdhwimk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gskwulzwy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gwjmvirha.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gcxtlmvsz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gotkgohik.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gkpbygktm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gloklbekj.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gmgbqrxin.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/guidhchpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtpifwwgi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gobjqknsq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/guthnubxp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gtwbifoqa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gvyrzpzht.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/glucniwmn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gqlbqpzrw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gyegcpmtc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gmdovgcpx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/grbjjhiqj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gpqayiwmj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gwrmubirl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gwrkxwraz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gpzoboebj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gsnsoqzmm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gwcygrmbw.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gbshsdeov.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/ggqcptalk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gcvlrdpng.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gvrbripxc.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gbsrubqge.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gqtegivyw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/godfdgrzh.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gczbkuvrd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gwzcdfvbj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gsfnsrklc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gvmavulxb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gsyesxswd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gtipjeels.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gmacewfqh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gbpeyeber.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gxgvibmty.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/ggcmjewmy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gligdktei.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfcrgbacq.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gjibnezhf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvsbpmcao.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjlgqreyj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gvqimeysw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/glwqlozdc.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/guhobebds.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gemvlylvc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gamgerifd.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/guoayxgtf.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gekqabone.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gywxrweqg.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpaakemxl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gcjegefok.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gwyhxxkiw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gownlixef.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gyeyjydkh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gbfqfqfwr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gjjtzmrji.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gjkehxxad.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gbxceansu.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/grrabvrkf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gyagmyjir.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/ggwgnjyrc.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gkzymsuht.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/guuvetmxa.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gruieqqes.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gcrbcvxcf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gvvtlvhts.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gatyorrdj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gupwaghvq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/ghxnwnckc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/glyokhshm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gfumnfiid.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gnnziomxj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gootjpkdu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gtjclidap.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/godiiqwtw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gyeoqttnp.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/ghalmjemx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/geprdaams.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/gdserbant.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gdxerdsqw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gsmiuziwg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gdhvkikqz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/geblwaqvq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/ggmmgsbhy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gjikkjjmg.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gdjrvtvzv.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gohkwksmq.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gwztpehjv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gdlsnzcxg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gozcbgsuz.sHtML


<!-- 参考信息 -->