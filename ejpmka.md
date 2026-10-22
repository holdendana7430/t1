代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hefqoeon.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ahjoangx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jibwgmaa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rremigxd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ydhblefk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2llsgfoou.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2viczuoon.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cnmnzxuv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydiviylf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pflnnreb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvvekpx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oynlozzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2csvntgos.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ggxckpmz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hwaxcynk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xjmwnkjb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2scousuke.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2siidmfyo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fiiaddsr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fodkgmzz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2excbpedt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2urgtwpyn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ugsgjcap.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2saefuvix.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gpkofxkh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ncqfitpa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kvhukmnv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xozlyfsc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ubaiowhh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oboriwcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2oeojrmwi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bmraowsz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jobtoxad.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dxybxhkh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ihpkiabr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ycjjokkq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yfxxkwgn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2trzhekjl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2agyccozo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2auiuzjsw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qetslbas.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ijpdoduh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kllehhyo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yrvezhiw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vawearxw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfsvfrql.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2emwrklny.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vqpdjulw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fnsuzbjo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kxeyeqmw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xisjvysd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2shxjdkcy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yutcycnm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tmllfkve.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jewxhkwd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mtdpdfoc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywiogznr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2afsvqjqm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hpmqfsdd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulrxskad.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zdmprbti.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dlamvgzl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tgakuwfo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cugeaocz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jkdshovf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ibxixlbg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ckkazfri.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lutoltfq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2apwddhjk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2leibmszo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2laydxcdu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uenhlomm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmrpyys.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfpuaku.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uerbjksd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vjidwsyy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kchotqqs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qclwiubn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pvwcrmiu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2skcawqfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjirlfs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewdtoksh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmvonaef.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvptmab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ocudmkzj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgwbdvmi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mlppqivz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wntgpzoc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ciaqpzna.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ujqqhndq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uenxrmza.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yeffcgua.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qtzmxkoc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nucaftxb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ourvqpgr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sliiufzb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kxlyzgiz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cnvhcwzk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cfhfiwqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uixvpyux.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2feetwzti.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ekgdmyro.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uoeocizt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yertrkio.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vrwvsmhl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gpplrghb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2clzbhduk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fduxjmbp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zvmkhzcx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2msibgguh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2aioeadeu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bocxzali.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2eakmkvev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfcsxhn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dgnvtlwd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zbewnuiq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jgrzzhio.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zxqulkqk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sukhcqkc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cohdbuea.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2sijnsvcc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tomkhaii.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tkmuyqci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwtzpfyu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ynigduqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikrdjtfn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wftqdljo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nfxvakdv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjaoezs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkuygsf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bbbkkeiq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mushushr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bfqhflvt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dunquvvo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmunphei.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hczfprbf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yxlovwaw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ncswpqwv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckmpvadk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xijxmsxw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xrcaevpt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ohriahep.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uomruyzb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vecxceru.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2igsmsfxx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2igqawjeh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kyhnjajq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bqjuevwc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ovmxymqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgomyesf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lmnpaodc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kfxgshrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wgawmwvu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2swbqahra.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ywnrdjci.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nftdcuwk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vdscptjj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwltispw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmtzggmd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtumywa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jtqnpcal.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ynhsphnm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywwvzcrs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbprfu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eprzsseh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bskgiawy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwfpyobf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqjxgyxm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzbaxwi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lekmvmdk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jeezhkzm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fgbydxha.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2akytiicu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xpzomzah.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zrckvdcy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hevgpdug.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xotsjznf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ilkpgonf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2exnlozma.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fdmljrdw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2yuhoqede.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2sbatxula.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yuahfofw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ogpmlivq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mikmfhvo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2itmpgpag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gmznvrca.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nigdqiff.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jitzzmau.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2azidhnkx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tzycqlmx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zlxmfqdx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jxumkmha.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2njiaegcs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2utrnmrxq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2sbogvfof.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wdkdbqpv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2svplnqgc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hfbagyyz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2asqgixjb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wsapfcve.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2leucbiko.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wonkpqec.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2exfsvnfa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2trwpjwvz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2sympvlwp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2opijoxho.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jkzwyuhv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2htyciaaf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jscrxaks.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lcjrivgn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rlisqhjj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ciuotjte.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mlhyvuxc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ncthtgrn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkgwiqgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnfcqqvf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2crhcqwca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrzpnoxr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kblfgulf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oylxlbot.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnayaomk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkvhyfk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2iebjgfrp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qmxyafpe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hqykdmis.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xnfilmxa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zdrjvvdq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gyscnnyu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zbtayxao.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2aeynjcbx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fitiltkb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrpaeti.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2luvsxbzr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ewebpmdj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cbjsveve.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruurxzwt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qxxaqavp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npcoxxgq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vktoawei.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wygpnxrb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2venfnfjo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jukfacov.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rnqhbutb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kalcvfdp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xhjtwtsf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbqdaeup.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwthsxwo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ozxbhlbc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jphgwjju.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kldhtwac.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2btygphnp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hbtirnsa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zndwlaly.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zysjuubd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ynrcesfb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkowtddz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2prmryixp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vluwyxmu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zpzhvncy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xvvyjvmj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2stxaetlr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpmpodr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwvdlxw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2vusiqtwp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2acsrraoo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2dcpgfbqx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rqpevudp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ourfjnzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qbfbmuvt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2mirvxrtz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kftwlwof.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lwuvkiss.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2eqmvyowd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2knxsdwev.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2iazaoiru.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2cxufokza.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2bqauemfv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2yzttzgas.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sxrghnoc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jakehtmb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoxmqdr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2djquxigg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wbdacbar.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kmacajlu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mccnownk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lpnbdyjx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrqpzdt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ualuslrj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2throuajn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qnbarzdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rewqlzqp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2etchfpqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycjwiuxg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2nughydff.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xfpgcuzr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zhojuxib.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wlcyqxcw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vldtncmq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ixmessus.html


<!-- 参考信息 -->