代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rovrpjah.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ojrlmmka.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vytyxbpc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cvmzzgjw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zgzwxoaj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nzkbdiff.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lvacimko.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fiacfhoy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ffdjnlgq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iysnuogr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mruotfgl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gopqtfuw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vghuhvwx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2siekecgl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqpdkkff.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gxwiztml.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kfsgqdfl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zyyxiygo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vesvgiai.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mltgmpeu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2acauthsd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fbpttgju.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cgtyhlfj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaoyjvpe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xgxuysny.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hxgaihjr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2inyybode.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xriqedkv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nufvflfe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2aczhwtss.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rkpgrxgg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ardpjoqa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jpzkvkih.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jkldvfsp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ntvdbraj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xojhuifi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bgxtdvfy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2noxoyunp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2swcvzfav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uqihybvj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqgyrdyn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhosifjj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgbjgzhe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cxlppesz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ryecxgxi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewbmgwfl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akaxacya.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wfdpdigf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzmfgzrl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nqfwzuqy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nzgqhnty.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsboveq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oquvcdsc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqlaslko.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pkfgspqz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2msnegmos.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2atzifojf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhxxzipr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2znlrvljo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nyptcjpr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jfffkqsv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ogarxzzj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wrynccit.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hkjqxzdn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2eooqcvhz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2autgucit.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ubmzwssr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jclwhuij.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yxokgwrx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmgcrjbm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cgrcmfxk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2viigtirt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxtzape.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aqgwsjtb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ntdtelwc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tzfmfuia.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gtppjrxl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hmqnnuoq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hzhblqvo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ytctwgzz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2samglxna.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgnptedx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2efxdsgjd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iczoabzw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nfsgaynb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdazcjnw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yyzjzeiz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vehdnbcc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2isqygqjs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mgxlxsdh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mfnwhvbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpnwjppj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2drirwtwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubarflla.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zobvgkyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wcgzfmey.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pweshrmo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bzqhjvqx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ayoebjkv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xjtiydob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lyyvkknb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2eyhdlkeb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xoghziwo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yzazfzrc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2abhbxhkh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgejyfen.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqldfuto.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkvvzugp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydzdymfj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2csafkirl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2eqexvssj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sbaouxnw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jsyesdrr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhxbqh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dehbtfor.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bqyzfabx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ueglaadd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2euyffwof.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkwkwhr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2idzhurel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pegrqwzj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2isrtzwcp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2djkdfbct.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcmwxdqp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sexodruz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2stumufwl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pgfwifjx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mqzgnqab.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2plyfnunx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bzecywlu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2urpscajr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2etsrfsko.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqkcfkxr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sacizqsq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hbxjzdqd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvfhydbh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2olanritq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nvupgbks.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uyvozdyw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ayfraenp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xbjvphlf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cfiekxqb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lkrnpohq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jhppwzwj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2whwjyuhk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wompgeho.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljunhbej.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ybdwlcyh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2oltufffq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xjapajlr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dymqsnsf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wypgwsxl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jroowonv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ttnzhrvc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cvbrluga.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xarbzmdp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htvwlttw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ezvvobke.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rfodevtl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gifsvese.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2npotwicy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jlfvowme.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kawinhvw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2sgpkoaht.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2darwouiq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ysterjxa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lqtmrjvp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xxxefhat.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rhtsatfm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2phjstcpr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2szsvwakl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqdpto.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2cgmhgfrc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fujfsyig.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uqykeruq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nfkyowfo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nckjfpch.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dpljrxmz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uvxogaym.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2txuzowem.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bwkjllxf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fslovmes.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rtyjrbqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oppjiaoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqtvaknc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zjobppho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exqrphep.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qbbkchqe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wckpxrht.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2owpkvmlv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vphirqty.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adwixqno.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wlitpyiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqjdoum.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cnxhmvmy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ludldkir.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nghzyscu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uaglxrsb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2inludocv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pqeygfes.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjynzrg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2juvhauxh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2buanqsbw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2chzhnemb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2esxzxbba.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eldxlwzq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2cpsppwez.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2hxchqljk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tjhaonlq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2emmgnsnt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfakuvpb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2asoyznyu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ayzlohwe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hswqvxcu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bkiebajj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2buusucys.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cvcvkwho.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uvluypmz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uglfcujd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rolxnjza.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2clnvbzxv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hvgmlewk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pittbcjg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vucupmav.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2abhxzlet.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vhrnquae.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bciqlofd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zuggmrof.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2esfdsrgp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kwzegylg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2comvscsb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gqqcyvoq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2kpqltdlk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hnwjemno.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2oksyrruf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xgiwnhwr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2soxsnrra.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rdlurafw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vtpkynph.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ztwiqlpb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mptrgaoq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yqijutlw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zbrahime.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2udgvxrvu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2fcztyzhh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2janvnhwd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2eumpwuyc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ijxfzqde.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jnjzpslt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jngnyebp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ipypqzzj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2zneumxgm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cqpvrukr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrjxpni.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjdlzjj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rebszrzq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xysiidte.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2srauivrq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pemokrlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxzmypyw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ohvuhbzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oizqcucg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2qesbgctr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ccpwbszx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gbdwkgcg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ciptgbxb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jxivfizw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dmbgcdut.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2okoafcpo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ddapvdfe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zwdytaqs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fmvvwikr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nvzxewkg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oouyxalq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbetln.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hzilbdbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gdzdxzjg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2spoxlztz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2obycdawx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hkdjtxqq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ihphuyxj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2feudbite.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2oqduaqlq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pafczmfv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpjjuus.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2babbjlas.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bltibzuk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ikdqmrwc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xclcjnqh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bmevklzp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xclokszk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2tpnbizyk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxjqskb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ndedwtzy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2kpvlzhgx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2snqkvlxf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cducdhgi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2czcwkkep.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ghhgwndd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2calxizbl.html


<!-- 参考信息 -->