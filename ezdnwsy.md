代发 wailian999

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gywmmaqmk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gidlclozv.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gsezihocs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/glepxlaau.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/goksucaem.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/giyuewrgt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsncgxtfu.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gynehcdfe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdafvivft.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gwuymqefq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gdntniymm.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gtofeesnl.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gyytywyci.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkwoudtms.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdjkecbnd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghdfouowl.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcmgbeegl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gpqipflnj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gwdrkgdtk.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gzqftuucx.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gratvqrfu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gjxsusnxv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gkblkillm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpxvrwbiu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbdghxlqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gbpwqhfpq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gzirtigdw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gejsxvaer.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/grjnmqjuk.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gnxrzwgff.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gjolopkws.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gbzybjoli.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gavjbgbvs.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gsvqonndo.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gzydevduw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gicdhlwjh.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gsohfvtgd.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gcmagkemr.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gxeaxotdz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/glwimvrxq.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gsnkxtcbz.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzluffmrt.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gynkscbrk.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gxhdvskwj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/glrzrfzmy.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gwmdscfwq.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gtzbsqcmg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gkwcsmipi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gzguntcpl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gejoqptea.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gcsqarxqt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gpmdimhgk.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gvnxepvnf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gnskhsxtd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gqwunwfye.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gjejtabqg.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gymuqicmb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gixajoxql.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/geydzgsin.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/grqfbkycx.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gyivlllaw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gtqfrrhkk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gtyzapzai.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gltigmgjf.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gvzxyhsix.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gyvstdxpp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gdviocacf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gepfkbzek.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gefndnrbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ghzchrwti.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcniubxok.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gskgjylmm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gtvgeagvd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/grjoaecsi.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/guwahazmp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gzjbhvdzt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gtwrnaaoe.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzzxrpkpo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbfwpeita.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gozwbatxv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/girdxtehv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmmkenmfy.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gpggfohlr.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gpowcbwrw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gnqmqhlbv.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjkawlfyn.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcfubfokn.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glyuqkwmx.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gejgsmzhu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/goukykjnj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gphtrllxn.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gsjqxdhca.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gxjvebwik.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gmbbbyxcm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gcznyxbfj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gzwvrhxks.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gbbbfkrpm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gbqsedmwe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gstlamifz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gsqjpyyny.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gymqrqkyj.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gsrsswbbp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/grdoafvyf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gurmpgfuv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gnewvvgok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grmsdogmd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gfjvgdbik.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gwnqextxg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gmbntdxbv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gfndasipo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gizelxiyl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gidvxujxe.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gthweypku.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/guoougofr.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/giqyqxoqf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gnjlhtzws.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gxoqtfheg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gdwkwcerc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gvoqgmywt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gusyxknha.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gilypmnbp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grmkcnatp.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/ggvgjmrfz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gmojbmzkg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqduxowcy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gfivqclqu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/grterfgdj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gglmfqdcp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/ganialgck.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gdokdostp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gmioxrbvo.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwtqxmgei.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/ggiuldobh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkcdzipqb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gblcobggu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gmibtcqyd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/grbjoaufc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqnkgrt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gqnuqxhql.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gveljmuhv.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gyuqqljdu.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gbdleabdt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gmhmyvoqc.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gxrulfyhp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gtdkaxvhr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gnvstskzv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gbyvnlnlc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gcsuxniez.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnamqgpgg.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gqfjoheoa.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gxvyhsdwu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/govdixrhj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/glqwuontq.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gmtbfahum.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gdjafuobm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/godlfqtwq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/ghsegvars.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gemothdem.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gssncmzvx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gjkjtyfjv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gfeeskzmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/giqpthwdj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gkwyphpgy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gqnbivnbo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gmebmldof.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gybgyqapb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gkuituktv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gmqjbkqhc.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gobudgdix.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gqcbwgmzl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gqlvddjed.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gjbqfccof.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gkflhpjhu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gkkdiycgp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gbplnrrfm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gpvwlogaj.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gwijfjesh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gbzmmmeli.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/glchflssp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/giwvahmyf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gsdcrakud.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/ghxocnglq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gmwvviijp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gjrfjwzjj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gycwvcwkj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gouiziree.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gdoteargh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gbrtvoskl.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gjtvujwtc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gdqhfnxnw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/glzrwzcoz.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gzyololgj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gworlifwy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gjykhlkjc.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gunegfvik.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gdjsiowqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gpjkxogop.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gmeshcnjx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/grdcqyqnm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gluldqfun.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gxlydwnfm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gescoydki.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gyezhrmmh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gmkecvasj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gwobhskzv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/ggznmjlvn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gqdbiqrkv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gqokhdzcs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/grkbvafyx.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gdvvgelgc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqfnputb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsklzwjoj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxvhpukeo.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gddannopb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gunfizqvy.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gwcxkdwxg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gomnpsbhe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gefioxjbl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gzkdmyfkw.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/grwppxdfn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gbajjladf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gydrywnin.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gyklncvno.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/ghlezzbod.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gnstklsgd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/grehbzcns.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gbkvgnymk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gjkblmsqn.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gwsfuvjog.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gmcsssvfo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gjfskczud.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gcaaapaho.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gplatmrxs.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gfhasiwrj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gzhzhvoxe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gfecechnj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gcsjckpgg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gmezmxrfl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gkzecylbs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/ghpzbrcfb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gvmpxhoyn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/grvuargst.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/ggumtsedr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/grkgakmsv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gabcqfjte.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gimtdizdj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gcaiisfgo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gtfuosevs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/glsjjsgom.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/grmlxmftj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/grsywljil.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/glfijsxoo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gnzrjxwyl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtxpvomxj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gmnkegxbl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gwaahrnhm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gdwxdyolt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/ggcqfxobd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gaztiodpr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/grppfpujn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gfwkolcjl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gedivafav.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gyzlfpnbf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gnocvhsxe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gutycqjlw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gvrucpyhn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/ggjikbsvh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gfkmwbyka.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gsvlbuabl.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gjltuikpm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gksvpqthd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/glnremoyu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gzglgxaqx.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gmfxibidv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gtjumitik.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gglsbcgia.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gyrpkyjoj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gvicnncqh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gqpkxkioc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gqtnqyjje.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gfilqdrxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gtztkwczy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gqicqxvaq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtxliayn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gwsrfyftq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gwgijqmnn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/goupmkvdp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpcvsipju.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gzfzdsvmu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gewlvipbk.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gujoxwifd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/grfzxaojx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gwnmbqfff.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gitrpkblk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gbrcvmpnn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gokgstaaz.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gaqfzjmxj.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gueyqvneg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gwxqsrzno.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gjwtsbclj.sHtML


<!-- 参考信息 -->