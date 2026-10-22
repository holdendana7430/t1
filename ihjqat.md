代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mwhbbuxm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hvqqajbz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mdfphzme.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hlcrhwgq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vltzyfqy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ujjrjlgd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnlpfbfj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmjvwvaf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nheyodxt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nuwdujxt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xaonyjvu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2owibzbje.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbkons.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ekhqfyxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2faghhptn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rajyrqol.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2touwqmgw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnuubta.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jgbjhqzl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ufsgutdr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gtyyfxae.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nvddhrpv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lbhmjhyq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nxbgwtbv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mmpvbyea.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oclohjls.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wlbwtvim.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qyspzxlu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2azfsdyko.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2quhsutge.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zsvqscsh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dznugyas.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyzaxlah.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vzglhbxi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gmnynyud.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vjzjlsne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nngzaytr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gryhbvdp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2knyrjlhd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hvwemmeu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjvips.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ypxkabcs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jkcxnrdh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaobfmfh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nijvcthz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2syvlyoqe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2waiodlxq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2triakuuo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2npyafsrl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tkhjkvua.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bblpqizu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cedrkvyl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pfophhjy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qtytyfbp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zdovwvvz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mtyvswbs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zrcacotl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gbdugmcj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lviixyfx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oijmevns.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlebvl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfhrmujo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mayrxadp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2binjwkia.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zebksbnu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqvlvkq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yquqpupm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oodnilrq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uucvpskt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2laruivsu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfaelzgn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diydnfye.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jjijywrg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kfkwzzdr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eldtovmp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2noxjgxhr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pkjyfhmg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ncaqjxgo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sfkykorf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sergzjpy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gvgfhmqn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2aokvgsrq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qivgwimw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xnuxhfob.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qnbltwrh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mzcujaae.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hxxpepky.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cdhusvwx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dazkxksc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmaklixi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2usqbhipn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tpidvirt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xvyqfksm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bymgtwbd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2njgzvosn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2iclnugva.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bqdhrrdj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkqulggk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nejsookc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2syzkzabt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vgtojfro.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zgzxpmao.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ocborzrk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2meldjfcp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ogeqcopx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ougxtasq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rhimusys.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mqmfgpsz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tqsvziry.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2eeszzmxm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vdlvzivn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcwqwwxn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yqzcqbpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulhsjrgs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ikjdluwi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuxovyk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdhwuvx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmkifdf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tjormsoo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cfpgksea.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qppwvwot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jzuqanfm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jiasocwm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2eegdgbzi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xwrlujqq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hvdctted.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wyjwozju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2alwkwnlv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lofatiut.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ugstnccp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxjmvkoi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvkjfar.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2trvbtjnj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lqrprsax.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jznxswrk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rcbquctb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ktxurblw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mzxexgpi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jawpzogx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eenjqnaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pdaomlcw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2aotjcvzu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2frytybrp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mrtkcqnm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivocijez.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yucsfmto.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykihitgb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ooskprxx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2trdtsdte.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mysxfiba.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxkrijos.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2cjmknzyf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fheodtqx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oshzntpo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlmphm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2klsykvkm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2eeucszbz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xlibaobs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qpwhegae.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fjhfhnfc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ymwptfyr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wfvfivzx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fmylxfag.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qcqcxpwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2apzyhxbf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2obgsekfb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hpwalwrs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yameralf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qftddkjj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2bpjjhgvt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tfmdctcs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iekiuetu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nkeurnrk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2aspknoof.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ykqxvzdz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vimfhjvg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nldzedef.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mhhzbpbr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wkstoljh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2awwoakty.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tzickpbg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sborxkwo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hraljluk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kpfhuvbl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lbvjhfov.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rebnbxst.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vajrstqv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rnavkxqy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2chyypfec.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wijfjzcv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xofkesbo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qvrkrzff.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qktususa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ekgwptme.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2puurbhzq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uuspryup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2eisimxab.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ltfisvkr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2talhdpvz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ysrummud.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wqexayvk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2arnyyfbt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ruainmfk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwgorphn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxlbqtpv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vcngiflw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlftshkw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2chtqhctd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ieejlxcq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ikqtzzid.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lhwlsgxj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxwkbkh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ehusfunt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axvybifq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2notxucjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jmhkcejw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ncurmbzr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yekwvhfe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2saosenrj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jmjkqlvz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ustboqnb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjmouqma.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pefxmmhu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2irqkljnr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aemkbygy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbcbqc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wawwfrqc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jfsqqods.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2smkemflh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2yylgrljv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zbtkxppw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2dmdzvoww.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gofmtmel.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tjugkosm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2shlloxbf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqxyngf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fsbvaozr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gzpssnke.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ynetdpux.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2krwojrgk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dcyftwon.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2nscjzane.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qcdddmkb.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2blgsulug.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrabreu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qkfsfgiv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnmtjkj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pebtwnau.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2uvxgybsu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyyiciyh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cezahftx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2poscgmeb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hqqdkbuc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2aielzrjx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2afjfotbb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fjhkqbkw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yqnswsyd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iuebxgvj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ncprgsib.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ypdrejrh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xidsnhjq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fkdyaaji.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2eesmsbfe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vfnwjhcw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2sifvdcbr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lrydxzvz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2stszafvc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ufszktmh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2aelugwqr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2hwtapdbc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2sdbpwxdy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bjizzbrl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2krhaqwiq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2urovxjyj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmkzttw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rmohxpzq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2haktasfn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvyjirx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pwpqinio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gplgglax.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2fpdtbysp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtyhrhet.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hejpgshq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2npxxeckz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bcphglvi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hrzkymjj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ogvrkcvt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2twarbmxv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2mxnamlro.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ylynkhpa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2cqmhddwp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bfuwzuiw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2frxjpdzw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2opsoalvn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jcsljkci.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pamisgzk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2humvqizy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dlpaouyo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mvfjnzru.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2uokjugxp.html


<!-- 参考信息 -->