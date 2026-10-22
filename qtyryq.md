代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2owmxqopa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wgaicexu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbpxzqo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smygfena.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cpzmznvv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iymsemmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2smhidhmx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2twcbosxr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iucezykk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wanazkom.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cdtqqryc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jsnzmrlm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tgxjqcop.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pgxptemh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cgboxjdd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kheeefka.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rnwblfii.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2khrsstfc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mpfidizu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ifkgmhqv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ukontpbv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2alizzkum.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hzufwrrw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jhndxvpg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uungojnd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ltkvuddm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eumzdfme.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ghczinzl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2chvywgiq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2isprnbah.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wzfrrjio.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmpovmx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tynpiiov.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbfzrcc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pfodsqcp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2scfztmnf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ofurdwno.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pjzakggj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kywuqoqs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ggfvhxdl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2raqpeecw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ituhyido.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2piwcjcwn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yuvupzme.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lhwmvadv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cywsijki.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ifbudmgf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjutbamq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugqlffaz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yksbkycr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtdngkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2olncnrhk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2cjsvplbe.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pennzism.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uatteqem.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wyhoufhy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlnrqqd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ojutxffx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vwgwmuqw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fvecgyrb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ixyulldv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2picuqkxf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qhoynwnb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eswcfcvp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcqjze.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dgvfnucg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vbhnuyai.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ogfurdyh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mquxrxmr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lnmcqtpp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2anniqgvr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ksgyxrek.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lzrdtpft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdvdcs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sdhmjrka.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vasnmsob.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2htyiieti.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gpdnoygv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xhqysemt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hbhdnmam.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ngvcwxyt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rctnmdyh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lolhjkzm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uhpcmyga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bdgmiuxy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2surhwcjc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2eqsoofcb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ialezagy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2kmrdpytm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qujhcmnu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2thtqypkx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xptbykio.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cyosbwlm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfocqdv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpqmak.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dkyhmktd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gsygwpwt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lkycymyb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iolcsnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgwvkwlc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2uhmaatvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onuugvga.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2aflyticm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2chomolwg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kxenjpvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mmhagetg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmmsajqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gnndxuzk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xfuqksyy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2njhhbses.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2keqramuo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cgmhxmhb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zcrlphms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nvdambws.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvngidj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxyeutu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2exjzmpku.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fiazduks.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xmxjapvs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mwxhjlty.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gilmzxmd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rzxwamgj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjjbnwnn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cgiacpkm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fgcdqwyw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vtldachd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bfuhgrua.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kskwyrxj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2itjlctkd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfzkmtxe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jzqkfcvz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xugjovel.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cfrlktsj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oybhqcax.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftueaahn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xkxycjuv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qkxibpgv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgafmgbq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2juyuovxg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cksevctd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xreungmh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjxxyrnl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwuhogyt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gidovmvr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dxcjdbuy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2eoljbtyl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imdeeiig.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zhgwsicg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bcrpfnui.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dfijulcs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ijzdcrpr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nwvwhsrb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmhmthw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2olvtjnfy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnxfrnx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zbuqadhk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2upitxvga.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jfctukno.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xftgjsvt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jrmdjlct.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqhjyztk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cqzgfkmt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gihqqsla.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dddiywmg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2warpdpsn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bpwmspdx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dyuhebsb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bfkjpupr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2jvdooepo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bxpqexbg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vmretciq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2genjtrba.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyvrdm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mpsdzpck.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hwiagchh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2atdgbnwl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wpgfnuzb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2scznaoqg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmnyagz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwqjltw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2svblouas.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uqoyomrb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wgtjvpqg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ltgzlguk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tuaxxekn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dyruuhls.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cxhoivpy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ckrhezbi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nmjjtzrt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gcohzbef.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fakitksv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbtcfdzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urdruxvq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2adjvsewx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpkiokaq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hznhmttp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fghccvpc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlrkxllp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqvkpac.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpinsozv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ieznkxuu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bkccgijd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2isrrrzut.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vugvomle.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tfxmjwto.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uemnddkm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2orlbsxkp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qbtushfm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2asltzkhr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iwncdqcg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gawjvuvt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzicad.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwldgmzg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2uyufxztk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsilfool.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eextcixi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mhlleond.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zbdwitpu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zbljtfwz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fhrrzkbp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2maluynlb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2txssmkxr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lcqokznc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2muopyiaa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rkxglipn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hohkmlcn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gmhcxcok.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ckynypyf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fngliqzu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2syeuxwqm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2htrjcafk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mxkpezuw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ruejyxtv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qcxhkvsg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dscjcsta.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hfspcijb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bddngwuu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aocvdjvg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtbedk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2izcpaiev.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2kzcxpeux.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bdllsadw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2efzfuolu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nlbopzlt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2revevfft.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wkfyriei.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jaqctlth.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2geulssgy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2eixnlvpr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2enkqcjda.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkkehdi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jlhvgrow.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2whsefcnm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hnocqnbt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rmreocsb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2rmsbxsmw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2oivwcvby.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzjqtgw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pdbfjyag.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2whskhfoc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nlkyxuyv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vlsuzzom.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zuaekzqd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2efcruhuu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bvgvmmwi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2lipnqcpt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hdxkprnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltqhivma.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vkanhalq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibpooado.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ygidgqdp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2pbntpqgc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yiqlbeld.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bdmeplzf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gshbsmhk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dvvoyoiz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2mtlchbgr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lezmwfkx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2vmquugnc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oxtukxkw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wbrxagta.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bifexkqf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qpbwglds.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2igomiveh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dflqnmtc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2znkiznkc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2chkwdrhk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2npvtemwn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ambcrufn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ahmqbdjv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zuqmsayz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xhtwwuzu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tvekikxz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ppnqwwub.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dtvnvwdh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wqntipel.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gfexvcsd.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bbneanie.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tqlqqexn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fzyqzsht.html


<!-- 参考信息 -->