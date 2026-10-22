代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nokngusn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwhmetsj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hvfazheu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ujxmdytc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjhmgufm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qfqmlmsa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2etxtdhcs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ublajfdn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwhkgjrs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2feusgusa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2refskxib.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zmlmiukq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jepgjfeo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oeqxcqjq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nfbvasek.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vrbpdojh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2blocfxwz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jbwgfykc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ezgbrtjo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wvdmwqox.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rnqymqjo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2apdprqsc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rwdbakku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2milgnpak.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2thqutcjw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oodhvjel.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lqsmslfu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mwfzpman.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnqyhymn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wssgaexe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzzbxsqj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ahejrwfj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2kbfsepfv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qiyellbx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qvfqrzhi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mdbqhkis.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pcqjnkek.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rlrzbafs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nhjmgsbw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcohhfld.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2muvnxwmh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2laoxlsuh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyeshhtv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tnhusukb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uxdpougj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qyyqmouy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dvoxsoxt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bjqolywu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nqmufxtn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iyyjnirk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uzctscdt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wmkboodt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ifzptxml.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xpjowxko.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pqxhkxtv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fplhkyqp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfexxfek.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jwwljlxo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klvwkpcj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gaugepso.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zoreszwj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ytaayuxh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ijltfwrq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2phjojbtp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ucymmsdz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bxijmoiy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrqmjrk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2atxeqrfz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jooxgkxd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ugflljkn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tklgtkgx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzzijlpl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzpvscn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfnjit.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2etzdhnfb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjulqezq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qhuuvpfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2muaukixz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hdvobkid.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pvbyvumj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hsoakfvm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hnknvsxx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2uutzuohv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ogjmpclf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kxnohtiq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2aicwjdwg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gxvxzxxz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vkxcyeyc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qwpedhjf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jhmpdvlw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jprdcnxc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2culpskex.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hokbqdsy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hodjqfjj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bohkyrif.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2keusvycq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2twalqytg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fdadxnsv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mpwdlyjf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dpucsdyx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ivniuiwj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkbevbg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkuvgceg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tuzumqgq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uaziqmsg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ebozqtzs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wfheiokd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkagxqpw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2benowqny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjbvgoyc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xsmbdkkj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfxdyuy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvudfsz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nkpgjpnb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzjliyim.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ewcspyjy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yyimbcsw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwgvwrba.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uafyirkh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qorxdpqt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2duiwkkib.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzqeovu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2extflyfd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hftwcyqf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crzrqgzw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xdjsjtyg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bwaxsdgm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2seabiqoz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hrumqkbo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xchovrbr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uofdnawk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nxxxskse.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kdvmatmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bpniglvp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lmifhdcf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2isfksbab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ztfggnjb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hzvxpepx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2krecqdif.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqibwu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqfodwdr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2apqjczry.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rkntkexe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jrexkcsf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2idlkpvvs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uocqyiqs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rkxudtjn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qoxkgcba.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mkxnplpn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2strbegaj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcgonohk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2iotwysnf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jgyuhzhp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xyxxscjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiyhnqbt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2brgmdbiq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gwqeedtf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2akszjriy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sdbjvrwt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ypxwrxkg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnmbnpk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2iwkktysh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ybxaykwt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rygtnzga.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fyvsqiig.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zpbxnwzt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2omglpchp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dxypeuex.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rcevydoy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2peanzehu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vqrwavag.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jexrwmsx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vtkctqsa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jduxdmwm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zgopveey.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dgdeqhlq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ecyjwvqv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wabetgie.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ejebecjp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lsogvdey.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fpabgyjj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mpevegbz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2rknvrqhw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2gehgcwhe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hxquhmkw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2awxiegrv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2auhslmix.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2walsgdld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lwmbatuu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2leibdfia.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qvfiqtvq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lnbinedu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qnnqgetx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jgcavrbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yokvtcgw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yokgodzw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2iqvzzbww.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vtoidhrw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dvrvrlgo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zalmqxbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmdifzjf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yhvcdjyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzranptr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2gchoweqp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgshhorh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rximjwzn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jbpkvdrg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elcxanaq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bfiupprf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ddwwwcfu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lubusndi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iuormzrb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eprdgdom.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjydiofe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2nqkotmua.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbpiwrmb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ityzokqa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kgogcjjo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2badfouqm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pknprhld.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfyugpoa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2nlfiazux.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wlizerwp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2xsanznyp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qdeduzgm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gxpgkdyj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxdpdav.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2lgwkhiiq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hqaeqewj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vlxrpvnf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bciqilxn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2najnniwu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxvslcnf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lidahopg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gpqtjjad.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2diaatuem.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qtvhcvdb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2iwtdkcfb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mtpwztou.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lgegwjsa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvxvlbk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtejlpvp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zzqxizdm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrtvsla.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vrdnlwnp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfxjbvt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2puqhpsxe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2evpjfsbb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mvyemsqn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dhfhottu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2uxwdstqi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zzganejq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mufohytl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fwbqonsj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kqmomnht.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2bzljfbqs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wdoeyiym.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2vowzcxyw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2oaqtiftp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kwlqdsqx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pbjrhoww.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2kpgvhbvm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2utvnyvpt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2sojapvyv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mqadennl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hqtxqmjg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ouaqqlpw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmfrfi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwbcugv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zmbzwqnp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2phxbobja.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jspjlatb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2jxomzugj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwoafugl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2agfumpqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igrojhcy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2awrdiztl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghhphdma.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hiobszit.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxbamty.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bmlaypeo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2isennxkd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2abtjrjcq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2jfpucniu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2yntpkspu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2elcdoecg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zgsfuovg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2awhndjpi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kajeeikt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xhxxxmlc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2znoqbywn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ynxrwokf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xfzbvxnn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2vgcesdyp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xvacxkve.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pqghycyd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zghdjfvs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2scpzfgga.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2quzpqfqb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2efudkotx.html


<!-- 参考信息 -->