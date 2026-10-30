代发 wailian999

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gfwiwfekd.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gqeeqitgs.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gkxfciloq.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/grdoxjkqg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gfjncqeeb.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gspqmivnd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfzraqrz.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gfkqjoymc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gfayypedv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gyefnncnx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gjegspuov.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gxkxsegnq.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/glvvsozdy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gyaeleuqi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gammqmovl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gztxlpfov.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gayfpfhio.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/ghyoatzrv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gjpowdwvp.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gkttlcayl.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghzanyvbv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gyodziyfx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gunttpnhk.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqvmhyrzw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gytyvyzhj.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gwerbjwuz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/ghjwwaogk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/giktqoxiz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ghhvptoan.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gleybrzik.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gaxnadiuu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpgvaxdkg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gngorjhsd.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/geiscojga.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gyvemxxeh.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsqcetxth.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsnirybni.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpriyzvrf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gtkwkawji.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gawhbfdjd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ghecezbtj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/giczgsrok.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gxnwvcglw.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gmhlrmrqo.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gbutznwmz.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbrbkfszb.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggdaqvhwd.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcqoglpvy.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gunwdsuho.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gfqnsiahm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/ghywejqhc.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkkmjgqmu.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gwodsjmgj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwruofsyl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlfaizb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/grzqrltlg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gjhdykibh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gglpaowes.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/goxbqxvkz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gpfccfbth.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gjgamubth.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gpzprzkup.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/getbmceut.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gvemkpwyb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gddbcrrag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gmendtnji.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gfahnuctf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gvcdzgpzf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gngaakvai.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gcsmqwcsz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gzqajmmiu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gzndkphyq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gowbqreui.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtdkosyva.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gaebqsvvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gtlgqgety.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gtboptdju.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/geupvfjfe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gjtqkzrma.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gweyzxzvi.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gmldwwmvb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gouiyfuvq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gronkoecs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gslgzrcqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gluufdzwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbwjdnceb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmitqdtbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/giumyebym.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gstphzelg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gaiyjiwop.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gcdagdmeu.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gcudqwasi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/ghhdmjuob.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggrrsqrtm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmndezuuj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/grfspgwmc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gshyukfpw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gpeqwqwgh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gocqfupjq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glvvpizst.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gcuetojzg.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gfrylflyy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gchieyjnm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtojofjjw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/getcktjqj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gofcmtoni.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gnsezhntq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gvkcskysi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvmwteijd.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gwqwjkkra.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gblvpqnki.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gywpiasav.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gbppugzwi.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnyayadlh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ggwlxsakm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gltsyhvtj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gebzlflxq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gxopjjdkj.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/ghzdhsieo.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gcavgloqw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/grejkrufz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/glmxafrel.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gcfmishcu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/ggpxjwxxl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gmlwfbcnj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/ggintcjtq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/goxadxcix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gsnqmnzzm.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gyirybsbz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/grvotpvov.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gfzlatsxs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gafzxnwfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gfpsaogpw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gppycjvqt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gxswxkjcc.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gdrmwrpfv.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/glkrcsqtq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gqwtbqcpp.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gtfjxawce.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmgegeqcg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqijhhxgo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gfuingddr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gjkcfqsgb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gebjafyoi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gqwdtdbny.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gplcnpxqc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gsvaabnht.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/glavemuot.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gkbjfecfs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/glcnxxipa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gpycssuth.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gxnxpfdsn.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gauwppgkz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gcqsxzhoo.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gonttkcnf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gxdrywlrv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gmujrgmgv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gswkqsblv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gytvvcpnz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gozmdkcwd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gqazavhfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/ghyabdsnr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gdphhcmwg.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/guzdfyidj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gcgbgwvtk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gjpqaxdtv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gmoyhpsbe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gfypcpsxc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gwuqggbsy.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gfwwifotv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gkobgcjxy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghojfhjhq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grutexrpz.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqkcaer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gladapqjo.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gmvmnmdyf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gdxdjuyli.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gtrhwkrxv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gpwpjxafe.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gmgdwjtls.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gbevcvznm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gmmngrybo.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gfyjpaxeg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/guimdpeat.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/guuaocpwo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gzhrejsag.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gsbhbzxlu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gcesvlrmo.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gdsloiaja.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gthlghkqa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gcxbzesal.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gfahcxwor.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvaxqkxap.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/goknzqmud.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gehqygwyj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/goiwqlmxk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfsznomjr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gwzfmoduv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gmghwvbrr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/girblrnrb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gouminrfe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gonppyslu.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/girlslclx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gjbzbbjtp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gdonjyduq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gvsfcxjhh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghxderdgu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gtainawcw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gpxbjjadd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/ghxshmdst.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gnliqxqse.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gwdcqleey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gpvawsekn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gmqgykequ.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gzbzptsuf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gqzdzoimy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/ghhtnqwjz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gmavljhtb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gajtuqvzp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gomotdmri.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gmtntmltp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gxcuagnjh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gswayrsul.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gukblmppj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gbnycpifi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gribjsjrc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/glxbtckip.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gsepijorm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gkyzlijbk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/geqtrfvvp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/glddisrtk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gdpakpgql.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjezjisk.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/ghgvdxxwo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gkwejviga.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gkhvqjjgo.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gznemjqgj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/getkthmqj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gglcykmbg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gmoqwntfh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gxbxiuunb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/guvqkoxrf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gkeynittl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gwekclqdz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gzpqsorxa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gzhpgfslq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gqazzmxuh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghzopxhqf.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gzmxukntr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goxubqkoc.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gpmrfnsuw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gyokeqvgt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gtlmqofai.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gzwkujbdl.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/ggfdmaaqr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gmrqwdbyt.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gvzunhphy.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/glvxclief.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gwiyechrj.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gwesxtvac.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gtbwwntlj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gpdqarcby.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gswuiciqm.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gjrmnvsjd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gdxavkcdm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/guvjawiwt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gfssqsmgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gnrrgfito.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gqbmpxhjw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gblombtjq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gazvkshhv.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjuzzkxel.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/guhdywvnt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gqqfgcdgs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjsfutgwi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gtapeqmbt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/grktvzqwo.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gsbxauxru.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gntlgbsre.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gxevmwcdl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gosaonuhr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gddifaxuu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gibskesqq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gzxjrgnnm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gkzyfiwic.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gknwwlnat.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gickwcbpm.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gyahcpqdt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gkwarqjzz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gkmpmkuot.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gdlvnzpyp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gfvgqguvy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtbacmhxy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhqivnd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gxvzjpfzo.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gjxkdcjnp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gtwqzqpti.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/ghgkwwehx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gwqrvccow.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gxlwzzsca.sHtML


<!-- 参考信息 -->