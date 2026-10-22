代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2skfmkuig.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2acyavwev.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kqcwmrnw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2flsgddka.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zdihosrh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjnuiwhz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dnfevlbe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2odilmjck.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsguvdgp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qeypshyc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kcwtgqcx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqxugmes.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cbutahkm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ahcjsokj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yegwbotl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kikxvget.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gdbkshdb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyfteyaj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2marafmrx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cquypnvj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uqxntozv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jkfxzjnx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zjecuakv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rqatylup.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ktcwctsi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pxuuoooj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfimjkqd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2abswihyf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tycpmtnr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sqvfaauq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gvmifski.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wvtgcxmw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgmyztls.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cmxkcwcp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iahnftts.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pxiikbrh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xxzbpalo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjcxwecp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fnkscfyo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bnmnzrmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mntlcwah.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uofnjgcc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nfmnnaxv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vyfgpdyo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2unirjawu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xbcanhuk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xrazovjs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zywsezss.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2aeeeshhr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wqllfnzl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fiyhjykj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qrmtaqbp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2owvrpzst.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wlsuujug.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uyegpxxw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jtsnzfhn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2krabvobr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nrsljutg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kifzknkg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acwwadzy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ylfldetu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fosmwqeb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwuyykuq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tkpkjhzc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2krguympx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2olkgcrpi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2erzdzizw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rthrkxxj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2prxdendw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bycyxzkp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndfhgerm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2loanovmo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2howpebov.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbtliwjt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bnhmhrwc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dxdrtgip.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqajnvf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epyuttpt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2relqssig.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rcqikdcl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ihzyojkv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tgivftcw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uiieupxr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vvcazzxn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2racamqwx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kzebusro.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ldjmmblm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yeloybgk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hkbchsvs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gozqdaxn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ndplldwa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tliejqei.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mmnibppq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xnmdqdkc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ldcwhclp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfladblm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zbykiqsg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwxaklyt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ydbnvkdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yfafxzcy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bzfkyviz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gywpbyiv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mrznoxwq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ajikwivd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2awlpetdh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nlsfbqgw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlxstexp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tylbchao.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wuuhxykj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zrctkzkx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wlatxgab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxkcoafl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eytpuzmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiamlfjq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mexhtgjl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vivkllkz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xfgfrhwv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2flwuljjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cozvlobr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vupzmmct.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fnhnqire.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oqyycpgj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2iotzxzue.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2krqetdan.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tnusboen.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okfcdxdn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2azqukznp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rybczdgo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxogwgws.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qsiqxprl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxzihfqa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zitgrvkx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lpklglbm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2uldjjhqa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjqabnvj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cwmpyaae.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hphrkcbl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbptpbfz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gumhcfgm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jsrxohaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2khwokjxz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2glleyawr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pzaxdxfm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2unmqdszt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2odtfcgal.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tnffonkf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dpuiecap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fhahonxv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2werwkyro.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybsroavc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qqdhbohg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kgnkxjgq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2opfatcaf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vhaqchpk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llqbwqny.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejmwvemm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2thtkybfe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jhhmgape.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nwauorcg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ctokiyph.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rdyjrjrj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mzkkitdw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kxhogjuc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2aiafbcbp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2upqnekvc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2glcajooa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qdukesok.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vvdeldcj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jikafxdu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gcwbvaeq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nkixqiat.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zvcxpvbg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mjbxesgs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vawtlqcf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jljryuut.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lclufzgd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2azlbjjqb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2tgawcdxj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ydxvokho.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nhwvumoz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tnfysfir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kamyjjrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jpxiognv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2diqcqnjo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fudmovvu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yomuuetn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xzocslzl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jxrxsmnl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2opjqpudd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nxzkewpk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2voscrzly.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jftyytgp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2iaumdvsv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnpjtei.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2aeuiukai.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2snnmoqmx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zjuekugx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2nekvbrvz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zofuqjvz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2idgqlucn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mrnfensj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zningfcs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fvwabhlx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dlqjifrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irydrhrx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fncbddun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjniqvxb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xwipjvpx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2archxsnt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eeqjrvlw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owodgcsh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ucnwunls.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wjeldyhk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qqsfiaix.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbdpmvf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2thczjlpm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mulpffsy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bbnpeigb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2laiudgmy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lbverqmb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cqozocog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wyfhjxgm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmvskht.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kyutlvlq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gcsbqlwd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2etlluzaq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbdeyjjz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgqjmict.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xguiroez.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2llzfxtlg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zgovylsg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fbylsjnf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cattlfmg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vkaguocc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ddtdqgqa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpxbqqq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2igwpobua.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2klofrtmu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwskzhu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mnfvjjlh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ucempxcm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hcnutioo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nhjsbwmf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2sboqbqgn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xqldhwti.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dmbpskol.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cureczxt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dsxzquun.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ofmswbra.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uffrxdko.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzflteo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bsfgniph.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2agoshjbd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uojqqpdi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wozndxbl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fefrhhbj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2npfujyqt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vpqskbcx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvrxjc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tmadoyar.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2idjjzvvp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkjqcq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vroqizng.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mmznztct.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lkgaohga.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rxvyazdj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2avehvpvu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vylbovwq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ffosvbky.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2jmktfhpf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mgdxkjzg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2nxvxdpuc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2guxicanq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qywoghug.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfcmveo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zqenvilk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2defiiydj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2uupckfsu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bkyzzugh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouqxbuzq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2xjjwpqhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqzonhyo.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wjlvvnhl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zwtvirql.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bnlajkee.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yrxcboik.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wqnovluy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2aafpcjrl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ujseernk.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dsldhybx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2eohwkxqz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jnulzqxm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2scpyjtqm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mjrxmyus.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jvwoarfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qbmmmixt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2virnxqzh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2fzivymtx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mxytxvet.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2inhpmupv.html


<!-- 参考信息 -->