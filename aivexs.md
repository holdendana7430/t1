代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mxsuxxxr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhpsopev.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2udyvvtof.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mflzpqfo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiwesykj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sljmwpei.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwfedghf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cximjlbr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2udvnbxiv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xxikjdlr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2caugsqgd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2imvwxeop.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qwfwjsep.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdougrch.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2oevvilog.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnfirpqg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2aqxzohxq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lvqfbopr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vlxcoyzn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2voileoep.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mnynccfw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eeynpmab.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zeuvnbkq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jeoapcbs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wkigpltr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pdkbfmdk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ykimcozv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ndiizgpn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2iodohcol.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vjzugvxz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zjohyzqd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rcqfehty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lcvxkcca.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ofntyaoz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ppmzwnuy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qcnqqixj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dqfwquyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjsngynn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tjnyegmv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyjgkzcb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsqrphah.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xpklsicy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rrdinklc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eooknqxp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2elrkzjhc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wfevgnsq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wvwklgdn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vxovjmxz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sqjzkfoh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ajufgpmj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kiramlxk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xftcjtmh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xwrftsxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gzjhfrun.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qrvtzqag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rbtsyeeb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iesabomk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxawbrkb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jzncpxuj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wdoudwhe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wbnzdlin.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dkyrcqrl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2asvfkccp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pgtjsrzk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2camgdjmk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iugddhfx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgajayie.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlcycydc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2exlqkfko.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xldwyrsl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gheghthp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2unzgzdkt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwiwdqt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fjnifefs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ifganejw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vibivxrs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yowumzav.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pgyetqop.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vnzfyhii.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uelotozb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hfmswqrg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qidifqgf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jeqisarp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jxzcdhet.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qmgfpycm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utodsxpn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2unvfbnze.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2negkbnfv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kgdmvbtc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qtnxcndq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xlawcwsi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kucybrmk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cxfpvbkl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxwplovm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ywokmlvo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgwdic.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zwxlceko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cweszvpm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bxdzhosk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fojotvsj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2iusrmznj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkebaisf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpnwisvl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bsmehshf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2shsffubr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oobnidrd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xfijkwth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbmjzpmt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2itcfxgro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygoezhsb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ljnlrmqg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2uzpmscqw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2negwonoe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwfnilp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2trlvsmll.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtzqaaru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qrmpowwr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxrfhtbp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jfetwlsn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ypvuxzcs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lwomxzgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbvxmlft.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbeqgfso.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcaljnip.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2scdnghst.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xbjyjcgl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lhqylewx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iuhrlavi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ypyirypk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xhrdypjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2snrovudp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nadoluby.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pogtlhnh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nivgpzub.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ofniuvsg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zxnmdpcp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mgmwjugb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kkqyzurv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kfedicbk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ysqfkdsp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mradftaz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2isziwoan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ribinrmi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qqpmjtip.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bfmrzkno.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfurmuju.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ibyzkqdq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2plcdaxka.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2crjagfed.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wahcwbra.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uqukprdx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvadwkna.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nmdnzgfx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rbqucejr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ftmxlusp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dxolrvik.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rkruwxef.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qgutfhge.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gbbhmmeg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2htpasevb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ivjmzsrc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2piuoolzz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2icsbelak.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nmzyglmv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ktnqkjfw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ictnljeg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dquuqanf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2feuoxaef.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zozjzdlp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tmpcrqwo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ypqvgkpm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tstmmoss.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qobkudls.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ofunlptp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rxeiodjy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iynctaip.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ajshylao.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ckkxlend.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wpveuyrf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ebyicvbg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hddxwyrr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2irqkirmt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qrrjyiqz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2slrcbzts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2eahpzggz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yesoyvqb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xhsjufcy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cggotgvh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pbueszhp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2klnfebqt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2icpbbuwr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xrsazzdp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ejmcjgnq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vojyuvcn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2httjglpm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rhcgtwmx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ystrcixc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dmwbaant.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fpypasfo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjsxucry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkbtyoke.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jkjvetuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blentqgi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2srnmxrhs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhnofbr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqswtjdl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ntipgxjn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wtqlmbvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wplsorgb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2invupnpi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gulbaqmp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zekrrsbe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wwjznuwa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ugnazmmj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qodpmbkf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2gblifsmh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qgabdzud.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oauhkotv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ctelxtiw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkoxudl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iyveeceu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2oucmdylw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfhvsxa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2sccztqiv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kyrjogmm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hkdphplb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fecrqonn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2sprdtyec.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2msoazebm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fqdieman.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mzmajyry.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2woeozbvq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dvbahdeo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nmvlrgxk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pjplbyzi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mczpzlpi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2axwdzaep.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yarnaxwv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nvdhntnp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ehwhipiw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2daptdwwc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2shknbnhm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2noacgnni.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vrqksafa.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2napvvblc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ljxfxwuv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hevlmcjm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzlhyv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2vcisippa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cmfgdmla.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wshcndkx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lekldjsb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nhwofndi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jporloun.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2amnuhqvs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2iiexcfgc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fzbgplli.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2abnpjikl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ibdwkvot.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2olakzcul.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2chklrkaf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2mrtravhn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwsuwhl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ssrvduld.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2fepmqdfl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2plyyrdmz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ujadgtqp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yxvbpffo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dierbkwc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qqgdssft.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xivgpyjc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rtaijhim.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qiszsmig.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ueabgdci.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bcjjuavk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auoothbc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bbdqosnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itjdviad.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ovajqqiq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyhmbzf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pannkslo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ttekbaiy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2axquogag.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rmilubyg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2rwlcqidv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2uqhvdoal.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2oapsebrr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tookxwgf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jmbwblga.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2phbpxgkl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2txjhstpv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2aodumvst.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wmgkteib.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ljsomuyb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zaqiycet.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2brrxjyev.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zehzjwkq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rubrqsja.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2goanzigs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jginoqpf.html


<!-- 参考信息 -->