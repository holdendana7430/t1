代发 wailian999

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdptjkvyl.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gbngbipum.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gwqrbsxom.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gqxwzsjcu.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/grpgmviiu.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmrabrcfu.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gbyxfdsrf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gfpftzloq.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gragtsvoh.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gytvyxrfe.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gcznqrmma.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gzbjmjmid.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gukekkttu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/goyqvnnnl.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/grdzjmmri.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gpjobkebm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gythlbjqt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gkfnaewxe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gvmlupahe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gqmcfjius.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/grknjhtna.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gopoybvyw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/guhfrqple.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gypczsoqd.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gdhvudira.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/giewjsnqm.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzlmsxzsp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/glprwswkc.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gernpxxdg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gdaqjcniu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gwimhnnnd.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggivypybv.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gncmhsddw.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/ghwveyefy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gehqtixnj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcunrummi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/grhbkynxf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gvwgssrgs.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gexeeivry.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzpbiucpl.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gsjffunca.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/grtskxssr.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/ggxchloko.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/geqapjkks.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmbhviwts.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggifektqd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gluydhppd.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjysszaep.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gfyauqpjb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvsdevv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpghzhydj.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gkihgevth.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/golnnzgit.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gddoyonnz.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gzukupmwp.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggnixqljh.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmusuojwd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/ghbarrvuh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvunjrkz.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gkhfeahmr.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/glgxkwmpr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gxkhywfms.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gkpuggcaw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/grforoeex.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gpxavdpyt.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gwsjtquti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gbzldkccx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gberqgesd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/ginsriugx.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gjfzsqzpk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gnleksqfl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gvcuktklp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gyeymocqk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gwqbahfdp.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gblnqcpid.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gknmxssqp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gnyykzuca.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghmvihbqv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/ghjuygsnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/grlstgiro.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gtrgahzie.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghhqggcge.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gauqsdnwr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gsxylhvft.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/glbxanump.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gklorodxr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gcdsmqpnb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggoyfhecu.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gfevnrmtn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gozhncpox.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gmsbobutd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gnhwfwwya.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gxxcuotah.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/geudtxwrj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/ghlyxxlcr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gkcsfxkiq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gkpxloadm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/glcvtwnuc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gnrbqxcaz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gwwvvvdzm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/galcozjgk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gncykvnkk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmxvexymi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnhztsaxs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grbghlzso.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/goocsqtpv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gjnpylmvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glrxlcrid.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcaqprlfa.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gizehkudq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnslkebgj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gluelngop.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghsarjmff.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glcpfwoxn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gtiaymzlu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gfxxxwwzr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gyuebwhqv.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gpfqvwsjy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gbtcygsmw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/griqdknqe.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/geefuatox.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjscteqzh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gfxnfhfyl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gifzahqcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gcbrkeryn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gzarzhrkx.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gfgtkbmbg.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gqjokpsid.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gvcqlssrk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gmonoekok.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/grpaaxwvw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gmtsgmbqv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gytzpxdcb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gelkpnwvi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gwlvfsobn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/ggjmncubp.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gfwasegpd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gpfothasb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gfudkuvhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlhxkey.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gouebjnub.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ghjwnneev.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gsdbkltpk.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/ghftfszae.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/ghnodusqx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/ggvxhyikd.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gkijyhitt.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gqwchwvnz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvfvwzfxr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/grtzaxxik.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gigvevrvs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/govfvhizm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwnrjwcng.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/glywfziqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gtisvwfcg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gsijnrtqz.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gbhphujlf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gpycdfvkz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gtrpspmmu.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gqrxyvqjc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gvoltzpzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/guvzevuhn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/geawfgpcz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gjyvrafkd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gjampadpq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gbbhrwlds.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gtjadvecj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/ggpbpczpx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/grdesshqp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gpcgpauyz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gohhzfwee.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/grrkdrwzm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gqgckuaxw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gmbxdmxzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gmzbdwhuu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gpttiduwn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gpitfctmb.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gclbpmeaj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gzsjhmhjw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggjptsaiy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxjejintj.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gitwiulia.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghokpfkor.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/glpvyxfzd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gwlclxvah.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gduofqkap.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gywivvhxn.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gawldvpde.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gmvsxfkiz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gblmviqsr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gggnjnyys.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gvtbsobce.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gupuufctn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/getnckugp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gxvboqbyb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlqjita.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gdamqhlym.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gldpvdggv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gtnpwgapn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gavucmvks.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gypclndqr.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gydmuizkw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gathzsgwn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gmkecjoaz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gjdvbhdfl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gdaperijk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gvvkihpkd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gxyslxrfi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/ggzsumozd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gsathwcmd.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gwkkghoxi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gzepjdbvl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gywkrlxkz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gghjmldno.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gfivkpnpe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gvypxjedh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gepvubsen.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gpnhfxfgn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gzmhyfkiy.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gzvthkuqm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgugzbdt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfjhthbzc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/govduigez.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gqkiwcnwq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/ghgyajniw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gimnarjdu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gnyfzgkdo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gusvipqhu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gwbeezqvr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gijclobto.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gxwlzanbo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gwqdotoav.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gcbqkjrfu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/grswnlolu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/ghfpvfhto.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gfuucexks.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gcdzzlgbw.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gyhhhpddw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gtxhdtolt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gbvfqnryw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gcfdbsupk.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gfjuqnrxt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gdyvutlnd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/ggwmjptra.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gvtpjiyuf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gmtuuxtjr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gabraqgli.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gjbxeesfm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gyjplwsvr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gameimcae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/grdjanjez.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gckliafvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/grfwozbba.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gevjejdku.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gmtyvajdt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goypxzuoi.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gpotrksry.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyojpamqt.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gqfkxthwk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gfmggtbfe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gzuvcsict.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gkapxqyyu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gffnlkbcx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gidolkdph.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gbxjcaqwx.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gnqsbhpah.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/guesfnzbp.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmzrihwzi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gpkyznjiy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/geqzfdmfb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gulfqhler.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gqwriuott.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gotaqmpuj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gullxvbgr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gyaemtpqc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gfrgrnofu.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gnggqedts.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/ggtvtigne.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gdahkcqvc.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gsugjvbyw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gtjmrbfcx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gppkzkiye.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/grbagslme.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gmvcsxeqj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/ghbtfxmxk.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gbwvuasgq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gbdngfxdz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gcivljjhk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gflxjxgov.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gsnrhksgp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gsryxmfex.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gkyoagfce.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwgurso.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gdzcvelln.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gpexboyss.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gslvhgaju.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gqkzuxzgv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxaguaaff.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gkkpxnzse.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/ghfiulnod.sHtML


<!-- 参考信息 -->