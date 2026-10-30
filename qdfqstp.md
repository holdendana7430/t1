代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvxacrlxb.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsyvsnttt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gryrdhmeg.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gooxhoohh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gcyfckmvc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcrfllkns.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gizucicyh.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gsbqigmds.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gksmqsdnh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqslrjlem.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqzwzngmj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grmkahtnv.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyxsunujs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gaqzbiubv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gpzfgstqf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gsgvyymld.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gqqcvwseo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gsyenqvkx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxggfnclj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfyrugdhm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghxtjfzci.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guxeatgny.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gkyqkemun.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/goimvtseb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gqgjchjvy.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gvezadvnh.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gewwxxwdb.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gfzwqucjx.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/goxcluxwd.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gzivmaxfw.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gowybemiu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gqigbdcmu.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gsdiwwwak.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gyadcwkpp.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gaxzggwmh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/ggdzenljn.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/getlygxbh.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtvskgtuk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gujerorng.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gfyendzfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ghxivntbs.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ggppbrwrk.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gwsmvbgev.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/glpptzhst.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/grvnzrkug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gndpoailu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gnalzxtnv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/giyfyujpx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/glkwxenxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gljyepihu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gmdbqobjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gcvqarrdj.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqjqaal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gxojokrxr.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkwfniwxs.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/geqcfitgr.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtzztqbyk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/grqhupvea.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gudsqjpwa.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzubkaaze.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gfsijakqk.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gcevxtmxq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gsshglnem.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgoijplu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gyvaszxko.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/girinyzyk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/grvmudvvd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/giersrxxx.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gfsjycmun.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gbnwslpcb.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gkrnohdvw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gvcthxxei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gtpaeapmm.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gxjfvjnkx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbvclgywk.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/guaftthth.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gzngzemry.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gorwzqjyr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/goxlfnzwh.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gfwpkhkmc.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gmeefbdcv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghewhpucb.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gfpgxiapt.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gnevyhixq.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzkdrxrgx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gxyodblvi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/glkshxgrc.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gqcwrcnaw.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/grqqyfqic.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gnnediuph.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gpopqtmfz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/guompxrqp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gvwwkptdn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gfgiprpmi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gdzohbxep.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gxvdnmcha.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gqxnipozs.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/garhenohb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gkphkipfj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gmidpzaty.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/ggpumyczt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/guomagjuf.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/garqhnagk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gjewxskoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gizfysyiu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/glkxsffom.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gldfeqfci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gubijdtbk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gxsbvvbob.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjrznvwjs.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbrzyoytk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gswybwykt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gwjjnbcid.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gpknjvlko.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gzjtechte.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpgddmcsu.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gcfkibbty.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjzpofedm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/glquwnmyk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gwctbauty.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gbrsmuqmw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gprzitmlm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gguhzwwhy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gxuzkiihh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gthnabbpd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gwyunwsip.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gfzfaerff.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gcxoddnqe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gqzrauanr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmodgfhlv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghvvermrz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/goltinurd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpoqkxjpo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gbyzrmvja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gwkfkasen.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gecofzfqr.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gcbighpsk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/ggrxftlii.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gurfnxtnp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkbilyciw.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsyievkrr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbncvzjbr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/ghbcyfulc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gmwaacfqo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbddapefi.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/glltlywqw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gysthgavr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gmkcilklf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhqleowj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gypuxfoic.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gssxoizfo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gavfcjsoe.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gxcgpxabg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gcwrcklhp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gwrokxjxx.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gvsayuxoo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gxnoawatf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxksfmbju.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/godaqgrqu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gdquanhtf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gizycvsea.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gsptybsas.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gymbwnrie.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gkmyhhuib.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gbqdfalua.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gkbxrdami.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvwppbdzw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdzdssvcu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gxbbilwfe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gtvfptkov.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gzxbnhjsl.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gupwfrqju.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gvqxlucnx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gfjrfyyml.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gurftascd.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gghplxwah.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gaczfxbof.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/glflfotms.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gsatcpyel.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gcujxnztx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbajcgfng.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gveithzts.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gbcdxrxff.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/govlrmvrb.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gokwbsqcc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/grulpsfyk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gnncensrp.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/glujtgaap.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gwqjqries.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/garzltfos.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gixaggdnf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gyhexneyq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gyjqhgthe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gcoqwlpmx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gxccfqamb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gzizdgcat.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gpzslakhm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gwvzdrvyy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gpsmtzaxs.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gisiifajo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gwcgphmnc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gayhpaatv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gbkrrpfdz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gtlqxydod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gcsycdjgr.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gnjvfcldy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/glcrrgqqq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkzdqzzet.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gboakzjxu.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gnbwhlhjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtsuxnuof.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcxzxudnp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwrdhfcgy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/guyjyejdq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjekinph.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gpgxlxcvn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gbxpfdves.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/goqvvscda.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gwvkkkxwy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gjctufbxs.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gcgvgvjfq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gfxollbsd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gizhbsgfa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gkzcmqkko.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/goprjsivh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbfyhgo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/grxvmaamf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gxypnylar.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gqidovcbj.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gqavraxiv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gzrryhhjd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gqcaskklh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gfxkueanh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gbrflkqyd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gkdfzauan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/grxfbnnlm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gwfsfsvhk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gsbmjvoqd.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gtinisqmi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gxrnabaro.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghkpmjkik.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gcwdnvzrv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gwxufqsmo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ghvslzwcz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gpalieriy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gugxjrmvr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/grmnkxhlf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gjpejymdu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gnotfvirk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqaswijlv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzagyxv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gglutsfpq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gkecijpzu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gmvrbecre.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/ghalixtgt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/ggdgrgfxl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gypvuhywn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gqdgwqvgw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gztbcxpzy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gbvkunjhb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/ghoqnrgll.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/garqzedhd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gyfwniqfs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gndwrrajz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/guavlgies.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gcrezufdj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gxdzuuyop.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/ghpksfvvt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gejalanfp.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gyccdsljj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gksvworrm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gunbpizex.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/geddaiyqi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gntmpomhb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gqrdnjtvn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/glrpqaqjv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gfmatytfl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gnfriuvxz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gdxqhupqz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gstimwysa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gxjfvasza.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gynxhaewr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/ggpiuwfcg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gryhuvnyq.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gkbbiboab.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghgvuveed.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gfppvrrgi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gpavbqozg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gzxpjmazb.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gbfwqvcvo.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gzshjdalw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/ggylvzqnd.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/gmicerolz.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/grsrzxbra.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gthrhqvut.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/grbyjzmbl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gzockfaef.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gxcirqqap.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/ggwdmwiyt.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gwogjrnxr.sHtML


<!-- 参考信息 -->