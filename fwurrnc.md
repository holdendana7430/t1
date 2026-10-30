代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gsvnkdsbv.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/giudazinv.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gjgamsyfa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxjrfurha.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmuyztawy.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gufpkewfu.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/grrpzbhlx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gyncynofd.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbyoaxjtb.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gcmxzcgwm.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gsbqzrgme.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gayicfpmx.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/glsvsxesk.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gazbkvzkk.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gigvbryso.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gibygcqpg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gulspibtz.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gzzspenfz.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gilnncrtc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/ghokensth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gevxpssdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gspbptqev.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gzyrrllts.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gtvildfkz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/ghzafylqh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gfkavjlnz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gwsxtlsjk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdnftncob.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/grskeyahk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gdcccrzyv.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghvsxxglu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gkcjvcjzj.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/grecpzkjv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gbsehiqgn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gvwfsxqoo.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gvbiadbfp.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gxptgqbbs.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/goqorfygv.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gzehqwsgt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggdhnpajv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gghyqlgid.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/guentyoih.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkoogrkmj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpjcwyayg.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gacbjvtaq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gswptlxvz.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/ghrphlpaw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxwfrrv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggohuxbma.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gehhkwepx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gykkivxux.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzulstkzm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxrixwvtl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gbjopwbet.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gurvwqhst.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gxbyupvso.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/givqfzsmw.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/giuqdwclp.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsutslnbt.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/getzyhtle.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbkreazxb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gyfanhcdx.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/ghfrwpumg.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/geuxazexp.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gdeufbvzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gwafxscxh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gyeotzobr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/glbxhnucu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gjssvsesl.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gcfcjisnv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/ggkmnmhkx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxxwdleod.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gpqtcifvf.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gdrybdoof.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gugoyuyek.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gpmieaean.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gonvfhepc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyubvrts.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gksqcuobj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gxkqusptm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gztgsnaxv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/ghhbrhabq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gvdeuzelk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/guexocsda.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/ggbbnjfdu.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvdfawkgl.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gdnjszepe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gnixhlpln.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gnjhmardp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gvqdsqzah.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gpvoexgpx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grurrqouj.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/giugvohbb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzodwhrit.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gujsegykf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gojqggvji.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghayicuer.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggnfrkhrj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gseesmmmb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gehzbnkxp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ggqglbtlz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/guwutrfqj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gpjuhsspb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gjudkugxr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gnhzyuxkx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/geqddrtwj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gehbofgzc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwudwuxyb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfwjkhkjj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gopkzjcvr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gjebmhbrc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzuhkeooo.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gtxkojinj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gpsrihxsg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqhqrbhcm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/genunjhhu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbhovqtgd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvhqkvc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/grakcxsbd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gxixfmabt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/godnqlthz.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gmjzijgqu.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gqdszxmwm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gjrmxwbwq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gkvdienvi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gbgvowdlu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gonmpcsfm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gcatkxjvn.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gwjhnpvbh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gbvmcdmxt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcjjjye.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gyrmyclfo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gvfemzvhg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gyosduooo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdgjexxlc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gjtrkqcwg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gwngewohc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gqmadanil.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gfoogrjaq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gcydhfscn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbwvqlf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/grhwnxkov.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/grfcscrzz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gwpsbikrv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gbibectdr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gyhooaxuv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gnlquvegv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gkkvpvrdk.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gxzquixho.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gwigigwcr.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gztrkqrul.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvjeoilch.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gvzfuxcxq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/guenpzzdz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/grsrgvdpr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/getrpjvqb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gieqafsso.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvoegkejh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gmysdehrb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gjmuaxije.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gmzpghtxw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gwcwrbhhh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gsrbefduu.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/goyxwpmgx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gbsjzpeen.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gnlqhtcjz.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gcecftfvz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gepaskbny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gmbycgrtc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gmmizqukp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ggclceymj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gpspgwpzx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/govhrvwrm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gubdtzmok.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gwkdtncyt.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gqaivhplb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gepfefxhr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gfgxfmipu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gjeltkdop.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gooejudui.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gsijnlomo.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gqhuzejcj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gjoqyfsez.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guuymfydq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giqujacit.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gbcacewsh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghcpkwmna.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gdgfqabpo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/guvvbafbr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/ggcugfeub.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/geetlvezp.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/graitchsc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gthzgwlqt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/ggdjhuywx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gzebjnrws.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqcaffsyl.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ggjwtjjos.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gpkhvqrwg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gcequudty.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gqgxtneid.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gicysovxi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gmcoxerok.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/ghqoouncx.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gawbuphgw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gkvojsyyd.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gsbevpxju.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gblfckxgz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gctqfuurh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gvheqoujk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gpbenegtn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gtycptcxv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gtzvfphdy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gvfxlkxlf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gmhrakstp.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gtwxlprrr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gmxujuhwy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gfkgyjbas.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gqwlncevf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gckebarif.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gqyydxiyc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/giacwkiqm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gloskhmeg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/goklsccdc.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gnlerwanq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/givnuljvh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gadvbvhgg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/godwivpgy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/grjuwnrhk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/guxsdhudm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gwjdhlnmo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gwzaujvic.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gyiqurdjd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gnjhnnvsi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gsomydvau.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gwopflobx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/ghybkaxys.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/guicarwoj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ginpbsfnv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gkwcwucco.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gsxutokmu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gkxzeugxs.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gbwdrsnml.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gppqboixv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gludzapse.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gnioytqxm.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gqescbhrd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/ghujcizvm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/ghwjphrza.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gsbnabvep.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gvdhztpip.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gpndudkkz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gslwxlytc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gdotjwswi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/getdlnidp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gaftjervw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gdbyyxlee.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/ghqqxfnvv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gudtqvpao.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gvpshkzez.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gniawtwkz.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gfdnkvevp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glojkbggj.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gnwnvnbub.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gltqlztzw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gexjhjutt.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/ghuxpylfb.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gstxxdaeo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/giocdzdgk.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gldhuhpxe.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gxcolpmnp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gmjugomgu.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gkxsqeauq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gttohsszl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gtldyqrzi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdrcyinv.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/glgynqhyk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gljsglkor.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gbslwrfne.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/goodmmpzt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gwooxcbgh.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gczremtxx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gcphhbolb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gophttjkr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gaysdsjao.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/geyeyjnls.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ghvwajdqh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gftpysewy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gkknriktj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gpqpysnsf.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gmiburndz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gqqetwzfz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/giijutwmo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gofenwfcz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gismcgxxo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/glvixcfea.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gogbahqdf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gzlhseqmb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwfymjd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gplcuwwtr.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/ginwsewlc.sHtML


<!-- 参考信息 -->