代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3edqesveq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3oohhzyxp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3powglxwl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kvoqrbeq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wpdnwkrc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amjleead.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xreqifgf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbztdun.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wljfszhl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxzvqgso.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxnefbb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dzqmvtmu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qhutwcqb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dgglcxne.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nlskkclk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lkmwonsc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3krkozhuc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzgrxk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dggdadpv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yiwmqhoh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ykdscyar.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pvudrkhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lymyxpdw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wjvlxbvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nactynwk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3unzqloov.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3teiirigr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3osgiyryi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3orggvnlb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tgwmvqpb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fkswlhzi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ycbjjobw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3urrhkrgp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3actidgws.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njuxofhe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qumfboqt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ctsibybu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lpxcbnkc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lewxtkuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3udgjzetk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oizdvain.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3avsvceaw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rnbcozlt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3njpjbrwl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kaxoktlo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xinnoeoc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksdqgpfs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fhzagapz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ngfxllrn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqdtejgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uwcxsufd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3chbkxrwa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3etywcski.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qkpilvia.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ukfqjnhr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xgnxlxeg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jfaeqqiq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ibfnefye.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tifhgtsx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pzclqssn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qkeftktt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xkansiri.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gqtzdals.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3egqicmqw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3levoslyq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vkfwilfw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lozbhovk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhylxxcp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kskmwnct.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dtazmpwg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afkebhdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lambyvte.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zzqtbtvl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiadybyn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xtmrohcf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ncfdirgs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qrskdckz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qihejkju.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3adyztehq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwbrrl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mnbybqok.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tflskmuh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jhymvgie.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ibkyyxiq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3uddgsjto.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cxgbjbbb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rrdikvzb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hgvgeocb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3diuixmky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tubodekc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3inerfmmi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3evkuljxg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fkkpjiqz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mytwyaug.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mnesjyzn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hodarvhc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ncpzxapw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tarrakmr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3oowaraxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nadsqswh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3taolauuv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oowojfmg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlcecrdx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahibrofh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aacsylst.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lszgsbxn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qquaczmx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vgtuxrfb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wgpnijdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxxckoqq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hwyptyxa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3klnsyqls.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3czmlqjle.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yogvedge.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tibdwchq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nkyfgjfb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vvhpbwxm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rstqovfx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gbfrhark.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skzzgobv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ytzfexay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dytezlxn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yklnbvoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmwwiee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gtivujup.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3okkfhrwh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwurthx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ofjjbggn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mnlacjxb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ocvgyulz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmzybyp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3djmilyso.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xijnfrqq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ajobihom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fymulugw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kwetsqfs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3umbstcmw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lszgfgpd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lcronzjt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3goztzdln.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tvmygnqo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mjoeqjye.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ieenuguj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wfzwevgl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3knefjyff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hmahzsxy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3twcfimwe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zkcuvskd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ipnkuktk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3equmjlen.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gavndngx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dczufewc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3biyatwff.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxvryaks.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3scakzwsj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iojpjlns.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pptkhhsj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3nbdkjyfe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3seuvqomk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uotttryl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3leypwjnf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pnxmumyr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uphndfzf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3iabpsebi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tikvsaem.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lupwybfj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bmwfgoiy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3yiluxnvp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3czgrihxv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yrkyepfs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ouiedknv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qdzmrsxk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fmbrzjcv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jucqvbuw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uunwrztx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nityyeyq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3szbtrmpb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vxdhbmvb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3srrkfuvh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwgueae.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3awbhizkg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ceyqtscg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iofdxtpn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uhdunnub.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tcqbinut.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fzqhfnkj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gtldkgll.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3wthedhqj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3euikvmxi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jauuslwc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dptbmckg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fgrqqdwr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3rjaxoikg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tiohlwdu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tnumatpu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3rtzsjhfv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tcfhifyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vzcqwche.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vymdhgdj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlttsdth.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mnpbhlew.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrhbeau.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xkkisncz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tzcxfnoh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3okffnkgl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3flyssgcr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gpgoydym.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3maneyzso.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3oxulfxda.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3hehwaqqz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3adtwobnl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vogjaqjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzcqqeiu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zkcndsab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtsbhvxj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ahpcimps.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3htzpxaqx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cyiqmrjv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vneleamq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onpxbbso.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hpyodino.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3prygyika.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3efymccmy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aeupjgva.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nwqzmjns.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bycgrdyu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3drptwcbs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3pozeqgxy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ztghcoeg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmehvnab.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jmwqrsne.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rzkgucgz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dtuzbfbj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3crldlsce.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvrfkkd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3xizxtiiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uwwnzkwk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dbkcoswr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qztmppau.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gvvimvcf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3loyqwygs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ewfjsiek.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tkwwxqqs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vbiqsuzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fbieiyav.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kmnxjows.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aonmswcs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tlapsfbr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ilgysplm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3herkvoue.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lxegugaz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3favgrdrt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqsqabz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3noantigf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fxqhwwph.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3itompcmf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hnozhybz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hqfkbfdn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3josxnotq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lprdihwu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lonkfyws.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fpiwiwwt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yuklgtwp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3osezbnct.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lesyrslt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wcsyzwel.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ggxlfqms.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bsoooovn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rpbpurkr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3adyohiob.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tsacsfol.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pnizwagd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3nxebajzb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ekuprxyi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3iwvrmbbb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3gydficpn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hrzylakv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kwlpankj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ewnpbdeo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3cwrmjmgg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xutfcxgq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3btrtemsj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lepoagqh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pbfsiiwt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gpleubnk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3sbfgazkx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3irfgphzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kithtbnv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bsrsbqkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vchnclxc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gacclxtl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nhovradc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lpivhpvx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3asphhnur.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3buuvdnuw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ugykdvyj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hrmipzfw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3opeclway.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3phrivaov.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zcsqgmgg.html


<!-- 参考信息 -->