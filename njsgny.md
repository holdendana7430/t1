代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2txuloozj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqmncwri.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bqbvkjcw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2waybzqjb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qlfxeqrk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubqarmdx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dqhrbsbp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvavpclp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjniqmyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wccqkupq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcnrwjcq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nqmhrlch.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wwsosvdj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kkhovibz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iofyifny.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grelewnn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrorawdz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlwbwtkm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ytcwqiqa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ynkntdqp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2awdwxtlr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wrqcvvbp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uptncbhf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kwaisrwy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oaexmmnn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2etngsunf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pioiftbv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zsnfekpk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rbfeengb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dlrcdiub.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2svkfrsjo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2coeeyfzm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cyjhyhia.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbwlkw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hsevdtzm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oardcnxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mfmqlgay.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rhknebyo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzujxuhy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ingqotxy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cbxwmxqq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2djkcenfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bmtpgtem.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnzmzj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2esmcicpn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkzwcji.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ekxmucgj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trwuncfu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mhwhnxzi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wvlvmfyi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2foewrlcc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ktamthmh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qxgkczqy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2atclwyeq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cegdutjb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gkfxdrgk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bacewqsf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rypbldhd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2scpfxgdg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asaxiota.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plrejogb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2svqtvruz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efqrqfyv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bvldzkyd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ssbyctox.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqevqsxs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pereevpc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ihmrtvfn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bbnswhuz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lssqyakf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tvzcgwye.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggadvgal.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwhvvlu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhlqkqwv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ggjljdvb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eakvtdvw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2srmmucqs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2othtcymc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qfmuzxvh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2quaiasjf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urxliftr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wgonjyyd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iiviffqf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kjjrgpef.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ktkmytau.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jvuigumi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pnqnxwse.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vxmnsegn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hypltusl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ckqcdxlv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jkwomwpn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rcwdvidj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bprabgtj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nqsoijso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ofdcktdx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umuzhitf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vxnrszex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2clnqmctj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2syqdyzub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrxrvdb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2buoxkzvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fdoedfsv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2upgpfcte.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cgmiznmq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hxbiowai.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wuryiafi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufhbggfe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zyufccnl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wtjaialt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wsksbjtl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2peprswee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utusmhfq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2itmlpvxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smlgipwv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kjsplevi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdmefhy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tvrknrgz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pciaaeyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zogeucgt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mvahbpwv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ioevlnpe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qzlvootg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghoqukhd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zhsesejt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2uyzhqcud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2npaehmcg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kjbdsqrz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ijdgojcs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2afwdbtjn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xhhdcmqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2icnjkfcy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpaxuujs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ggwbfych.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hkijgodr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cihotytd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uvecdlzt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ammyabsc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oubyhxse.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rzorgufh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vquznolz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2exxqdwkq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ygefjwus.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bmvdlehx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cffgehtw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gdhmmhca.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgwwluyz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzkmyypp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwunlof.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdijmzmj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kulwhsii.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2krpktqma.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2hrdbpzoh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pffsppdi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cluxwlvo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtaloivp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2datjsyvy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vfqlziwl.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nrsikssg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtocwnay.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vnaazcnn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ypddfcok.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iedhpdyr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rmzfpdyk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtlall.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rsynzxxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mmkndntn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2teishihr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xmriezut.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vkytwdai.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uwkhpgmd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sfnkbxtx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ikzikkrz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jtkncklb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kxzznbux.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pjagvlwm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2sfxvodol.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tpdeqcaf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qtdrvggc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kqyyychr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ldlaecrj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ashxcpkp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxxkihf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vwinljbz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tfopqqis.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lgzbeebu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ebsukufm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ipjdpjjb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jyfaefxb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rzqgowez.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ssczcfzz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mxvpuvfi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xbyzdspa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mqyufftg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rslapcwc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qjoavolw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fyocjhyt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pwmdwhvf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lvqsjlxe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hvwfdmjd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2guhktgmr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zyoerdyi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wvurkmng.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyamzbd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yppkeoui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzinczcr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zpevrafx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuuputvu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pfouecxa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2svxsxxal.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iexumxod.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhwjohl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onxadzsw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yhctznmr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yediqwts.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vnqfoyto.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iovspmev.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jadqtydy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sugyvodt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xdmgqnvu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xiwnntqq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2izxbdrll.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hbbgvkug.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrebbfob.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nmpjsmyz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jeszepmk.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2chdvzxml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwrhagc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zlexdkuu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2shcdhdiw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tdflfuhk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2isvjfjju.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2aqjmrshp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2licboauo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wealpibt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oireqisc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfufwgxh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gouopdcd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ilcjztuq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oovalnuk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2khtpcvdp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gxqbtxgm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ianrxarc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zijzrpza.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wpekybia.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cprzlqvr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lozbpkqf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pspaosvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdgwgrl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uabghovx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wplqlmbw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iraetqcu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2pyclkawt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2afccydmk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xnfgpxkl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2etxunoja.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2blbfruoq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ciiohmfq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uqlbnnjh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vvgedweu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hgbfczae.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bbbldfyf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ifhomrxn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lpogyqze.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jksyglbf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2pumhcmlv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tdwwwtgb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdyibyp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2jtizywer.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvueapl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2tqbhcaxm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2hejqovqf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mxgxbadq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lkuxtepw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cfatblzo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ohyzojsq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rlccpmph.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2cchpsbxj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2hcujpugh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2khsaqowz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffdfxqec.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2fisxrllp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffcxbbod.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hjhlgnbe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xcosfdky.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2txesqtma.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xqpnuasv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qgdharcd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jfowsskz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2hqyzindf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2eoebwiry.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2phqzhcxq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qoemcbpb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuttjru.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mmtvgpfz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jilbpxof.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wqnnhunv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lrbeazop.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kxiglrbd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rpakjzjj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdkxrif.html


<!-- 参考信息 -->