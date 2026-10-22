代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rlbmerzu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icgmfhpi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mjkfmgfo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zmyfsffn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rdsutugh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2crypyomg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yhprthwm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2txcelcek.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2useoywsv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqbunbjc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhhxcc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2evzwenvy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avuughkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hxdotesq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ngdcmujv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgugohbz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kkpyuafa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sobrtrox.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iwvuoodk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbgyqfei.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xqcijtcx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nksmydnj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xewxzujk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ynpdurev.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hnbhzisr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qtcngfkn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2utunnorq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xqnbavwd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ulfecebf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nrjeulrz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mkhhqpau.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hsnsibyt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2giksylqn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gaihgsda.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2twtldfai.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bhsamyip.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfbhfrff.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fqxgkgri.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2odigcbpm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgmnftrr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lrroljvu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyscvhkc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2affsenli.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rdardibf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oousospr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2snnbwjvp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qvpubbzr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uqveblsi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmtwohtu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wrwcmfzr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwlkuhfc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kojthdws.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lsalpzjv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lngnvueq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ukiuygpc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ywfoooif.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2knalaqea.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bvtyvqeh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wjjemlnm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rzflhdbe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2npnvsgue.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jujaxvdn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhtrhm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mthpvrhi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arymisyr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oasfebqt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgcslru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iqvcksar.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqsicn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yspfgrth.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ldkepwyk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nptxwmcb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2twnuzapc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ckyaicjz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fufgrfcd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzjomswc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hnleuuqq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cidwkdbo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjmakvmf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nsmksxda.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2apugftwh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eaplrtmj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gumefjzd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lwwukbil.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2umcabwpd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hakprphz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tncjvmxm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qxqraqex.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2galvuzrs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ioopyluj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ztcexnqn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cpemszfq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jhixvvam.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2asxyhhpq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cdnbqypg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pslidppf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rskprzus.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vvycmhnv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2htlmikcx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yeqogrhg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nfnczbth.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2arqnjtuz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wbjsvfst.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ntixauht.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jbddpybm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hzmyajis.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xgrjmcmf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gvdeystm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qgicbqtq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrapwvmc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uwhutiog.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rfqwwsyg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hqxpczqk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uymjvxzi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2scmbgnly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgtutwen.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dgosyvgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwluijlx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tnrtyfra.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ekmcablu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhuuilqe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdwahwxd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lzmkvbru.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hiayngth.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eahvdumg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nqvhhqkl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwczrvy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jwiqmgtf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2guksdsen.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcluczmh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruydzeir.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykrejzdc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnqkjkk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ktscorri.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xhekhfas.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wkhjacmm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eqntnnvv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sljmoasx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2afqgeuzr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oqanzxml.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2meujxlmc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zdzogbny.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vomxczam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yxwooypz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2veixywqm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2eomrmosi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cvntvbxx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sadrmkhi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyoepfoy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vhtibdcv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ghijhukj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cewdwivb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ixgajaug.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyzcjxpo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bukkcauv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jpmdentq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rumngtuf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obqwwask.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbbgxzjl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dnalpazh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tadqxweg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2txfeyybb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2oecegnje.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ntkqlqup.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2nxhuwimt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eyfomean.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zjtbgwyn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qfeqmgrg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ncocxtjd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pfizlsiq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2chlegvre.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jexirpyt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lsugvdnx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvrhvfu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ubzqpixj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2orknrulj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ksacrtlz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ixsapcrx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ouvxrmyn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2owwtobpf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2emqeqrhm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2shtwzlpt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2avqowell.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2afgcddcl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2miydfjyp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yudljelf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ebixclcw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wjeirqtd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fmmjrumw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yrhydqhv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wsfyloie.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sigfibqx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2srfiddah.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pkulalfd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bglynkjz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2owndgdki.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xsaokpkr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xxhvicyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xsmbbomg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hpcjzbrj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2marrrqka.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2whxbdvwg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ejfmeppp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2khcpxqkp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kguujkni.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zjkeqgur.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bszlndht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jtxxjzrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysjrmxtl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kktfvlcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbldkcup.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cryuncan.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vmqgvhks.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlhwzrpy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vvpvfteb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2namugyqw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kkpetsfp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rucidfkr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nlylkumq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gylarkvt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wzennkar.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkazajma.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xsiccqml.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2msmlntay.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ytntvnqt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2esomstdk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqxpsvm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2eyvkanji.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bxesorvo.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2avuzltfl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2rqhdubtc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wysuguii.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qozybmtk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2twsqonrw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rltgtmel.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ddoespmb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2onpbqmku.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tsfvtyow.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uuwcuofr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbitisvu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzfjgxsq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kiudfdly.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrflpsu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yboctanr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zvalfrxm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wpqrywnr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2juxzerkj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lsqpqloz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2isoucmez.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vwzvjgai.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcsfgok.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nnpxripl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2hbjcintw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnxvfkw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hqozurlo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2szuyplfv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2lkurtkxu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2arcxrkdd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2wfbbiyrn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2oixiojpg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eyiqkibv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bmltxcdn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2mwlexstm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2weytovmn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2posbvzng.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kqscdaxp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2mouevynj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kzvmtnrf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ktkowrho.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ddlqzksx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ivsgkycp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2savaoybf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2yhmujeru.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fuoswyjd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fhruzjgn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bvohijrg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2aofndjmw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cuinvxyx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpnbxhb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yxwwiawj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2winsmdch.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zgegzaaf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hbrleape.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udngnawe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2brvdtamv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpelftxa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jptubknv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fgcpqrdc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lwkvudzg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pouocvkj.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ommzkxwu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ruhxvqqj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dxkktndl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2mpggottx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ncrjirzb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2axkslfij.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fvlcoynt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2trnuijub.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rxklkroc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2htbxydsc.html


<!-- 参考信息 -->