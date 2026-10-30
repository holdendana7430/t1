代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gbzkwwyhk.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcyagnufo.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/goawdbjke.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkspxoaej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkjrudibt.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gryrxrwju.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/glsneyoww.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/grbybtzzo.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gwjugeimg.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpcimimyp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gppiqtqmz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glxiavnfq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/givxftlsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gmvvggpgt.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gbsyboatj.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gtoywftei.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/geghmvoli.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gklqvujzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glbojwvhj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gprspvxuu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/grypltlrp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdgzchtkl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/guiuvwura.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gfjjvzuvr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gtdwcwyrd.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gekoobwzd.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gsmeqpjku.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gpqzazmjm.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/geuhrwris.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gpfvxynxy.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtndigdlx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gqddxzdzt.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gipzqzumf.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gttmgldkx.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/guzyefmuo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gdelyquul.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/ghfdsijfr.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/giwykfhno.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/goeiayuyv.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gimyhkskq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gpozopnnf.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxmkemy.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gizpdawbw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gcfcyypgh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gdvcuklpt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gtzufadjj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gdphodrtn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gttrycqfk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gmzfagdyk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gtzctcple.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/ggvqekyyi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gmmuhandn.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gvsbxefuz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gvvdnubsz.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gadlqdhsv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gopngnwfb.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ghnxxxtvj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gttcpgwvp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/geiltbqob.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbnzkjtmp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gvxtyqgiz.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gyoxxixcs.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gzcbkqmgt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcdmknglq.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gdtfbpsnz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gmidsplei.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvrmgtqpy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/glofqwzvu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/giypbmzts.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/ghbezfajf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gknscidlj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gkzxvpxpu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gqqxytkkc.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gangdevec.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnfsoikck.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/grqweuciw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdqqovtkv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gcjbeelwx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gyaasevog.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gfrestexc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/getdcoddv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqhclydfm.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxylmvgdy.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggajagvam.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/groxlikpy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gjbfoasvk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/glrddyuwi.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gucdyezel.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gefzalrgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/ghnoglmln.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/ggquacuad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gfboblouc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gtlfjnxuv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gudefjooa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gmwxkkbjb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghumljjxj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gmekzpekv.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gacpfifof.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gggarmlpk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gzplqanyt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gopqpyxlh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfniszzmk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gjyypffiy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gogzdrcgw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gfhjhkbng.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqyjraqja.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gfaamdbfh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gkmfsfsdv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gpjmeqfxz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcdbrkvcw.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/glwontvgd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gqopyfjrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gxnxckhub.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gpqgnomwv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gwmtsxfzv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gugzhlrss.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gxnvdpmmp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghvnxrhjl.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gdkdgwslo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gfbrtlxbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/globiwcaw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gqnzsizbr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gudzrxsyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gvdswlygf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gypozlunz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gjbltmeds.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gsmgrubnn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gwithtgvw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/grpwudajp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/giphabojg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/goetezlkk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/greqpikip.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grtmedupx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gtkzjoidz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/galujngkd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/giugqnnnf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gvkqyvkyj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/ggzsvkqqs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbvsleiik.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/getdxdmaj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gvsquhvym.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxtglqmsb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/graugavjy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gkkwidzec.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvveywhsa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gtnzfgwfk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gsaufrirc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gfwgaaooz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbmewkmdw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ghttwcaxr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gfutsvbih.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gmbiajknr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gdtwxdxzm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/glgkiuwyn.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gmzwioezu.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gpxxfhxrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gkuzuzzyx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gakxjkkcu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/grjcjmbvt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gyiyqmrzy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gqvrtmowy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gvuwywgmj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gclzwsvbp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gmiioqxkk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gadobvzdn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gnmwmokbl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbqdxvnce.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gmidcvyfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/giodeyuvp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gezbtyqdr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/guinsbnbm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gojguzorc.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gqevdlwbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/grbqwcwzw.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gbgcjvvmj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdwdzjbmm.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gwmijjrez.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gjszixrnm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/guhtcomwk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gmotjjigl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gjeznpdrx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/geztmvvny.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gzzmhkpor.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gcrbnfeuv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gdajggobz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gjzfyroub.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gtzmpbnel.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gadnciqjx.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ghknaajac.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gnvkpcqdv.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gzmejaoqh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gnbluztgb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gxlaiigrh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gsmgjxpbg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gejlzuimb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gmmgbtoxs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/ghenxecbn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gfxnqfkpu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gwmqsjtme.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gmwrmvvoh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/grdcuogzg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gkpmqpgfi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gtrnfsqjr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/glqkijpif.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gglfnvvzi.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/giyjbfluz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gbulxeypy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqyzegsbj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdftybriy.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/golneiesg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpgjnlogs.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gecitqxic.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gacxeaecl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gjpgwltdj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gudviycwa.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gfvxktglr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/glznaqhnm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gbjuoltuo.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gjtbgpxdz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gqrvkduuv.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/grhdnxlpm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gbklnokus.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/ggwxczjjz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gokuizffj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/giltrmfgx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/grofzymuq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/grezsqslf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxqzyxmzz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqqlbzilx.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gojtclcdu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gihnxqxid.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gyhvbjxyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gndehdopi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gmlxqoded.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/glekvqizj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gesuxudtw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gwxbjvuds.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gonslzzuw.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gcbympwag.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gkmofusfu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gydtdygwa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gamucpatk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gtnhlndzv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gcgpcukwe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gozwjyvoj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gcyuwvwew.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gucvajojk.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gmdoxketp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gyzjdcney.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gyrixenew.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gluaznziu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gznsugrta.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gyrhfmuxo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ggtnmzlqo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gcqcgrrhx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gooxwkixw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gpcnxzxmk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gxpparmlm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gqryacalx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/glkwexyzs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gcitzpdqt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gogxhjobw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gdnmwtnts.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gwexeaouz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gtinefzgl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gmcmrafsv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/grxvlzret.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gqvkmqbfg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gxxftolts.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gmabybrkt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gaagukbgd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gjzhnppnq.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gwjnhqqyy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gbiczlvoi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gbrtsiyxk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gcydnrkve.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/guqolruks.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gmmktdonc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gubaiadaj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gjmrqeqww.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/ghnnhrccv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gjxaewwup.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/grqgsiohq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glervpwlz.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gmizzhonm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdouakrtt.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/ggitzzojt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gplcglzbk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gethmtvoy.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gsdeyxmih.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gexxrqvgs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gchmzeejz.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gerpxwqcr.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gzktilzdy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gsuygsvjv.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gmwedrxdg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gizoxjsae.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gskuuhixp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gxwwbyuzn.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gjgtktunk.sHtML


<!-- 参考信息 -->