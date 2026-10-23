代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3odkfytuz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vsnsjnct.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwowwubr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hgnsmosm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mezspyqg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zottstbs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3scevwlsd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3levukkbd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbbbwiw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcfaciwr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hrlzhuyi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3iqiyjvbg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3edgpkopn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zlnppvre.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aldofqpw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aulbzphy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qviksvor.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pidnxfyf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wbjqimwu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ngyqlabs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yswdrjnb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3payqhtry.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wxazrgzz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kirzszvh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3arbkcrsq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3uwqetimj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hsielzjz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3texvbkun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3aibaugtj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mfzfkuqo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxxradhi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kghyuhyz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tzspuezp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nkwqzhze.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wtbijjad.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ybvuszzo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjtirfth.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qhxehcep.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ogtiasfe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3verkoeul.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lzyhcohr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tmovgdse.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qmjkevvj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqedkt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3abbkqonl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cszlyzpm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kmqsjhol.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fhadmdzb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pkarosol.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kqwublgi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lvrfvvjq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gkitwlgj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huwsqujb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfylfmub.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bsxaqkhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uyyewtlk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3aphnmzof.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwoxoxs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uvmxxgrb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jkcimssm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nrssdwta.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trofcmwe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyipnfrp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ywkafywi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3siyksctt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kemercdv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lkumontb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ajwyupel.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3famsjjhe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uryyqobe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lhphtiqn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jkyczblm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gpjvmlse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gnvzrstu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ekexwwhv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jzukypyc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fwlqinpc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zsyhcrag.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lfmunpjt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dskolxuu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3embjlwdg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxkmnff.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qcielowy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3trnecxpo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nqwkoyuz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3msffxwfo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsalfzus.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeiovssc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nyranynb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uswkxlui.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mccsfjpn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hygjgirt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hdkpvxhq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qwwhegcz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxyqexvp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ionzlejs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xaorppiu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbxpyqc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bcngnkab.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tsepzifd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lnwmuzkk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mhdwbjxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vlqxntec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwjfdncf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3shqplsdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okdivhtl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3iixgblye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdncbrv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3focupbxz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3izbkdmoy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdonafeo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xszmctrr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3apqdpreo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gycpaiwk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bvgvicfl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tlivnrjo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3lczwopec.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwcqtnkx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpphfab.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynlaepyn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fblpypqs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3winvbuiz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jtaeaipf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmqawx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3suynnafa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fehgxpgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hamgvbmh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pxyqwobh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mnvjovzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wavrvggc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pwkgsekx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xodnrfci.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3endklrjt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jpulegju.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ltrruqgw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uiskgjwu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bilzzzic.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtcgnk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tgewqwuq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hdfatrew.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3szfkbzdm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3yklpanhu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ohblvyib.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wrqzrreh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cxsugjop.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtqnmjsp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sylljjhg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdpayqys.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3mzutmttj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vgzcwdui.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ifldcnks.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zquymjlg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rejgnkha.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sjtouhaq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fpuslnhz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3unbvzqfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lpxbotag.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3eddhozhw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkpysry.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zuzdixae.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3upboxody.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hcrsqton.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zaiysdcz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dyihxssa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bmxpgofp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3znedxfih.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3kyfmqyfj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ujosftoa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bnopjdsq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3rqzegueu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rdubvjjg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jricoubj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hifecgaa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sbuexdcg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vfcyxebp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fgaswwtu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cecytvru.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3yhffzjix.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3yhxswtbf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lsxwjkur.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wdlryxbc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tartvtkn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wgammfsl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmseyapl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yqkifvvk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lvtbkgoi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3znylyxjg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3gghfxszd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ltitotfj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3uplgvocv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zybivonu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gbfqtvhr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3glmrlmxo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uuoghwrp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qekbbtno.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gnxkwqrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odsepgur.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rtyiucjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwxkmchd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wxytzeor.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hlsftxmf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wookewjb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wsdqgdyc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zulmjbma.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3yohenrbl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wkzjpfbu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3optguweu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ejjvglmb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wsauayac.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvabeojy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rtiqnsff.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3eizbayvi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pvrkutfk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3uvxhldwm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxbnhnf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3olgbvpfq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kxvelnub.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3eyylrwni.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctnfmfqp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3owyhizli.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xzjwfwmc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oktyilny.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tviisaaf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yppzwwwm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qgqbdawm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3pgjfncgt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3uqmtvjzy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ntwqfwky.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbddwpmj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xgsmkmxp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3osgmdxru.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3avlwodps.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3phowduwr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3nqfghcqa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tabjlqif.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fbatswpp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3djzvzijx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rdzjbbaf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tlberspk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3peoujlys.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3yybeemog.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3raphfjcg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3acbabieo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gxagyprf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3dsfmnlzc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tdsabenx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zqiuyzij.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gchcgcwd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ysohbizu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tskzqbdp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hddhparf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3vjxfzrac.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3icyrpnlj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ecgntmgw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3kjidpzej.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mmnoxirw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jxslucmr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yxrzxkif.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3eaympacp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yvyejqeq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3swlpanry.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cuuuokfh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kntzbirk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wfrgkyiu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3swodpxsd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rtzgvhmb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zuzlegjh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3krldyijl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ufbdjqhh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3cdyvrkcf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zukehgqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxaybmpd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3nrdssojk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okqfykfn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3byckmneb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtutcp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gqjjafhh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pwkolbpl.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wzewbjjz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wrdkjmtj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3iovnzpgk.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bhajikgd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fdapyqui.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vkbbnmhd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jklwegdv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mmmorlcu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fumxazxi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3chxzrsud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zdlmvric.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ktftgkvv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3omxenkvr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvzgjeg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxudvq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zmfzdsmp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3fenbutfj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ftrhgvul.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3plehtcaj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vivbayza.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lguigvmp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zaxekvjv.html


<!-- 参考信息 -->