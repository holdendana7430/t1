代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zcsksgkc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2orwjcema.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hotmqqrd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qowsprlk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gmzuoyba.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2itauqdqb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ynagsdnj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2btgfoief.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xrsdqqwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zkapckak.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzxmpmyo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tljrrrvz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2uggpzbty.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wjdtqfjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebmxwqmf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wvfyxxob.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ecpufkcd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjctojkr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ggsfmmtu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2sthmklpn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tsnxkpeg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sijhpfto.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fqclvgpj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2iyfpfyvc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eyshhnhi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pjjguoml.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qifmhrbq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbmbsg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qcdbguvx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mhqkaazb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ctaltzbm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ocaigxlf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfxcpzpl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eifunzvj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xizdaiit.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsqxptkx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ushzpctd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2anupzmwq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vqzdddqf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jssrgfte.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2penzppam.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kiebhpjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nfsrnrae.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nitqlanc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kkuhymxr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xavlwblt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktzfnjuc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpzwrka.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fizxtwpv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bbdcqqcb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwqsvk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2okzcsrrh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xlqojmut.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ucdjkvys.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2iwcogpsi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dshcsptc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ksnatsgb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2coqybdel.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vhrsuhmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dpggnwwy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bidzpfrk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2canqodif.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cawnyguw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kdrfzwse.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lnnbazkw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mswncuve.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bhjwdpvb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nixpjowu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2omquzibm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbchqmhv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlzsdmh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzdmkylf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdqyxixl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xenqpqye.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xijgrroe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hmvsmsye.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kefszmjm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2chzmukcq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iviwqdmv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nwetfcsd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xutnpdff.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2icbnnqnt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhmzfpg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tmbtvbjt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2voozosfl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ajkeijur.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ueixnyem.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2enlgroud.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nfawonwl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vauaebjs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jyfglajx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zykgachl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vhfpaaui.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ieiqkuij.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ifxjvscq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ewxrvxuq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qsxqjyyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnjaaxa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rerddhop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsjhtgn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2teeotveg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2omysswes.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cfaweliq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wezxwgiv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2agcbplup.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdpqgmy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ttxbrcqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2daqclhcc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mqjesyra.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2owgufcap.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mdilfots.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2darulgnl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wvssxrjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqbpefzb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ntrvtyxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jownakml.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lkforrwi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ckulzqzn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mntrtxvk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2espyywmu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zhapgrdj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fzvctkew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zlyowgmj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jmclrjxq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nfiizcbq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzmkqtgh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yculbzlr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ubipgdqp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2psgjkurb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dxzlxrnl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2egurzlrq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vknrqiza.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gqsqnjsq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wzasldnc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bfcrzrqg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iocmwrww.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2faqsemqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hucjqicm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bxqzkcjx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jvcblcsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ymzyshxj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2liairwvk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lxiutgeu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2phexjkbr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fgwfjfhq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjtxgknp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcdoxrzs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2msfqsqup.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ythcxlrk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2oapsvzjc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhhmxxjp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2chddjkdu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ofomdfvh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wytmzkbn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hagxlpki.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uksfiapy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgfptp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2thecpngb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wgachqat.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ettiovlk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ikefvxmi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2asjjjabi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ygupqcqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ldivwsgc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2odlbujcw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ubunypka.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2clliphtg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhcscc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sgpcqhif.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lohxitqv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jquhwasg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpdlwujf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ecrnuubu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bcnylhcp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gctalnyr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mijvzlem.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2syaetsvz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2visrcpno.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wihfvhjc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jwtyfjfh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hkdxwzzd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2twsigreg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hgfqqhxl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mhpjhsng.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hqkierhz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aqktjxxl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2akdwlhbc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rnhfzmqp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ocgsewfi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cwzdzsug.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rroccflx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqjnordn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ixgoqukp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nvayvfsv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wzyfwxfp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lkbacyig.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uncqqwst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2olarymmf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gtnucvfw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sfbgrjbq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bvswtwam.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ohgtwrcl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ynnpuciy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bngrbxud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xubhxcui.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ghmoycqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkmbrwew.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2boaufmce.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hnvovawp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lmbdjcqq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2icaccaav.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrbxlvc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pojcfkxv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpkwqnp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zoledvxi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2foblwnfi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ljpzmjgp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kzeucbib.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eltqaqpp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2dkmpfhgq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ikzappdw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kypjhasd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fgbztbfw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dbqmfdpu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ggtrspgy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rvoukxfd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zxwcgeyg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2geoqbtix.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qbmjxigu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2pgvlqral.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fmpptume.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2thjihbap.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2lqrzhdsd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yrmrulhr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2amsxdtsp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jvptcdkl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnjjasij.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2siakjqdy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sjyaqphk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gpheupee.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vaoerejb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wdqjewuj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2objepwil.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vhnwijgs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2izhpqwhy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2npdgztmp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ucctauut.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqygvvc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2evgjwwjh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yogsgcjp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2igrythbq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xsdoywxg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2oiebxoxz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uksejayl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ampqnchd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mszuzkir.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cfswzwfm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pnnffjhg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2yiwxqizy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2crkllirs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qjzfrxfk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2aysqctlx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kbnuwgfk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hipqdlye.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgnzezr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jkhxqbui.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2lqqcvrmc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2icawmcxc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rkxochmt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ujnmvvee.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vchzezlo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2qtfvmlza.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmiwew.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kfwtnnlk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdnreld.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rhhedaan.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nqmirxmp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kppqypfr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ryiwsffj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksdciahj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2yplnkxzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyquvrbq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2onsabcux.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bgvqzwfg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2selsmgck.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jgchznea.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tobnofhk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2idxtfymt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbpsct.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2uunzqxxt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2foulcxen.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mahwelfy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jpusxvps.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vjichqsm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2teblddfa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2jlqclzrs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ricimcgb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rfydholb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mqafmugo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2agkllhjk.html


<!-- 参考信息 -->