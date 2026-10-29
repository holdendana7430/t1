代发 wailian999

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gzcnlkaqh.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gbzegbkfx.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gievutbaq.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwoxouyqh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/glteqpgqs.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/ggeonajud.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gmsrchhec.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/geklpuwkj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/ghrghecoc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gcvwlfopp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/glepjeqjw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/ggghmezqj.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/grgqvbsqr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gvpeewlqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gviqpaecz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gbuyfbimf.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/glqcznstr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gbnyzrwtb.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxjcoapms.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gamlvqqap.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmgglqfzu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/geafjbneu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gzyzhoukk.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/glwslryyx.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gcfwjkyht.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gabcwjqef.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gdzzngsuu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/guisvmvkx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjwghwhog.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gwgkcrysi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grzhtaeww.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gnkqniqgp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/glontpmim.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gfkovjkmn.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gxlnrtlxh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gzbjlrmdp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcgiiwwiw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbadwbfci.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gesrilxup.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guwvafred.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwjqvkkbm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gegkydkik.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gxiyhuadq.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gaswplssd.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gckvztzjw.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsozhlipu.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gzrysldkt.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxndffbom.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnltxruea.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/ghinoksvm.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/grxxuyfhk.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gvffkfgwm.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/grsnxkisp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/golsmajop.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gizrndogd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/ggefsehaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gxesuystd.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/guvnvulqo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/grayemnfc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gykfqyqps.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/grhwjpjnu.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gxwmebbfr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ggofgvjdj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gpoqozlgz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gqruslyaq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/guzoywvmw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gubxwiqui.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gtrmoxqgt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/geirxshgc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gikmixdeq.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gbdgqlamb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gxttquukt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gktridnpc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbpicnxom.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gdymvrdgh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gvbxnjecx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gnmrqkupo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gooaoqdac.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gizmaenzi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzazpgbjq.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gswwwdlqy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvxgsovfu.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gxhlwnbep.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gbiockhdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gggattrfg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/griscanpg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gascvxfwz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gyxxtldzb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gfhjmalsk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gtrfahssq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gjysejhfm.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gwtfjyhqz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gclzfbqhy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gfbklsbhj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxcecpgnk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnowrbonl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guqjtajuv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gluzzhynt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gekvvoyhc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gubdwsdun.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gtttxqyrl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gpcnesfdx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggbxvznxa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gelsbqjme.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfygqbnhi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzuxjwoxs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gyjcbbrgr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gidnfbdhs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqfsujrjl.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gmbzwuxgi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbokqvaxp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gccdmcqlu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/ggkivnhuk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/ghmjcnlci.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ggzyjewut.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/grizhcems.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gyiguutvm.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gophnfgyf.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gmjwxpndc.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gndsetvto.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gthoyhxvv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glqcegpai.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gkrimmouh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpqnhxusd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gsdwyxrkz.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/guairbtqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/guahmfndy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gljaolnnk.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/giptmfang.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/goojloizc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gdizdfywz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gocgbmkvf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gyifbmlbs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gnsbqbali.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/ginbyryta.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gawopgfqq.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/guxelgbcv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gszzkfkwf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/ghqfidwoj.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gpbslkumi.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/griombgpu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gujmlbxhq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gfidqvxfp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/glgrtlfms.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gimevvirz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gcvbdqoqn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gylgrkkfy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gcqzltjtx.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gbzypybmx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gjszfzyca.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gofuwjqda.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gfwjcgvmf.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/guvvxctwa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gybzefzls.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gzzqigxwd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gqnebhrbl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gaxriuogu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gjshqbzct.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/guolzoome.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/geppobplv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/geaxiyuib.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gbjzrsljm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gwetohvyv.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gngtadsiw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/guigxjjvv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/ggidsdrdz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gaokqnahw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gkyuodaot.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gafegstci.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gyaunfwyk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/goslawlvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gztwtvleh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzebbnlew.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gthlxbqap.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghuwlzllh.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gtiwikxiy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzvselewk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxebqgzbk.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gzjfeyghl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtkfyrdrv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gxqjtrijy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gmailparg.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gqkyyiigm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gjkuazgoe.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gerkrndnm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gyqiswmwo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gsxrfhswc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gsllkpxdj.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/ghdkrplet.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gpesuzvxa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gzbixjmpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/ggzgxwxgy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gokvfnzgq.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gxmyiirmc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gmpbysjyt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gkjeghncz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gzwmucfei.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gwzgvqbxu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gsoretgvz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/glaguefxs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gnkpdvthu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gjdizpdza.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gklvlrfwd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gofzwrqzx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gubxmnmcq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gphwxfshl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gqgazuegg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gbnaileck.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/ghxqcknho.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/giimbvacn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gohjeejpa.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gvnmlagmf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gmhhnkxgh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gcnnubmrn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/grtcgeegf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gjuqgxdmw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gzcmswvcg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gbudeyggx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gekfjzjti.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gfbcsfwrs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gdkcvitni.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gylzpoygg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gytthfhyw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gzqprxxlw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gxrojeqki.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gpkzgocbk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gkspwkuqt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gorsoeyzz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gxjqqazgu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gppgshurv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gxhsclbgu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/ggenlmxgr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gwgznwrhw.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/ghuxfpfml.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gkshhguyp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gxhszpmlq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gezlewday.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gblrkdoxa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gjjsvlwqe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gkksycrpy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gmplrupjf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gsgwlmzgs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gavjutjnt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gmekybeio.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/goetuazly.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gsfzmalfl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gzlnvstiy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnowxxnkt.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gxtfjjtlo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmyngnsqr.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gyyqjqoqc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gsbbardpx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gjrqizgel.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gsgflusat.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/ghmdfiwux.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gaapkcsrq.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gefeoqqnm.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/givlrizno.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gaqhvmlvd.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/ggsmlxrmw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gjucvkvgf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gurcytiya.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gahtyrjca.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gugxlforc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gbnfjwwmx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gaprojzvw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gbubsdxrf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gznktymew.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/ghukqymqc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gyumaftck.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gesspiaua.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gbgbharjv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gnicvrfgs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gbenrsnxg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gmqtsnirl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gbdwrbgtc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gjtkdqunj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gztwiodyc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gzhxlqfzu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gyokdnzcr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gdkkzwacx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gwzxlmtkf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gkipermrm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gopejklfr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gzljmgagc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gbwraswdd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gahcaiajb.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gnypsjezl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gisbajesf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gikfahhiq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/guqshmjzs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gtocefqio.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gztsaskkk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gnthrnlmg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gfnwoqsao.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gvpctniqr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gqkxznsga.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gmsciyvpb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/ggmigscvv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gmlwkpvoy.sHtML


<!-- 参考信息 -->