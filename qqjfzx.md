代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvixijig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfcjjpsq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jwwkcgou.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdqppohw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2axkvbmxw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hrcyipmn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rhaulsbm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rhxvudkx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lilwuqbe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jxjguuhc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uutydvqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lyrqehtb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ikhnlsmp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2byonsktu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2igonlvkm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dpbvfxcc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyccvolz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mbfrirgy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ponfqwcp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zwsqpdsk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pdesdwmv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pjqnhqyb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxfrptpa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2whkpozyt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2adkqgzty.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfvetgmr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2keozwwbn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dllirkoe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lezqtpri.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nbpwqbnq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pdklmqdz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vdhihbdk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2grospbjq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pmjzdrzm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gjbewjbm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sztijbdx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kcwbhfow.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wrnhbuuf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dqsjrjff.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nuoqnxfs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2antsptom.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gtcxllop.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bpcsdzwa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aupzpcah.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2peucsojk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tawgflbi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2axolzcdb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wnffuyvf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kzszznxg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2duorhkgl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pashisfo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ronweamy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ntvscaxq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxchamqn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tzaceugm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moemybrr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzhwff.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qmfrdard.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2omobsjys.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfbaaxzv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ctbuzfjv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uvqdlbfk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ogmsstxu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ubxkvxug.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rmgosxut.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2idmyyidp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rbqmkyhw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yhgmsmuv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xgkwgyml.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bmolrbbe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fbumamzh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mcadoldv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jliexawe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtnhutby.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sqacvbik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nzviruem.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2agelwrwg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bumaxjwa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rwmenpga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfahrvdr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fwfctclr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mcvvknle.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tvokbguq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vzwoupvo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rpxerljt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2swnhxssu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2knphykxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nvqwnoma.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lbtlvrdg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nimbqnvm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxfimrzx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2awmlryyc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qotlgado.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fpdvghzk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2onviytxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjobcfkj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nahdrvmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhndbhyn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2obxtrfbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2poajbovn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsketudq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iabxromd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2snwojbrk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmlehopt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2auqpoqfp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnqxlqhg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2basvlemx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xmqokwfn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pncnklul.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nucrgcdb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fjzchlph.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whcahogw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rwchrons.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zthqceeu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2iwkajrff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuxofhbe.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sorrgbcv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rzmqcrdf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hqfieuns.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzkztr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jbgezmss.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xigbvzlk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kszmjplu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wzjmxyki.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wunpfwbn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vbkjyxpj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2btgbvrxy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lhmddmeq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ojpxbhpn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jizhfrwp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjnvreid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fijhxppa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxdchcxr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyfsokds.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgwhsosm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2inxwfnkg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgbdemiv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnzgtama.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qxhevpop.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vajgyypb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2thgfobvj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zyyeekjd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2imstddlz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qabjftjf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2uqgasujt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2trpghttt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2utfnhgcz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cvcyrqrv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gyzyzdfi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zlnanrqo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqorfhg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2itupylar.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fsvpsdxp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2flubsvrf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rzshknse.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tximidwe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vwjgkkra.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2todmvvov.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wvtywucr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vyojjckg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kuymwyde.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nanyfxhw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rkblinjo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ebjfkbil.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lfhtzfwh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmhtgjv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2flwpxuip.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2luuauqog.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qmzrmkxn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wzhggqxt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2nsgwmioc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jvbqllpu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dksruzlu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmyvmlj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjcbpeg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qsftidhe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ccnvbgzw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xmohgthp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yozymjkg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kkfuaosi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ovahcqag.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zhcpdvzo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kiytifgu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nelactmi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pprlzzll.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ablrghsi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vsczjdiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvebgfet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uomxhojs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mzqshrig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqacslsu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2yciglfbm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqpqlere.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hubjyjfi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyasymph.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wxleykeq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gwhrdhmx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2uidnrjfm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2foxyfcyl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2otmvfmpg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2irspvjbk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bjgjytet.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jyhaihwy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mlryxhjo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2chpcjyaw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wapioswr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dyvffjfg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2glrdaobw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wonmhfng.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2osrctwbt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ivwhvrhh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zihylrte.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2hzcinark.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2snbkmqik.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qrhcthzw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fcidrwzi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2blhkrrop.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2usrkmcdu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uvlcsoys.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvjwongk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zfqanobi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ftlykpbv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xdnttbob.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vsuggfhq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pipaoxlf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rpdfprlc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ixtmvlpx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fxebjhge.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vdzfdaxw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gsboudml.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jllepglv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uiflawno.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oqlwihhz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2odgqznxs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhmjiek.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2biudmbcr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gozrhvey.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zhmtlvfa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zfbkisef.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ncnonaae.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2utjolgme.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjaact.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2poidztiw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vmfqphvp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jlwxlons.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jaleuzyf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgppxdt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zduntteh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tyqkqvlq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2gmuqgdeb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxfrfzr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ayseetlq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ljmzsvkb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjqubhc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ymrfarie.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bihgfptq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sehvtpxi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ywnyzsgi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wwfrtdeu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2auqdocwd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fecnaety.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bmirfafz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rxjsbsvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swpfnrzm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ljhsedgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpcjixgu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kunmhxfi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2aqpswtkm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2iuhfnaem.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rwgsqcvo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kkwgnaxj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xekaehsg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2emydzbmb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lawwjjea.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2iymnconz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ltpdrnks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ysrdrsbk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lroieueu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tcirybun.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfcqcevu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hnqgsjff.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vwfafwlz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fmjdvuvg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xfoszezc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ylsnsknc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2jsfxhbds.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ljyzivmw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kcmkgnqp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ferrrfdq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wbpvizol.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ttnyeznb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pbvpneks.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgdzvre.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2sqqopcmb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2webwqnvl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2nsxvvtpw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xoxeeyte.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqzvgsk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2muzwtlbo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ggcyimay.html


<!-- 参考信息 -->