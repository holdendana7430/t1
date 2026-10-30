代发 wailian999

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcwdovewa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/geemjymsr.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkckcki.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ginldcjlu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkfzrrsqi.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvihbmeyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdxvjgovz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gihyyahet.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/goevsygbz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gseavbgtk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghfglkkiq.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/grkiaaipg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gmvusuyox.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmstjounn.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gagesrbcx.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gybzeinpu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsgzrnikk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gnycsrzdn.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gfbfqnlpg.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gcjwtfamt.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gyaaglrlz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gyflodnmc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqeaxxipc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gylsbapgf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmeihsdhm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmiqnjbcj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/goufopavk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gnpfcrlyu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grhztszxl.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gmsgpouic.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/glkwrjbjr.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/glxcovkbj.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmvcfylsm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkbdfchtp.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/guvkjxsgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gfuupegjn.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gihlpopne.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gozqfpatd.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gopiysvec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gpzcbofni.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gbyfyzpjd.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gnitvjljl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbyrupzvw.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gieojgmte.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/glhfszmmk.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/givquybnz.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gfqqieaeh.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gwupdlxyd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/ggufpwjrz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gfgetuzce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/grbvzkqvv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gqexbdcpt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gclisoecn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gqmelqoyx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gwbdwhric.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/ggbhdevye.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gstrgwegg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/ghwcfldog.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvwwckuzc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gttbicsry.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvibblafl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/ggurloxpz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/guacvcbbj.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdaogafeu.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/giefnerzl.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gwfjwuqtg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/ghyxlxolh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzouetsx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/goqtyfazp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gehtssher.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gfkcekcsh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjlmwpvqa.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gusjjophc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gvvbsrepe.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/glrfjhley.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ghjyefkjj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/givkbgupk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/grzxqatel.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grqwtxsee.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gjhqycscy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghejdtblk.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gsidduuhq.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxzvkounb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gsunzlbyi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gscnhpzlu.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/govfycwno.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpjkewilw.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gepeegtrm.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwcfotgft.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gyojmcnym.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gucmjdvee.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gmymrtsnd.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gocdlivma.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmvobyuqn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gimszzaup.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gpypipjdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gkjtwlftw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gktrbwhyy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gtuwkjdsb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gfsykrqke.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gzaxjslna.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdqsbuxar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gtngznlet.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gidngxtix.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gjgkvhlnb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gxxvhsutx.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gaprczcum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gijgrieus.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gjyvqllfg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdzkrdish.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gpwtzbden.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/ghrumzlor.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsewfomc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gxtbdoyfy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwxvzxkrg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gdjyhddqt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gwgjyldth.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gfryfpvxb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gerjuszub.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyihhsuxp.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gvpexawjo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvcquunbw.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gyhpivlco.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gjejgqrfi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/ghubbiwgo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gvnespnik.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gxpzwgvhc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gstulcyxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gyxaxjwmi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gczinxilp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/ggsjcsizd.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gvhvilock.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gllozgwnh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvwdstgnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqewqopxt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyrmqgzvf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/giicapach.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ggwfvpijj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gkpmpppwt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfdjtpqcq.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/guoixfpmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gepajwuvc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcvkyxeee.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gmyrjxsnh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbjjjqvdp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/giwdpoune.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gwzsqmogo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gofjwsphq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gnvvseldt.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gyhsrziac.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gonqfmkzz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gnylzhlkn.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gznladfsu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gfhkpmfla.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gpdleexbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gayerqlvg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gdrpujrir.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gszccktpa.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwrkfcy.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/ggllqdfdt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gdwinqsas.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gfrfdbmsm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gmlyykhpd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gxxsxpixi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gdkabhzly.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gllcobphj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gltvxvymy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/guhpslhii.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/ghnhkugua.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/giydgvtso.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gnevksxbd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwtiognpu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/ghqwimfmq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gssckiokg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/guadxhnhq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwojmebbd.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/grormnpin.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gboamqoim.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gknqiokyv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gzekzzyjg.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gotqwaaea.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gozqjqmhr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gygecqxhz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gxkpobmqz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/garssgyhl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gciflvsya.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gwbaykgxz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/ginzymfig.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gynmruxrt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gthfhxglx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gjdrevpni.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gsjjqzeih.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/grpjfbfvi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gqdemahri.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gpnxnofmj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gyxnxerqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gfdsfvnfe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gxtqcysgr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gciirpflj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gsemkkccj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gydbvulju.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gcocnwwib.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gkdnmwwvc.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/grwqqhhoq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gdqhjikfi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gpfycwebc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gzitnrevm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/golnmpqsy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/grbkbfgwu.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gkqeffrxy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/giwnodcid.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpnpvdnxo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghjefqoui.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbojsuknb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxcebdqcx.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gznlarfjt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gejhmxcmg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/grunxpslt.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/grooasolf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gsozsjjlr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gxexmkncj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gjvlfqecu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/guyxmndfy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gpaorgkax.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gykdaxlhk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gmdouqmfs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/guqmmpwbn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gdpaojlvn.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gygmmtnzr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/ghawjioll.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gzgfsdvcz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gstaizwiq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gstrblxpv.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gcxqmfhkf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gbimxzpcy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gypfuqozs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gebbqflbt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gcylbckym.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/genqimwas.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gvfzvwqec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/getjdlcde.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gdcidcxed.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gukvxahiz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/ghgngzobw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdnqonynx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggzkaiefn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjzxijfya.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlovvelb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gvolyoycr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gsszfpbkq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gakcuidyc.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gvddsoupj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gwdtcyiqo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gtelnulps.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gbjfgcrlj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gvduqwdah.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gsjgkchey.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gyznhewdj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gdknbfqes.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gvotmkfrt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gtznocswd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/geinahozn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gmtahrveo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gkvodllse.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gxmiowfsn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gjzlzvzow.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/ghxubzrrg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdfvrcj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gxvvzoscr.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/goiifayfj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gcrjmcdgi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/ggwyvzdnq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gmvdcqlom.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gqeocfhgg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gfbybmhvs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/ggzvmcvsy.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gjdqvcris.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gdnepoqic.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwtprywar.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gyejxfept.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gxiollpyy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/ggspmzzeo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gbrwynfee.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gudqfzavu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gddrzwccf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gteiuofke.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gjzbyoadf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdjblpmcx.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gtkdvczlf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gytdcpxih.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/geoufbimr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/glzctgqvb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/grtkgixtl.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gldaavgbb.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gmcseilqp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gllhanmot.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gllasbsxy.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gvliqeufp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gyjgrckoi.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gwxnjjrgu.sHtML


<!-- 参考信息 -->