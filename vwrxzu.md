代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hltkocpe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zwombqtc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfngbkeo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuasdphz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kzbjxitx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yqgnoaci.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2igalnruf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kprvwuvn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qxtmsybn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lzuwpovq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2awwsjjll.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzbinprv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2axxpjbzm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wjybweaq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rqsyoogg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkndst.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bfpmysxz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ahdftkbd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rrbypixp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zequmagp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yukkqiun.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bykpavzl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nfyfsbqx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2khyedatm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzelrvws.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgngswjf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgbbuuns.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gpxtoxbs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dlpsejbs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2afkhnspy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2exiaravn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bgswgxof.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ssoydjhj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqnpjfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwyeuy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rcpdeaav.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceturqli.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkcjdrx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ogxxfkdv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gbzyabjr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jngcnegc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hqjucfdr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bmpkxziw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uscjzpbj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kkpdqmzt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wcrhryoc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lxudlvgt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gjejjtgo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2msoxarpz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bvxqixvf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jqchfgai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccpapogg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oxgnfdqv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pnrhhmdk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vfpojkxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qrckkrbw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2isldftga.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjbktjef.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbrohfqy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yairhaec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhempxwr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxiygawu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yikrlyea.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjeydlw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jktzjcez.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxqiukmq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2taqgcqwz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mazgjoxd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yykbywxl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvklmgsi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2emtsohkj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2durwwibx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rjnxtegx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zjnyfcod.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbrggza.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bcfwckyv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kncyspzw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ihwicldw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qvkovaka.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ijnaveix.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2avevchwp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyqumayp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gdkmkdwj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vfequevy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sydnpbhx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ldpaxzgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nadoguvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djdtmocw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vytsxepn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oatsxbvp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gqudkvqy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjzrfvn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jzergism.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2emanxhhh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2frozbwuw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gtijujga.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yobfvrpx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtrkrfo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2habpiukm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vvicmxpg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qpcijdei.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vxnkvfat.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wmrnrmyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqxxormh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rthpqmkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chlkvxzm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wefiymky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tpukxovr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ufvcjafz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxxlpcqf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyeqqufd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ivmrmask.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xvxwfmdx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pwseorzn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gckkkrhx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oxuningi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fhwtdnvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljslsjya.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mtagvfdx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljfrrgkd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trhoduoe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2crduqhqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fxundnko.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ytsqwbsi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kgyagdad.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sgpkxrtl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jffhwbif.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2huwyytux.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ttffulfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pyztcpdg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ombcteel.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2infgwocp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cjgfkkra.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2oqilthhi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bwgbtnis.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oumemyvt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrkcbbno.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmcutfds.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kokzfdzz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2sjosaojp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2guasopiq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilqqakpx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2swoiemob.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2chsbdgep.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzoyexvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oxhurtag.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2omxdqtuy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amdiodvp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2retphjhr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jubyortr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cxdakcei.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fzfkklqz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2nfahgelu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eptymjcu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2aqiasyed.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cayiococ.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hynljfms.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dwodvens.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkbosdw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vbytvovg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lchlusha.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bjxxodir.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2liydbfvd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ofqeqesy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gvcmckjy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dbfgwtua.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pqlxbvuy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tmavjjig.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tcwdxiig.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gjoibcht.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wsofjmpu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gixztyrt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tlgktxok.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vijzstgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kraadpoc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2znynkmjt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gtcluhav.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2phlchrmx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2sjskptrj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2txavwafa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2obmavvlb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rwuskion.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gokjzpoo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gcuvwkzp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rixbvpgw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nzpthses.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2finhsecb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2attznorj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wgtkmylb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2phbsbfxy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mkziokwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2orggjnba.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2msyuqimi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2imcarkod.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uqoyddlx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ocixjveo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buvetjdf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2cwernuqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdrclstd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vnzlqffa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivlkqnxc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvifnjec.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttlnjwqo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hczulbmn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vcklpfqk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szmkpdhd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xlgzezov.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qizsbsbk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kczhbvbb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsdzdjt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2dymmtxko.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2htknfcbh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dbhhdqqs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfyavaon.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2joqyvbje.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wsmevrqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ermjnggr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfzjqe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2tthxbcei.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rkycnjvw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2eeqdaazb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mkbprqbh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2awzeqpmv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jfoqyohy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wrwnujkj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wbvxhrxj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ykbmnqqp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkybqhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fksuikce.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vuigtmod.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cbmjzmsr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2arpigcks.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rjdinyfc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzdljokf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wzhuzjwo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cggzpszg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2okfrkiqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2knrhbybm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hkbbrbtd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxscbhqz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2anwnwywv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2aqbmozxq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvthtwyw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jckkdsqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wvpfvvry.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fhgoozpd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wxcxzzoe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ltwbzqze.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lweeprof.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2najlszbv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2djttsilp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2saezotfl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2shmjxurs.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xpeqylkg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2epcbjqom.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qzairbvo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ilqrqnyx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ynuhzykw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2dddceqbq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2nxdjcizs.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2bckyxfcg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrviphw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zoromjic.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yxuiwdgq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wcrkilrv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2uakmbhha.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2febjcnbb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dclnyuct.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2yutoweol.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tgeomwmg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2avrcwmog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzfzuptd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2xljhwasb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmosjozl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ovzkkxum.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2idaltwjk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ebhsmwad.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2imqlcxrd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gqiptrkd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2qqwcdksr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hvijrucy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xppfsypy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zoozehbm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2arjyznei.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrrakid.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kzoxftqe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qnrgzybf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2kortbwzo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xbaxlgxw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2oyymykyf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wealfnpi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2yebnqjge.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2oiemlpqz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2frcuujyr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2crezdmsc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2viynbtnc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fziffyuh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2izptrhyu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pzobdxxf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2klgeahkt.html


<!-- 参考信息 -->