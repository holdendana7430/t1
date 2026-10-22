代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mcnzemlg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjaslpoh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2laupnbcu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ifavgfha.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2evxotccz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sypekpld.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ifmsnvod.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cyhemmnc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cfdsnalu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtvqbanr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oreszplc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2stfjmphd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cjlgbhvk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ybwrkjmj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnjiubqg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kngclxac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2upivsyyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssiryxrd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zqnpoxqs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtempbik.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2poklotbq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dxeneuyc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpwnhwnk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cxspcwwc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gltkvaxv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zcepotns.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mphjvxod.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bobpywcw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ekivqjii.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hoseaftu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2oceosoim.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hxnddzlc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pcbvzwps.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dimigksh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vhiujzee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceovnjql.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ojxdmydf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvuzkzfw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rkpgwafa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2trfigpqk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rfqeualb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeoroftn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fbinnhiy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cexmgvzt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uvuqlamo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vwkatppt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otdurffg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwqdiyhh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2thrdhwma.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mihxvvnc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hhwmonni.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebmtmwoe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnxfvse.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nvcctkyc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2msobgoso.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zbihtubc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2avjmdtsk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ritfebfa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdxfzf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yscxhjbh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kuadepkc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ijfjstci.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gxzfcien.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hcjwftxh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dadtpfgo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xoqsjabb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yqbbexqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wbcezolm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jvprbeya.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yecvclnw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnrkdboe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2keifvhee.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qkuvkhnb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpjgfete.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yuzfngdh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2eclbmtni.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vrzpxnhh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wukopvpc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2djhkcetg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lofhmttg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vhjrgtax.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2saebqdij.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fzntsbcv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bvgqbbjj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bfxtvehx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yyumnzaa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tcgsetdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmlzpvsv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rwufrrxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlzenpea.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mknulure.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ctimuikf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zgtysaok.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qzonnrso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtwyqkxc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjoxhrga.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ztdavpjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tsclexxq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uszoooui.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bviprxao.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jkxplziu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buuvaglm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2euchsbqp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmeyymxl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cttizdtv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mysmhuux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmucwudk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsyhiggd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ravociev.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kmehcigd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2huhvtaoi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vnzubrbd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2todjxuqh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yejrxhkh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vwnpatgj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tudsdigt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mmtmdwpb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsygxmos.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kikasxpy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2swojtlba.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlfangrb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dhjhkttp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pypovjrp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vubxqrnu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwigplvq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdykjkwn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tygkeovd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2hjfigmaz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugqiiqxe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gctlqdiw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2spbtqxhd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoglvcns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nvevpcum.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2affhsvqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiubephk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ujvsrkbu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hlrhfgls.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sdfqrsjh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rctdjhio.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hrikzdec.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wpiupdyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hsiknpyr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gjsnsdjt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ygwkrcmj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zswvxoim.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fnpnenbv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tuiamnvu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hxclmxkx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xtuohaxe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yhckblcc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2grjfmkmk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2konfhlzw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zwwdvbpl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2yicpwrpx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ncgjkggk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2amgqsrws.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hpkxdljp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2spavdnss.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ofbieeol.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yimewvqq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ddkpnupz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2aovjvyqg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hhuolfnj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dvwzkzrk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mgvdpdti.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ehdvnlwe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvsvtvko.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqcmdaez.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vknoauqx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2syraqazp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2oaymmozb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ofpwwlla.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mazgufkf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gpgnnzvj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nvgrvaqh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aezsblal.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fbmnzbxc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mbshxwnz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jcajrjqm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2etqhvdqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkdcthmw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vqhdvykq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jopvooay.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ryhhdapl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gshzmrwu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgxiansq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tpvkckpc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cgbzylvt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wiatapzy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2deeqflgn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zkgduuoq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2izxtjbrj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mrxovgyg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktanympo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yqeokrqe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2iyuyyexs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2mxwjrrre.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2reqmjqze.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbqvkjy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjoqzzy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ahuujczj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2eectoirk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmznyp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2pjgihkas.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bqyujtak.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2szweqwld.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fwujwcno.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fshfvuqh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yosrsick.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tdkkjdjd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rtiagmqc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wpejqery.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnbcmdtf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rcdzhpoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nobhxivq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hcxcujwj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kcgqjjce.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2urpfpdda.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvquzhqe.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2geqskagx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhsbabd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2atcghwro.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjldzbe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vxxffbyi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fdzdpxrc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kluzfnyr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rnzhbfqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vnewnage.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gcjzhmne.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ywpamgja.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bkbxzptz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vuytrwfu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ekkaaqrf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zfvhfjpa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2kdgzdojb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2urrepenq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2upuqrdzh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zccuzikf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxaidsd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ysburswq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cjsnertz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2otlbgaam.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgulzsv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wsyggwbt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2wckjlnct.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hpnwmhbh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iptkwzow.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jfmoooxo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wmnectih.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bizfyori.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nefmmlmo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2klongcnu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fcuiaavv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxsgcxas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bsakmwdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeekxyqu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hspepafh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pifmvyuc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mvrvgnrv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2gkhlqcog.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jluuiqrk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dkutabty.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tepovirg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2qbelriby.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2rhxkizhp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2oqnyirte.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ffucjwui.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dcyiarmg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2yukbftnl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kdqtglva.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hteuqynv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rnhwiiji.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fveqvyxs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2swijjbff.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kqkeyhkh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2zlddjejt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2yvrmajyd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gffdbteb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ezpevsbs.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rrbmxufn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kppbdayp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ppiajvrb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2krdgckci.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mxvtcsyg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lsvaqled.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uouvjsbm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzjgjfq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2qaruhddu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2hchssqnj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpxkdiw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2amcjwkkf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2mfjzbtfx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmezkwu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zvnwflmd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hkgdlieo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jjzthpct.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ltplkako.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zrgdjixt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nfoorzjq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2apzaemwe.html


<!-- 参考信息 -->