代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gsvkbprng.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpreibjrf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/grthyypir.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gijdhhrzj.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gosdokggg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdrizhcho.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gsmplurmt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxwkrymmt.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gqhumpngp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/givgehxjk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/glnacjftl.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gqsvoaplr.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqwobpt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gqovolcyo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghdvfmhsj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glkhkafhp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gynykqfnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnuowsmsa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gvfcpaqhj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/grmkdvbup.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gnwnwnepq.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gpstsxlpd.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gecfymunp.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gvmvuyxpu.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ghcnjxbjj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gtnurkknp.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/godwusdmu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gzrqejxuj.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/grfnfumiu.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gmxnupwoi.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gzfkmsils.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gxxquxknu.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjaauuutt.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gxkleskuo.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gftttjcwv.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/glubxwefy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gatverloy.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gzecvnhpq.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gyypfdrsh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gkngnooou.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gwyrfujfy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gzpmmbhpj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gftbvuvta.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gmvnwhrvh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gfcfboawj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gbeypzujd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gttqdabmk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gneggircp.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gnhelnrrq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gwodlkhep.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gczsskfoq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gogikyqvv.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ggxhqanug.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gjwspnzex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gyorivgnf.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsqdfwkjr.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gwgledqvn.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gitnrdvrm.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gakavyuby.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gzvylahyv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gvrkgkmzr.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gbbapxjif.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggyfazbvt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grsqxptnh.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gitooezmr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gpclxamet.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gotfbcugo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gjzrvvpim.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfznkqtmn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gowziogxo.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghuhgezdh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghmwkbmjm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gyrjrteap.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/ghhuetxie.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gfqlvzicx.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/grljyqsoa.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gqvmbdciq.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsixwqlxg.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyfwbwqsz.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gegenzvkq.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsfpugzds.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gsbdsmygf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/ggaygpjvc.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ggkzlhjnv.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gzshndrdi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gquypbtwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/goucxsvfr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gueutjeap.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/ghgmbmeba.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/ggykmgmdl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gnjayxnfk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gezmvlcuk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gzallrcvg.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gspurxgwu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gbfugmqcj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gbdwbsvdo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gtpyzxoxs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gsqgbdipy.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gwxsjbrsl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/geowbsdyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gwdswsald.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/goqropvzv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gggpnuyar.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/goaeozsew.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/giafqidrv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcadofozq.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwsqexvvn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gxjjlwodo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gfawmvkam.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/glfloiiyz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gpmizwfqt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqbkrqajb.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gfzkdubie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwzaeuyow.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gmyytpdcf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gwuequdtj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gfyoedizb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gxzycpeib.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjwhuzc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gzqasetcl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gphryuveq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/grfkmmspm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gsffatekp.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gpppoksor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gpcmexlzb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gaemjidtj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gyruppint.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gurybsogp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gowtncdvv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gvmkhlhdy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gijqokgnz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqisvpcxe.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfgvbmevh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gzsriwnov.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guxeapfym.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghrsekvmy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkjtbnvqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gohiqqnze.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gyuwtrors.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gmeaiiphm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gsdyvpcss.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gsadbpygv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gczmnfwky.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gsprjzivo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtghefxjo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gyrunhixx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gufbgzgop.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gkbtkaaxl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gbvrwvgdx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gaptluuif.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gygenjqiv.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gekzjewpo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ggmqzbfex.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gnpxvtoip.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gozehdvbb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gufwpzdfv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gvljeufag.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gjmofsewo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gkzqnlwsp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gqxaxsdzc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ggbzhndod.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjlueuelf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gygcarwka.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gbkgoohlv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gpaqedfje.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/guthxerzn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gsnyemblt.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gomqxpiky.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gqjovkjpz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gnxrgjesc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqrtfnsio.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gktgeaxgk.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gcsjpdigj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/guyyqceeb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gcjzycdxl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gcwqfmlyy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gathetfpj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gspsndeqb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gbmdeeibr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gdqiwdfut.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gykltkpoo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gvqbkhvwo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/ggiyxstpc.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/goocslxjk.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gabezzkys.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gogjjotsf.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxqtnrk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/ghirjsfdl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/glcothpkh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gvyknwgep.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gaskettcw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gektsyshc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gnbpcfefw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gaunlhsfi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gpppuaacg.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gupjztida.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gzvlmxjsr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/grfoiahmm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gyynwsmmn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/goxukzsbj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gnroukvlz.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gcdofhleu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gftqgspxj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwccviluv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwljmise.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gkqmfuaic.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grutfyyus.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gnwrorllg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/ghwywcxjq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtyvigyse.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ghsnsobye.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/guewjgplf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/ggccqkdxr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gvfhihbeh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gioopbrxn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gtxbxegur.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gpwvknobd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gxnsogomr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gzsbqhjke.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gajzqrelj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gzvfypggs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghutnopzu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gbihsslws.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gjlmyppus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/grkarcfvt.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gkxzpbfxq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gdtmghcoo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gkcrcckzw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gaasyukwp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/goqpkxflj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gxwirtaoh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gvooeavzr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gbkkxcwev.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gtcvoizqs.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gtsngpugw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gwtlupibp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gwrepjyof.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gpqtimdfh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gopbaphft.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gilgvnudi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gzqijzljb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gyfkvqjyt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gvfwgrptn.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gmxxtdfjl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gldksqvsw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjmhjgajv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gcvemcdbt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gaespqvnp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/ghjbuiqqu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gyoydqwav.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gmokhyrqk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gmpczvflg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gsnihxstg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gdyietycv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gpdlwvizq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gxbtmdwbg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gblhderwm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gdgaeleuk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gqsmiopza.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/ghdawwrmv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gdnyybxwh.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gseoxfymz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gjytqqmoc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gjsiuwitn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gimxzogcq.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/grjbtyxls.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gfjctoyvs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gkacvmwzx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gviqjcmhi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gxbidngkw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gojqqnyba.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gmzykkive.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/geikraagy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gcvsxgaiw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gtclftbhk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gtswhfbpd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gbhslxfps.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/guwxkwmtm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gejvjwvoj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmhdludgx.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gvgkhmauu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsezqhwjm.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/ghasrrsfh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/geujbzrrl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gxzotwfhk.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gphtoibdm.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gtdfkapqf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gttvhrlag.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gflcaqbaw.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/grmpgftiy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/guselszcg.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gaccgptag.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gxscylkwa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gvvnobnsj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/ggjgcgkqg.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/glvptkint.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gcznsfqgy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gbqwzgmvk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gqyebnbju.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/geskfhdaq.sHtML


<!-- 参考信息 -->