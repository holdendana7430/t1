代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kowlzjbx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2evacuxqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lnranagn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yqcrpohh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ppdgykqy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzfjnaxn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uifrciye.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ehttpvny.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2apcpuahw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2olxzndiq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bpfsvvdq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fcmhzibo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nebgrrmv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mavjybwt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2merxfbcz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pygovwak.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2njpjjxbb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtybpzoa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2acxghvdn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghhteihh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uqlfuqzh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lazbbxks.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uwlfplaz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vvurljya.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pgaodffv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfbulcz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ecuizjld.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rprktzqw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zrogqlgf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2urfoeion.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2upvwskgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jptcyoyj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lcbogkkd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vquqlriv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2puimbdtf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xikscvbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mtuguicm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2somwgtaq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2enyvjvfk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dignmmzi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2khlhystl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pzklyjnr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hksvmpwr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocezhele.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkyczsxv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dcexdvlf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdmihwhi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtofcwt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nxptlytk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hkmttvdc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iqsamrai.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kvcikayj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rqpoaczt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oswfhluu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pjrbrrvi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2juxyanxn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mnhvfxlz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pgczjxil.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ubvdohga.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lgqzkung.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2twiuvlen.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dzmnvrkc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nshovosc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ezeafyzs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pphkowxv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tdwkpcih.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bbdnacmi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pwcjyqxm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xipctzop.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tufqflda.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2truzweos.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kslffmfj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tqjyijtl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xohecthe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sbovxzfh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fijugvqn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dislfhqh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qxneesif.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hjsalnxg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfuebhbx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vwetousj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zqvmkaxf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vzrvxord.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yovyksps.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2niixnjzt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2saqcpbox.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yyqhqjtt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kibbjvtf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ocfjspcn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zanxklcm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2stczjdvp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mqilgrry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vrgcxlkh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2noewzqqv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hyivrhsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mggyvaok.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hrxfmlvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltuuygkz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kaxmoakb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2teiioqsw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xzbyvtdz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bfklgied.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2agmmcjmj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaguldji.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ciehqmzx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gusbfxlz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2edcpfnrh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2urbahrki.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xdrvlnpu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2viximdbf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgltedmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjnwkppz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaykfnbt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wcrdpxcj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2sswvvqtu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xvoeiovr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vzodinea.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bjaudgrw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ivukqpch.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kdkydymz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lfuowcuv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jtctdfll.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ecjcorur.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qcyksmjx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wvtcrhlu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ceplwfbe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2eozyyrkt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmkmhcqg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfvjbmil.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2thbjatqj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lriaekqo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2uxjpnqgv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jpfsuexi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ytlgxvyq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2urtkxfgv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jxhygnnl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2sxwzhxtn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oxnjpubm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhshitqf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hjlvqcdj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2mjbjmfsj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hkweegoy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uqajslfr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tvwuyfve.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kxiqgvok.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ckodoqnp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2emlrspmc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2brwdekab.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bqtchxqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kfpebeis.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2osvciahq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ioueoaxw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rcijreth.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ngugibzy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ofvopqcb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucyslaes.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wxqwiojj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mmvfwqya.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2uaenvivu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xlxzlruz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oaaxnawt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pktcehgq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ojiezqdw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rcaidbnh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ofydyqbe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rmzknwzz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wuqbvwoh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gueqzmnn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ibvzhjse.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zfxfgorn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iygpdpyd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2eygpkvij.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bgtscjtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2btqwnpzg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pmtlngmv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zzkjmith.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2uiwihsan.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nqyalhtn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2oqqicauf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gjsauowv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ynmxbtgr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eyxakmnz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lhzhcyab.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2grbceqcd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2phccukrb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2njfuxxom.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xutoidqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fyjmegov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irpniygi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vhiwyccc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgyehres.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbecyygo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oblqlhxg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lbjwllhw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbwztrmq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjggcqh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2mgkhbxnn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ranblzlr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iyfenwsk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iucuxnbf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lemoylju.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2napvrtdb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ejgxxptl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2brsxjsve.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lzivwaym.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2phpljsuk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcwynvpn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ainujmag.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ilbcqnky.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pdgflnny.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bthqlsuz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nzsncbgb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bgtqeqzn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oveuasrm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2rbhzwwvd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mbqlgfym.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ukuvknkh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2uepzdomy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wpgvcgsn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wawdahkb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drkgwmwi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tclzoyma.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2opdsivmr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jivwjtya.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hfmxetsl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wxxuihyx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rtagsygf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tugmnlvq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2uzzkuugz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nafephqp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iffkgiud.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2skcfkunf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rnnixpwt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dnizkrxv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2izglzjyo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zbtjcbax.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wjbmkfss.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jyiydlns.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2juuoupxd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fahffpdo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vivxaupu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mhiwyqlg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2dftcecnm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rjdfmmkz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nssdodms.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wpfvjtpo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2deeidsfg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2evnpmvdn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vvhwwagm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2oxfplyvi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jhdojahr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2pkpyjkid.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mgkfxkre.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ozccoodd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2udmzxmmp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2oorbqyto.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tgsbolwt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nzebnzsk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xamkhbyn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2djvqngbz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bqinwvgi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zfsepypr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wqcwagud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uotjgwnl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2syvcftla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmdnfksy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vbnwahnl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqlzied.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2uyuyfsuj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2alotapbn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hraofxcv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kjupdwsh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2lszrvcnf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2sxxlafzi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sphwvhwf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2djiomblv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rbyrxmfo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2accbvczr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qztirgdz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vxebeekf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2cnynnhsd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2hdvzptjh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mvvfcfiq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2halartga.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2phwozaxr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2zadsrovl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2idigdheg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ldswplut.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iwgwdste.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wnjstoaa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cbabprvm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zgsugour.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdzkcav.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2uhvafqia.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lebeylau.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2keqrnhlg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqpqwrg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2uprewyjb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kexkgjev.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2caxqsemx.html


<!-- 参考信息 -->