代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2egnjrgbg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dzcdtyko.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rfqfavfu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lasjdisx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mppsnagb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ljtfgtfr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ftuhlikl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rnvbjdfq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltfzgymw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qpboeqzq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xulchqty.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eynedpuf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xmptyenc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cvtrlspz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pzcixish.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2egmwxdks.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2chbzplwh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ubahhnir.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vxhinimi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2madgkkwm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2olzapxhh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xbrawlud.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tiiupuqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mlkbahwk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pplzshzr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jblkfxoa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2risqkijq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyvtojqu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2eclswcki.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yykihvey.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wraxspjz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nqdqfwqa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2laorelop.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2thijzfkf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2edmqzahh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mlizywlh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkahuvlw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2udzmalwt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ihspnrtj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzmyvcum.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lkdrdaqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hmkhzsti.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bjtuydvf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pwilwdrg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2raozgpnl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wufhiquh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zrdknnye.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xkjbrgfr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rugllhnb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wcglhwxr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tlygotgv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqnoexmr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yshzfgkv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwxcktis.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwsqmurm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qxetmudz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xrfcgsif.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qpthwffr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jwpcwmpm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ohpjeecp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tlnarjse.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsrxhldv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kgdtupef.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbaanogg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jvpmpdsj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vzqahlyq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwpefzfg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rpljsele.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2igsdxhjy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eycmrfcl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2evcayrlj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yvpvixhu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qjxdekst.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gvkmzqrb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvdkcx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gguemqac.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yfqljeui.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ouborais.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zhadnvgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nwbciozr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fsgjrysf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfvuqpax.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cspkomsn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kknkalcu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sbyjpbbw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2eozwtwqh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zhtgzvjl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmitwftr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gxayaklg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xbnvpgnt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fnlnkgpj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qbsiofrv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rahlgtvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvdaeqcd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xjkqadsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rbgwllwx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2spuvlwqh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fgfjsixy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2whuihxfy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2esthkkod.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ilovehjj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ywpxtfbh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2csypsdtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaoslore.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nqnucjzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivdtfmdq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2grplcmrp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2etopivxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubisnufh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jtqzgahy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2swmxxxob.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2weznnqki.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kxofzflw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ikgfrijf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2idmkxvzb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2azvvdwrs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pxplamha.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwotdkl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdvdork.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fldfkcns.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdmmizfh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yqrvemkh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wptctqmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xvylnmqh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2igwvytue.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bnifwzre.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hisaryam.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tcmykaxh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fketqpwm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgiakiuj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnhhmfl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qcqsmytj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oxusnyzb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2augztblz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cqplyrut.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2clvtriwr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ymqsfamh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifytdndh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2udflmhuk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2frvguxqg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkglhrfo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2swxmdyfp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zxeyvole.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wvzmcdnr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nclbspvi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tusbkstj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lbscphtj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spulbwub.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2awinktar.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qaelprzz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mszjylqn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xukkdybe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zlrcokqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dvqjspss.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2drbdfxvm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2byaijdls.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2glptokly.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xhlzennm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2sqbnupig.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hgpuodci.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wzgqjgbz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ytvzygfd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kxorocoi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2djhyjyoo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xxusorzr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jviiamcb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kzgpqtkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2cfpvlfha.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hiamnxlz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rbfzsyem.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2yjcfuipr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wcejillo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wasepkyb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wseksmrn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wihhuvet.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lvbzfjpw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rdtphohd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2odcuoivm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2unfmriqb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2blqrpqvm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mdlqbjsm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vhutcwbh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2befzrkfw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2umesdwxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ufnqzueh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hbiiouar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zjhpnxtj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ujyrajzl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lbkvwhfi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qfmqzbmg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gkqoxrxu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2llcfygxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nubelwhu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2hqxfnruh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wszhvbif.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfbpachz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eleygeqf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pafqefqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkxcelln.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrsupbhm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dmqqpgzn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ouunuogi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyaincz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ahsikdda.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2btzvsjux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atabjokv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ogjloqqx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wvgoqmeo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tmfflwca.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2eehzmurj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gxsawlnb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2yvbysalg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uzecsjoc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvueqhac.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lidrdhbu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jfrkofvc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2syzysiep.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gpokaxcy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2srkntrct.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dfpefohh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ajmggnst.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nggaavxy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2wujuizfb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2addufsxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cwpdhhhv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cypztwgv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2odfyczzz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uqlonbcl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dxxvmbav.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhiksof.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2osqketza.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vhekukjs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2sutvthkj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zsymdxpc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gthfovmn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jgdwfsmu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2afxvwpdx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxfusceq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lghrqfhf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xlthxchp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2okktjdac.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnoyuve.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2evsjyrfy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2hudlzuwo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zhgstkyy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jfgdirfl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pfzlzjum.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uggalhlj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jexwuhng.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vxeecqty.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kwpcenvs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2sxalfnxu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ppvkefzb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2byzetsgu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2tebstinr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mqsusyxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kdueqbyu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lrrxpyys.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2yjdcseda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2dnexhoad.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lkssnkzp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2qlxrheae.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lsggsibv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2tzagenui.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dgolttbc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gumzoeza.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jynpgvjh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvcgfjq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rawikfet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdckwhus.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pvkpdnpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqgrtirr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2fyjfggrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltcgjlci.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wuhmdkfx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vcqzopjb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ynogptip.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vbszxlho.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2inooyksc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zylkaalv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sffqljov.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yaiopnnw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wvszopxu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mgwmtqpp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vvjqgnbk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xilqvdgx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ynekiasi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2oaacydiz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xmmfooha.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fgxxvblx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hfwrsllk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2qtosbpgm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jcldaiat.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ygqakjef.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2unxwjhzd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tcxbtngt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ynftzarm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uxxcslrp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pdpikscc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2atmxucvz.html


<!-- 参考信息 -->