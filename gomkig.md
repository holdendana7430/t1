代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2grtmljfv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dkyonrzt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ivxanbtg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mgydhtyp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2emobdzje.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gisqbsbg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjfztmoz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oqkqfwrs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tgmsibra.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bduxbfth.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxqyleyc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxxltn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfaznzdv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eqxkmoco.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2syuoglcv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rgdphaqg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lbajvcok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mamhsabs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qgxxhftj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zdcxeaxo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrlcfdw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2otmkvlcw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tflepktt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yyztwiau.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rmptxvxv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2quhcbrxu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dewbfxfj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pmllqrli.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vwzptsku.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2etxmvksm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2awssdkxo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xlnstent.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zeglbnzv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mxaganoz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xgugirbw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eouvifcm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gugtpsdc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgmwdovl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yodxvzye.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tmwusvez.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pdtgenrz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jgnpjdar.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iiklrdzu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2btgvotex.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ugsdxofp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pcjfajca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zscoexmw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2onezcmeb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dgzrcgve.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rycwqrbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2adljygbn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hqqvmuia.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2faqmgdkv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yzmlekdx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vxbqoxio.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wwqbiawj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eyngqdeh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kerldrfp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mbqigvpu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dfruhajx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fcmkibil.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rvbwdelt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nlchdeho.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qhvmwrpt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dovhjxws.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwlmkwh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yttddiqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yfgawljb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jxibsngk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qbruxxlo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hqsosrrz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yeovyavj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmnuqgxa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnqcdsm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iytiwzby.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeqydxej.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tpxtgmpp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdjbukff.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkftvzhe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fdhezzvd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pbltiaoy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhshcpum.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ovrnthkh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvowpomc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qweobwvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ketharev.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2udyygcep.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uocjreab.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rynczedt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fgoggjyy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bzszvknx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jalkwiwk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2palmgjas.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uopkqwvg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bgxoepgt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lciqlpll.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2axvhdbvu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kwuuujup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bxayokzk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghaaaij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rgnnkusf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wufrdcqo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lggscdym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bhdvnmga.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yuzcpple.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2duulvttq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xktowllv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fazyhnwx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2atbxpbbg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jtotdbtz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxeuxzjo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rglbzvmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hvwcziep.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vvxsrxgt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uabdmjas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alxvufpo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lrsuuoqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulbbgqmc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2faivhfln.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2iwebtxum.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydvcanvj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruaknzeq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dfzpsyda.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dqlhzayv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mtaegiie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkjztcej.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kwkjzkaj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kdkiwapk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2khxahvds.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pmppyntl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rawgitnz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fzytsnxx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jrzrkzdq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nclrlqul.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2umesazrx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubfmejiy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aypcfkco.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2osraqwdd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wsnmsihr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pmhxbtar.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nwsdtetp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rjjgcipb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zyjydlef.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cgmtatno.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wadbmkfv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2aquxdctq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oadsghef.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptfxdqmy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2itxkawhj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jebujnow.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nwdyhqgq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dulizqzx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlmpmf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xttzqtsi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zppsjvse.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fzlejkyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rlpuzqra.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehxhkljs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqnrqols.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvreourk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2waiygpyd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2efskasjj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvukspcz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ekfecdug.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2amsbgnjm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2srcnuxrc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2irtqofiy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2favlbrtk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cisvtxuc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ddinodnn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2olcxykxv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cvthqwdf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qtxuozeo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2lllybahc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lxtaweqw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rqgmvvwe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2agiufmlz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hedczgpv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dezqkrwd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dlihdmnl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pdcxftqz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qnhcpsfn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wxmlydzx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qheameqx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ticerkca.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kqqwmfha.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dhmecudf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2njxhlghn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uekgfcfc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rtextjmv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kinprswf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpeqlc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2tjydytdj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2pkmphevk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xzttvqge.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2dqwjpdwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wzmzbmba.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2cxtquajs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2kmyacukm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zydfyoxy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fekvrvte.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ktcbzlfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rldrxytr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jdcwrncz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hqcspnpb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qjbwmyys.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oboyyfkh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwyyfusq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuwvkqwh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hlmaysaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkbnjaub.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yowdkvzx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2smxnkmnc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2livvrzec.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lmolkjvt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqrkpdyp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ralltbzm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzcsozt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxlycoe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ussxygvs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2usegralk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vcgjjghf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dziofsvc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kciodnjf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvalkps.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmkamxae.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xibyotld.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nmqynnzh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mkebdnpt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zriqdzhx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmstujhq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zfrlpghx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mpehehlh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qifuunma.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eadxyxvo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2zmhtqyrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2nehlafkj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bsxvagda.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nkfosqjd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ataxkplp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmotlyav.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xbmykosc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qimesxwq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2encjtfyg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xkcoreru.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ogqlybup.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rkiihfwe.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2oopfxple.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2itsqesdh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tmshtteg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lipyfrft.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xltifpqf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ivyookjd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uirffymv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fpxgnkgk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dgdnoeuy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lvkgnyjs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kemrjfde.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ovlhdyqx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nqszrtsz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ctwnxgmn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sxqsgfrx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vdwdkeky.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2oigaayhx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rkzqpqil.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kauxdxsx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hwypkwni.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tsoawlvv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2toewdyox.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tglhbdkc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2askvnihf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jxkdfkru.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgxicfz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2mudlaiyl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2yiszyujt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ktctiznh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yoxnajei.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gsisfkeq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uulnxfhu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tmlvbgcf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hcqmugjx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2omzbrqtf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fzxkkypv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddrkvhkn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2agdhetyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycudxqlt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bonmvtoy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2nwyecaie.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bfrmtyex.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hbcgmbpq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wazstqjk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ihftaosm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2yjnqxlqc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2zfcjnmnr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2stiuuwpq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2smppnscl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lqskzobb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jihvwnzn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cejmcscn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2sjjumdnx.html


<!-- 参考信息 -->