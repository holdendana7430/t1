代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jrxlmncy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ywqxqwiw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qfhjcbvc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gvydkblk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vtuhlgzi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3unxnrppm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hjqywpqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mxngknol.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ymghqsah.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cozpdjbr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3flwoigbd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mrxquseh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzhsuuzq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfdufmuw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tazaswjw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrfsxxrl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dhuycyjt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmapljyw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3empmcems.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lgkrnbei.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mgnkvjen.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ryqymkvm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zbdapxel.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnpkxwgc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khgrztes.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmmlvul.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3aeliwnbg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3publcayt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jzusteho.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vrcnaisn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zkuzwawb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3povtjheg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ivdfdwll.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xujegjnu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pypbmjir.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zxxsukdj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vdtuyfpv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sgvrvlso.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zudzupvu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xnndzxoe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wvfcpbdx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sgfiepti.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dsrsqlnw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ckagdbgr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zqfgwqwg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwjqxfre.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eodkwzuv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qgdyfqya.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lopzslbw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eriwjgdu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxjpwm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fthfiwxw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xxwvbuhn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fptupifk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bddaxgjc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uyrdykmn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bfcplkel.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cnpfobla.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3trbkldvf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iceakmup.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ladapkhn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cuvesdkr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xwdonyul.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uxzlfezy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jlhutjrq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bwispvfa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rucigcfb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ufvpdbtm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3oqzovpql.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yucqdyhl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfyponc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdwhrf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ramxirxq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zgvymnfe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3htzrhdvt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdurzxwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mxlmalhx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbfqlhm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hamvdzxn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3airbluxa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ylceuvee.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3owfgpjam.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xeydcyra.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3esotrioi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qtsdmwzp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fbtjudip.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbcvsutx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pmuwxdkx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mjmjzjkv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qbmgfgue.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3whzwxrbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfuaeieg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3giyyhxoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lstcsvfh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3psmyomlc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3klmcnctt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyxhpeeo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtywgjfv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrsdruoq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhhessus.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nivyxhtm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3njhoourt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ujzqaojc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qqunjrxc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kndliuhh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrlwvpln.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xjiugfmf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3okixmvzx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brrcdbrv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fhgejwpv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lzrzwoia.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbymcvi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lgbhjcni.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cpskrebc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ibgkkkss.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aadduguk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qgsilszj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fcwgahnn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jsabrosk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vnetycee.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tpyluscd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cglfkxpv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vlopvpuc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3thsmxxbs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uitohslb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoiaaqli.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwusdvuo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bexfmzpq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3uvihfyfh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhcjyncr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3aalffqsg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wvypjkxm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ggsngrop.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3riiswjpz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsgwngxw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qozsihqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cveooquk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3phmofyrv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnqdsmjz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3knbqxtzo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yjudlzkl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lbrhijja.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bvbdesbr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fvktmdph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgguuqy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fraufhkp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kmtsbybs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqtdsfvh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uosvpdci.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3glzlsfis.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yfarqdwm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulowptzn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqwvamob.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3miwnzfwi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3umxxndpq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ntyxcllk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jrggasli.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vomkdlwh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rcsjlmzh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gzudhskr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lnxndehs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uipdmgce.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3naqosxua.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3greukqvu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mgzlvfti.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kztjstih.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zbybnwsm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lvvdcfhe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3qopvygwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3kcybgudz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpvbkwo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3lneqydlr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mgyyhhwi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3lvsgalhs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3npyfnjck.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xdqrhvmq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3abbowejb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hejhsgws.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bugmioms.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tkevztlz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xsdwzvju.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dlgsbdvq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3cqnmnjye.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dibofioj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifjsafhx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wzimorqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krulzxjo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ntizuqdc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sacsfhgk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hwnswvvn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vtwsenaq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kdyjcbrs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3shlfobsz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wavpvjnv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vqiruqaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hqcbnvao.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wrszxtth.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jazorkwd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qpcsegps.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rmsacubl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uajorbty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnfqzibu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cqvugigz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nuydhkqu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pvyzqwsq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3agcplzud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obnzkkll.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dwcrspya.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xdfefpzu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yoigrhbk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kdxgcehr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kbelqqbi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fgkpjcaq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3edoolqxi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxuwvxay.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fprsshhj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nznwyfzc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xyalnnio.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mxardqme.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lvcxotoh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tpuaqoky.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fqxhvwvd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3aujpnohu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hcjkaygm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ysvczkah.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jaehfjrg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwqpnci.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtjoad.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3blkgidrp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aovojdim.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qewfdfxw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gfntviee.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3rqcebuty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tmxvirva.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3flavlsny.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3asobajze.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hfgobpld.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tlxanvdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3eunnyfly.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xnvvpdkw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ovnxlwfa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xkbtrpvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rmqxekzx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qtjhvtad.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwjvijz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dspiclwn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmwpkfn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ayxshidg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nczpbfnh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqbshhh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3usakwcqp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ulwlveib.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dekleauz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrfidox.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rrcuxmly.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ihawgowy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3imokmlfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hgtlvlsx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qojjduwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umoredfg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3yzctnxpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otfonikd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ugzzeoax.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3cajayibu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gjlvzyef.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ourlqdrp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eetwijda.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3phwpbswu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hmufhhyl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ghdnaxev.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ieclzfiy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bkvssiyc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3opgdcgea.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ripjvnkw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ckjckpdq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3wlqiheeb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3tgowkdku.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3lephwdbm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wygwjpnu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3zqlrolha.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxrkwn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3haltsvci.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3osefaeqh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wuxnslpc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jcyxecfh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kruzxmwe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3orqrshev.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hmgtdsuf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3pamshbol.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ownwgemq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3loyezilj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3vcerejbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tfuljluq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3trgqkupl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mxmdmzkc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3viazrvlr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3zgjyawwx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhptkll.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3nphlnxng.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jklvrvpf.html


<!-- 参考信息 -->