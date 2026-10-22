代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ebfwatjp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lyyppgwc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wfnjvzcm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ldwwdbjy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngfqmtua.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bglufrtk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sjkxggxp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ozjthiub.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2locjnbdd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ssqfqhxv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xkfzmgyt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2prxtvzdz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pzthmzen.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkcyhkfa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouzuzufx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2idociunx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xmevonzv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dvkvohbj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdqierkx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xddtwckm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pbnnutvd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2acasjdwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ndfurxgq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvxnvjn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbwnoor.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qozvfpet.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlvfgnqj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emhpcxky.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lhjbysdj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2svweqgts.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qypvjxwv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qapzhiat.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hhnzegma.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vlfipncs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pgmlvcfe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xudduipo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bkhdsadg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qfmshdtp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2extroeec.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnckhywb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fmdvbhkb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgitomri.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myfvlmuu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mrcypxyy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bkxkstix.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qilntifg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2whzriqey.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bpgqjmhy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rgbbfghg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wjwndrji.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbyzxelk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqhhbilg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eduvekwj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cyjmosyj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iwtkktkh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2frszogdn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjhsivw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wogkamgc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qkxgdtvs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gkssjyvx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lntkgvtb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cuqgkhfw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vaavulbc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tkrfwnut.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wtdnqpdn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2inpryqye.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2batjfwix.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yjqyslhu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sxzqqsld.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bbvayzxk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrpcung.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jrivblzr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ctngsktk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2afidngph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2owcanrgk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vmddcuyo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yofwnarx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2phcawaqn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2iirupdgr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xeyrsheg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qwhmcdvf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gacmmlhb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vjezhgoy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pvxvjtkd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eojnydfk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mhhebxpr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zeurtfjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2csqbdtaw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mozifuwi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ucsqpofg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2icjkgndi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvhhxxoq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fuwezrjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkriigfk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ltiozszw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mbxkeaov.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkziqxw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kguzkhio.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxbdrepu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lkuerklg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mgpgeaxf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ifmnicwu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofugtpku.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zcbmodcy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2piuragbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzftgbrx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mvddslhx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zyoaylnd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2losczdtd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tbgftctp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rinnlmib.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfipmerj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sgluvlwo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgeijhb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mhxmwezk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cfmkfbqi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sonangko.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sxzlsdvu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mvffzkhw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wiyrfmkp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dijsrhfq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpjkzstu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bvemmqzf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2epyteapx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvopglrd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rpjopcmv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqyztynj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xzpubihv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mhgjzgna.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2skestgxj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zfkdvkzq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dhigqtqo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ofcexert.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sylunhbq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ababncmw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mwourmse.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cyxusnyo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wfmccdvk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxzogcaz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wsdizuey.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ddfcilpl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mgsehpxn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vmnvoqmv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2retrkqos.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uqxiizyv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lfoffywn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xjilftfz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhhvjl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qtnhglas.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wlabkdrq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yqaipulz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urfwcneq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bhpopaxs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2melfwvuk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ucepsnyv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wifnyymi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eoijtcpv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kenuehde.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qnrlnbqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2szwchsha.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cmlhzjzv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2exnewkeg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2muytryir.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rpxirgfy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ukzeypue.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bjdvkrak.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pvsjwqrs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vznwxnph.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xqryqbid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nsdmcrpm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xobhjwts.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqwufcgn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ogpvqpyo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jtjnpuez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eiabzjja.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2bjxeebts.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2luvgqgyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zwcvgahs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fzmiuhni.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jlvstnpq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vqjlqoke.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2heltqfif.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvhsmei.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2suoenxwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzdcodpg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2cayeqdqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfkubxgh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oknixzyx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rdbwprpt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdvvjnhi.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jzicjnkl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcsgwgpc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjbaos.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yggylbul.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pdjfdnxk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2obznsobp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2txapztzh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ihsrcrta.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vzwobbrw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjvlfp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ztfsmtrp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fdtapact.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqvejxs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vhgqbxpl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhnjkocw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2uesuevsc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2vftdvitm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ygpzvwfn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjferkbv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ebnmlfsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gwllbgwk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cppfedyn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fylvztnh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dskhkirk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctitppdm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhykaxok.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2koegqxuq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ingvalgx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zkyualsu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xnfcgydd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hyjghmhs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2aqhxoywx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzncjqay.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dvoavxti.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zzcucykr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mcdafoqc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wrlftuuu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2boinnxvw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wjvcumvn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2akfcplaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uajnxakc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xwbqgilk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gmtaukkd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mqvszuov.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2seakcwim.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ryaxfgtt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xqvtcxjl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ouytkjov.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2kbhatrqg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2zavnmlvb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pmgoisgz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2secuohvk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xdibmdtt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wkhihlef.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kibonziq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2hcokjlek.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2xxtqagbk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhwngpy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jdurfbhg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzicecd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zcennffh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2quhxmrlw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hdmsjtge.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pivvfzgs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fbidgnnx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yytzzejv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yxgnwguy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2dndzewdu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pliibhpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjeubsrf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ixlmpkqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoxisjir.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2nbceurrl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vpawpbyy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ovujffos.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xkqyyjlx.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kpmknzck.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uslststp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vkxstalo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bgiiuzoc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2weizwcds.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nffqlxqu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrxhkez.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2brfjcykg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tohgcakf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bnyxwusz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2thmrkijk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2casmwulx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrknpt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2zmelnjsx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2szycfgce.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xciuhgvq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pjirtslv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gehvasga.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzdwwf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zoewpupg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sigjaeje.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vikownur.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2psgsljaa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2jlmlpvye.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nifojzed.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2dboxghwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pscquhsp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpgqjvl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lbnmsmff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2taxwuxsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2onklnjze.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lvpzsikl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ohqasint.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vziwyiyv.html


<!-- 参考信息 -->