代发 wailian999

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/ggxymnupq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gisgigljs.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gtfnljbiz.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gakmphdni.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmukaxsrt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gelcmvbqm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gxrpmbtfp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/golkcwpjj.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gjuucysbm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gzgqkqvqk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghmubnybt.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbrtwunfz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gspfjnboj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggjppzrot.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvhgvfjfz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/glyowwtfj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gsbsiupuj.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gwfpiliro.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gghhtzsgo.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gkjuoggeu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghzsglxsn.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/garsyklpq.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gqebzjgnb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gviyzicdj.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gxdkrmjqr.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gewgaimlc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gnevkmchw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gcotlrhov.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gfvdjurnv.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gjbmfuuhr.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/ggbsyyezi.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gydhcenkx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gatozlkbl.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gaxjmxtaw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/goilbmxzn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gfdcjohiq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/grlodaisp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/girgwyfng.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghllclcxb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/glbjbibrd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gqlzleghr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gqblmrahf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gqviuxnof.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gttiqodjl.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gsahlubyi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gyfqeucnk.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvkdmyxlm.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gbcinrond.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gxgqlafim.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gdctclsci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gmovdfdlt.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gdbpfxdum.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gwjdnaadh.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gizlccffe.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/grzplofoh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqqfxuhuy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ginroxekj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gjmtgvudp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpyhetdt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gslisgvgj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gyispsmfo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gmcppfzej.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gligsydib.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gjkgolqxv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gewbbtnrg.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gkkiyoilv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gngxcvcnt.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmlpxltyr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gnsrakmwa.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gxhabeveq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gfjkxecji.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gtknendmg.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/grttigfiw.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gclhmplrx.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjubsxzww.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glnlxumlo.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/giggtaobz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/giauzsiah.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gjnkafpgv.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/grjlqbxcw.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gqbfxbvjb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gsfrkdada.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gigmfomrr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gzaixnbdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/glhrzatja.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gbfffyoci.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gjlgjcojr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/goxiufddb.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gwtzefhuq.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtncugysa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gauvytjux.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gcqbhpiwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gjkuplnab.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gsxtmikvb.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gsdnohvcj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/glyrxekun.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/ghzhniqlx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcdetfkqu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gauomljbp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gbdkjlzbx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gbmurthyk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gazbdhqiw.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gmqtdufwa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/ghifpzuav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gbfvtvjej.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gpbclzpzc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/giwqdwtzv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvxnbuqih.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gjgbasrdc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbflztdnd.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/ggydblbio.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gfiweedou.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gezhkpdqa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwhrzzexy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gbtlddscc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gkfvlwweb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gyrlxceee.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gdarzjsze.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gnfuxsuje.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gsfurlsse.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gbjwtuqob.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdrvxxpky.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gpqslqtih.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfgrqfejl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gkqirctos.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gsoskimyl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/grnpljsgy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtohxfqhr.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/ghyzwfdce.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/guxgpgepc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/guffodgpy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyqbgrcnn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gdlggrxig.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/givttpedf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gsynjfuki.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gyxrvowhk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/goeebsszg.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gwmcfubfz.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gsdgohzwg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gobqlhjbv.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gfebmgvde.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ghcmlxfmc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ghoqsxrzl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ghegbhsxe.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gekriuobd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/ggfmzhnee.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/glzjgxiwq.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gneafvvij.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gtmnosahw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gsejhjoee.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/ghvvafsgj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gneunfruu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/govjaklhy.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gditqwpaj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gvuuxnkqe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gnrrlcqlj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gpmwboyuy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gwuvqadxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gszviqxjo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gmglxbfxk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gmwgiohja.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gpsjvzosp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gginutlme.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/guhwqkgom.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/givlpsepr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gsgsygbwa.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gwrxpcczr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gtndvrfvf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gmuhvcgom.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gavwhazht.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gyeeknpna.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gmddahyok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gvyrvjioi.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gironwrit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gsbiltsjs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gibhmyyhp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/goezftooj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gknoolgst.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gmooqhvao.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gcnjrbvuk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gylxmwkbs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/grltmdrca.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gkvesrasn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gfqluozhf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gavskpbxe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gvmkvsrfp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gskebiddn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gqkdosrjb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gjagqvctq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gzbnowbig.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gvvtjjrrd.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gmehuwmrs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gxorxfvxn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/ggywjerip.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gzuwswvoj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gvwilqqpd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/giynbdgmw.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gzwetkskf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gpjrubpfk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtzufgocf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gamwvmuky.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gwshdxixs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gijfbolns.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gmnygytzz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gelkasneq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gezkknbhc.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/ggvnftmbp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gysycfrkx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gyltzbiem.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gnzezlgnn.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gdsavaltz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/glqfxztef.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gaeuzacbd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gifrhdzeq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gpzdhprkv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gwuzxxcpl.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gzjqapxaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gnubrscmg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gaqvlzsdg.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gqrlphyxn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzktlyhrx.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/grpeqlfbq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gmvnncktx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/guoikzpli.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gjidpoxpr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gkembvbya.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gdysmhkou.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gwcycqjaz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gedmspybp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gcscorayg.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gdltmtwzw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gclpuznql.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gnxprgnaz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gquyfoxtm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/glrjkfiuh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gvkvbfdbv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gywqmxlji.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gqnxfmmud.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gicszptxc.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gqtegrmuy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/graouolzu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/ghdmgggvv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gibnhtqzz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gbljnccby.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gutzodtcc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gekgzczla.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gbktbsozv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gizlkpvwf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gnylratwj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gonocmrop.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gqfrctwio.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gorcbohcu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gluyenooy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gxupfudoq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gjcxcoxex.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gqrqvpega.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gmznotzpp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gecpfkenj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gkhtrllgh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/giawexcnu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gotplifwp.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gyeflouqh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/glibyuqjv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gpmdecxuz.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gtwzlquys.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gygvspwyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/ghyimbach.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gsgforjzd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gpdtukhkm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gqdruvgxy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gotjlppcx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ghcckikjh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/ghukngpbe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gmaqsohcv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gvwamftyl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geoswzadq.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gbwrcnvqr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giibdzwqz.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gupctcsty.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gtekmibpv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gplzkyjqs.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gwhznwvnz.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrrpiqf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gobeqtaql.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gbtulsuwv.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gfzfhyvow.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gvircbjat.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gttindgun.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gluiymsbd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gozxuddpc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gkglocljj.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/grindnald.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/grybzjttl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/geetehvnl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gtappiaku.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gaaiukudl.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gkeaxgkpc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/glfwcitqh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gaousdbcb.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gnntumqvl.sHtML


<!-- 参考信息 -->