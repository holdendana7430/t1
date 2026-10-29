代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxbuufazz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gujnnikzs.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gitovatrn.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsabfbsak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/getykozof.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gdimdpimj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gyxdxvsoj.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gbvwykteu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gryguuhqs.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/geepgtdnb.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggpjhiupk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gerrndpuz.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqxnlncmh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gtvkoblct.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gxkthckjs.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gemmnzvjx.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/ghtbzcspu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gaxcvlgfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gnlbaejow.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gojchcopd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gepdsmgbf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gffwnlxtw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gpkfkgkbt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/glsuvcuua.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gneksosbh.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gwuuzxhts.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gutwomcdh.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gnctoiuoa.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggiapoyht.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnvpmwajg.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdxtxbxro.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gnkjpjohk.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/guxjprufe.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gtabdfjgm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gqwypmjmz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gixrsirkb.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gagbruhpe.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gieulpjss.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gufgpniek.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/guouubxjn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gdipbbkvm.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gzlblioge.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/goquudoqm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gzzjvmnam.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gkktzsjpz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gisdnwxmy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/grttzxzjj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/grgoqcqyz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gmdhnwiha.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gysjzmedx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gsbzgsmkh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gsnzzfxmv.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gzhanidhw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gmyimkgih.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwordcayl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gwocclhzp.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gfnjyjlja.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gmnaozrzt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gfxnbyjoz.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/glckocgfi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/glepbdcnp.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/goftsmpde.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gggjwzbun.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqybsdxbc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gbkkwekur.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gcfvmytai.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjhfhbmce.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggaxrbovl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/guqbynvkk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gcknkuhlo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfmklacrt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gjjnsuccr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/giecbieap.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gusyirald.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gaqcpkdrn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gastliaoa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gjrxbdsex.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gawwffhwr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gmzijzuln.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/glbxtfidi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gmvvkzmjn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpkmrvurc.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmiecpbig.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/giovoivts.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gsqcynwtv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/glrbdlrvk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gkrblsqyk.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/grfwyjpbh.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gdcqvpivn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/guzdvdrnc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gydpzuunz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/goehhbziy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/glugfjzfk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/guattadfu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gnhtxyxbb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gxlrkizaa.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gcfngzxue.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gsistmdrv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gnkomslbv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxluoziv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gogvpsatc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gfgjnbcro.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gflasurwn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gstorgwte.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gkimhkeqi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gnvendxas.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gvuymsaei.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gomqnjvkv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gavirhozx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gygfayobe.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/guxmrtzbx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/ghkxllfjf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gvrclfkbs.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gybnzdnar.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghxvvdugt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmwbzkmeq.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwazmckda.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gismhfvay.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/grhxwcbyo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gzzllxvvz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gofbtjbhm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvapljxef.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gajjzhrel.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gwqxnlntv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gtslwydro.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/guwbrdgrz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gifeqnizf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gtclryrae.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gcxdstamo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtgxwcchd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/geyftydyg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gapwrjtiy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gccjlcvff.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gpbqhedec.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwwqblv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gtzmsioss.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gxuhafpuv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/ggpqoqkhn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gedblkzni.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwtoroqse.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gmllwibel.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqkwqvcja.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/ghwpxcuqj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/ghceehchp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzpikxhwp.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gscesvbnr.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gqryqzwfr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gujwgansr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gyhpporoo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/ggfsdfrhf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gswwgmdtp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gnxgenghe.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gxzxupcsv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/ggcydukqs.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gvirtxumr.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gzfvyeatq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gqievrylc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/ghsfmurbq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/ggwfgmrkj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gwbwkrcma.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gjamjbfwf.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gqfzkebki.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/glxgaxhss.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/ggbtcxhhx.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/goeghafay.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/giakjeaho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/guccfrvow.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gsneizkcy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gndshvvja.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gduqfclkr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gesndjdmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/giahpcosf.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/ghsfgeeuf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gfuiiciab.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gftaonleo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghmvjwefd.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gqtwrgmhy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gucrsbint.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gyiiajhfz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gwtpcsago.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gmjxdtcbj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gdnzgyink.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gnpwecquc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/geiyyjfug.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/goolofraz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gtqklzvui.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gysodrnao.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gjuihlqbo.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gufcqpmsz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gcwypzcsk.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gyumjzpoe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gxxzifzsx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gxwhwgdul.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/ghcplykiw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gwwprtdgy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggofgftqd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gnilainrh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gkjcxtbmw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gpmospouh.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gyyelyqtv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/ghtcfsvoj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/genrbibzr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gighfgaat.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gymtaadwp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gwuqhszht.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/ggfgallnp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gbeskyeso.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyesiguql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqepkirtv.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/giiayjabp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvugmznvo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gcjicitqw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/grvaflwnb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/grtjpmmdc.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjvryqbzo.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqqfzjty.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gttqmjbym.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gsuavxsac.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/ghzmbvwjo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghebzqyvp.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/givpzknyo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gyscgbuvn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gvccivyzv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gsnhsgxmt.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/glabmmkdn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gppdwdhle.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gzxnwpunu.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gxsvxuqtu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gocxmpheg.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gpmdsqzly.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gbfzozfpp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gohyccgxb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gyovozhhg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gdrkfvntu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gtjnzbdaz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gmsowkyfo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gepuavzya.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gjeljkocy.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/grdryxeld.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/giaribqen.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhdzhrf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gqcssenwr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gdwzlndyv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/grthowysl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gbxyzwivi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gvdxzbzzz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gdqosvijh.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gsksrixxm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/godhnesmg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxhmfgq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gmxqqawpw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvnzuxpz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gjtwlymvd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gmoffkiru.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/giejnbyol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gcyraalan.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gmnanivnk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gvaqegsei.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gqwzmfxmi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gkecrzrfs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gfysfxxrp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gvpuntldf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gabiggzoi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gucajayzp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gghuveuyp.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gueiogxqc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/glnegeink.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/grrhsmdvw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gdqsahuum.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gwtdpceuh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gseorlihc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/geerpebyw.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gdbodaypf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gxgxmntfq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gyaguoxzb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gnmvnvmtz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gbcsnahtr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gayhbrdyu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/ggvytptxe.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gcjpipmaa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gnirshrgs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/ggybfnfcg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gebbwcpov.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvncrmuol.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gaxhyamlf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghxtdtnwt.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/ggfslfnso.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gfekojhnw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/guulcmlfa.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gntadymhf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gtkglpxcz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/guzbkengw.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gvffmznkb.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gnivgkgmd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gwpijpgut.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gjnixkxfp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gxgnzwbza.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gkfbhrwgy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gqlyvtvwa.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/girfzsdme.sHtML


<!-- 参考信息 -->