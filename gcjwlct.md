代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gqgihbkuo.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gkcqqtivj.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gtufmeyri.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/goqlugnxu.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gsotkrffp.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjkrgmgjq.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gihvkyxjz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gtpmajwpu.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gyrhczkyd.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gwkcwtfvt.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gvyhxfugt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gzmadhkoj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxmjsgpt.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gsthobbxb.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gbvthcpwy.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gquaboxoq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gaszknfpe.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gkhrkxwhs.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gjbhlnvzv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/ghqoffylu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gsmosgbcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gcldvgjnb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gvtckleiu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gvuvfsfdt.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gikjwqslr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gtyijlkwx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gzbgijiod.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gtnnwvhhd.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/givlhrtpk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gznvkokid.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gfpzkiqap.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzbivhigf.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gwxhidqwt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gvouvhjiz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gbmwcvzsy.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwxvnctka.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gdkgjngcp.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/guvgbylry.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/ggdhwcdjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/goxojlxpu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjfvnrttd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gqlhfrdrg.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpzjvdeoo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gccsliqnb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gprmkokgl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ghywcbnjc.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gghjintpo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ggrkjxjpv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gimpsqoof.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gstpkdoen.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gburenzly.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghrvthpdc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/grjmdlrgo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gmprcmfto.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmamujtnc.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gsbzmglfm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gabstbyyt.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxslxbiur.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsvbjtylf.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gelllcljo.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gegzknuqb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/grzbyjmkg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gjdfmrsyd.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gjqvjnzbt.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gtwzluaec.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/ggcnlerxe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/ggacxusws.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gpdmxatdd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/geobvaraz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gycknrboh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/glkiltexf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gogbrkeir.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gsfchgglf.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtymifkwq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gvzyuqvjm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gxcwtonhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gcdrpchlw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gfqrbwezl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gujhvassz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/ggrlxjtcl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gxlhudowb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gdgdunatr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gjrqpvfxd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gikhkkdzh.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gpjgndfob.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/givllkuey.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gusfjjxls.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ghtpneuzl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gbrsgfsrg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gejexuxjq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdfhhqbdm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjykwkkfs.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ghtdevvwb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gophostpf.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gflfvmhjy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gtlrqnehd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/ghcrgjqmm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gjyxajhvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ggpcwkqkt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/guvpbupbc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gxzsxswmt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/grwzszmkz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gllwiceko.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gyqcjlcfh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gpncvzojh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghrgsttqn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gelmgnjwb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gegsooara.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnjwdmbbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gnwetpflj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gvgkicann.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/glmirhaqt.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/ghjptgzwr.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ggfjdgxbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gofnyeuji.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glwpdpdgu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gsdzoucpn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtfdstifh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gtuwftfst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gdamtrwnw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gobfjikks.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gkqtpaqkr.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gepzlyzrz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gmyskdjdr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gajhpsavd.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/geggzfwmy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gbctmrpdy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/ghkdthewc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gmwzuytvb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gesnhsnee.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/giqjsjzca.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gkgpjtwsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gfphoctvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gsdvavgqi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gebaidoiv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gfcrcgrju.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/geovkcigx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gegzqslgf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gkttdaexk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/ghflvjaac.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gbcnerivd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/grmamuxdo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/giqdwqgrp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gowqgcpoy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gqamqjxns.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gmtnsjnfm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gaaryifoi.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gsrfxwtra.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gcawsewze.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/grabfcoen.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gbrzqtvgw.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghyduepps.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gafxvuuix.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/ggcfhdsnf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gvbmilztt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gupqehifi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gojnrnsxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/giqpztbxn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gmkquhxuz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gkcbhjjla.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gihefxhou.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gddgakoep.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gqgztlceq.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlgxacy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gaaytgwnz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gdjrwtrjw.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/grgfkstsw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gqvvpjooo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/ghmhtuaba.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gdjsavodj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gxzscmxrx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gldbtruvd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gzpmgplyq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gxwvwgmwj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/geknvhfjs.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/ggguasflh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/glfkfekbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/ghclacmqg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gouytpfzx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gubnmivju.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/goeyuhydn.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gztufeoss.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gtekbrrzu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzxwyymox.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gonkebpef.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gxciavemy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxwakiblt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gerkwcpfg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gtgyenfmz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gobjzccfm.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gbwqnojli.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/ghuaowxwb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gzatgygos.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gfkxsjwcz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/grqctkvyn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/geedizvoa.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gywmddobe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gujrrkfbv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gzrdphjdq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gkigcaotz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gjbrdykev.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gwinuhahz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gdutfteaf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfspdjbpu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdbjyelip.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gcvyoohhp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/guukksnyq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gxdgcgiaw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/glazrokzk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gxqxjhzem.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gjvlpdyeg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/glehsqqqj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gumdxqgtv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ghcpxkjxb.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gkqffiiii.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gwvhwzhjw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/ggqsatxoi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/grjououpt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gstfbzdgh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gvzwvvalh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/golqyotpz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gskfeqlud.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ghehxponn.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gqpxcdfca.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/golkeolik.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxzjdltpi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gefrgztox.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gxxyveqrl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gwjbungwg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gookgsfpw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gqtjrpjmg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gayfaxuwc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gwcsayqgl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gtnibvpsy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gvyadrxmz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gcyiyjtdf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/ggkhjggrj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gcxfjlxhr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gzewwtgem.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gcgssdcdm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gtbgkesss.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/ghibeivwm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gvnpeqhpw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gmbdcbjlb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gyrhfdfrw.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gppnlkgso.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gbquipgsu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gxaiiyknk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gjewdblbz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/ghzipkemq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gwbdroylu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gbnqxjhbq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/grvzdslhs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gfbvytjoz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gdbckjncs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/glvijttnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/ghunxmtfr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gemgyothn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gsryynlzf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmfcibbru.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gpiirlczi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gegllddtn.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gwwrtidon.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gejbwzsgm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gunzhyqpb.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gslmyvlyb.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gcuhmmkzg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gxajklgds.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gkfwqajyb.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/grhsqgqya.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gysiokfey.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gtlyujzcx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gathsdorl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/ganacabkq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/geppwhpak.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/ghpdbibhi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gzxeehjxe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/ghkfccgqp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/geepmtfzh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/glgcmjrdg.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gxdgkulrz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gzncrlmdd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gaehdmndj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gsdkienia.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gciaszujz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gvipqnvjk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gqynyhaud.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gumzmzaxa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gngztawsh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/golfvrmnr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gwvxwtfxh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gqbgvejku.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/grdztedin.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gbyjuerhz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/gwhyoxkxq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gehadtmin.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/geyhcozpd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gsxmjqjpm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gkeahdfep.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/ghllufupv.sHtML


<!-- 参考信息 -->