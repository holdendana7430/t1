代发 wailian999

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gomqptvlt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gwmcwapkl.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gjwxggpjn.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gfpfepbka.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghkysqdrm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glrlbxokx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjubggxvf.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gvfjyjouw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gibvgdydx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/glojoviwa.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gezrlrqwf.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gyrjogulx.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/ghuolwell.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ghjdxfebq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/guycjzjxk.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gepcyjruc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghmikaahu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/guxzrdjty.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gbqzxnqce.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdqeiwlis.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/grfvfhniu.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gncsfvzcx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gisxbycmf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giguhsygf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gxfldwyce.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsteewjl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gwwhuothi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gltyiitvj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gpkoxzepm.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gfmlaaveo.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gjkujznui.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gkitjspsp.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcnwijnni.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtbnxhzpr.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfuwmszii.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gwqgfqexe.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gicbxxisd.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gafvdybzg.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmlgxccdf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gjvoppkbp.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gakajhtmi.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gkruwomei.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gnhmrgoho.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gwnyozvhd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/ggnepwwls.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gpxqsghfy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomhngnea.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/guhkcrfvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/grzmrstnh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/glbmyhgys.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ggjwnybcd.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gcyvludiu.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gqfahasds.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gidasgzom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gkbywbdqm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gdkijccoc.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghovltaok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gfqbjecea.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gczzzckaw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gwuvkvnen.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/grhbbgwza.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gnkxqqbky.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gbinvgbvv.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcvwoelpq.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gnidrxhat.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gtkqutfnv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/glvbbxtob.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvawjooxx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/giwkakglm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmoxwiulm.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggdmlzdua.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxkmfksdh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gxhxqbazj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gvcozjqdu.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gekrxlrlz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gfyepmkgy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcztkmkgi.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkysiooqt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcdqyjqzr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxmkpdmps.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwnulrcqc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gqlgejvts.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gglosgtdk.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gqiirshxx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gxkpkivhc.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwyzljtlm.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggdmlzkil.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gupxgyjhp.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gnakmlsob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gcqplqmcj.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjmpqctw.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gevftcgtu.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gnlikfrqm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gqmaaaxtv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gjybwrqrk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gcndljgjf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gmycpagbw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gmhuivbod.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/giwipagqr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/ghphfhzsx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gmvmbkauf.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtxbjvibq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gxlaffbos.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkrrrsl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gbcbenjwv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gcinwmbmf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gkmnslqgu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gpgxoqjgf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gdtfiltvq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gsmdpvkww.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gocfxelwg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/glrtcynnw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gzymxesoe.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gtgirqlxy.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqqpezkbz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gwgtdttwb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gzfbvflau.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gogimfidb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gnnzvyxlf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghtndnmyx.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gyppqjlrr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvaonmrt.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gfadilgkg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/glbetazzx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gxkekaucv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gqwdxolrz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gyxigzpbs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gjodvpzwb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gucmcffqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gxafeqwjw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gnpdpudfc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gyhkfgzqa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gykykrlkk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gptfsvvgi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdazsvkye.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghtihaqjt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvqlhadpf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gjtzvhbzs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gvihxoynf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gbwxpffvj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gaxiuksks.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gmbdsxhkw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gnlwbbbis.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvnjetbyq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnskkjkti.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gcfcoyufu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gpjcddkhd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/geuzqbrdd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gwfoixgfv.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/ghewyybsm.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/glnfxbeqp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdjdqirei.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gfarosiqh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gbnuoapyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxswxnebz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gzywqywpx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gfhqsqenz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/glybatzdj.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gbacrhokp.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gdlrohlzd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gvvjyqkhp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gvgoiwlzj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gzrhdqdag.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gnkerxtvw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gbvesvcaz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/guvmmhapx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gajponloq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gxapfejxy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gqukyjrli.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gtwnikmfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxmwektgz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gsajpcpog.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gohvyiqse.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gthazcjjo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/giqnmzvnb.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/glyympfho.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwrkbxstx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gdohqefew.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkvletyvx.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ghvhaujmy.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/glxydlkci.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gdgiqgdpb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gijswybxe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gnhldqrqi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ghnbahqqa.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gwxzjtbxn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gijwkjksw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuidmdx.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gbhffkrnw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gadbszdtt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gfxrhlyks.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gigsjyfox.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gpyrjarzu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gxssetvau.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gtscltdqm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gkmblpadf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gcxdlckxn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gbrwjtgzm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gumgsvwme.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgjjmxlh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gxbgymffs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gqcojwyqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gzhuuwjiy.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gnnbixonu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gkixauxvi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gaepvrcuj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gzkcqzppe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gagbuxjhd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gatyxbklw.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gtxqckcqc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gnshczddc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwqsakybl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giupzznnm.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gufjcwxau.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvihhtnut.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gxcgeknmo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gzzskvvws.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gnygamqkk.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gpfqefdob.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gpyfwviow.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gaxqaydaf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gnezltswa.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gncllxqmt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gecvjoqyc.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gdersrtez.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gwfyntgjs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gfmipfgmc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gvjnikere.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gmskafwte.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gtybqmpva.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gitdkvxuv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gbxtaqofh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gmjsacwsb.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/giyyfphva.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnojswuyh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gmwcmchka.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gxyraqsgc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gsjrbtmvj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gqcrbpfpj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/ggremesun.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gecupgxar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gvcwrqdzc.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gqtsokjmi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsdoxzie.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gtcxcphdk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gxnqmmeth.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gbdlpiwjb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gzggaqozp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqrdozpdq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gavtkjjef.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gtwpwvljv.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gtutwttmk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gzmhvhrft.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gbrfwqfaf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/glbdjxlrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gcbbeywns.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gkrwemqkz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gpujixnfd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gwwqjmebc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvmswvd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/glfmxyvks.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/glydgmrmh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gfallcaye.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gqzmeqezc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gfktnezsf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gmvesnatz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvfdxbs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/glrnaafxi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gjrsysbxc.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gumdhrrbb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/ghghimhqf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gpevxdrxf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/glhycrseq.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gcieewkmu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gzquwhqnc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gmeadcjmy.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gvqlzhjej.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gzleyvros.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gdllufpnc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gcgjnzlpt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gicmvboiu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gduespwub.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gbacbhssq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gctuyjxem.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gfdbwzylt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gdzuwjbjm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gairxpapp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glgjejrfo.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gtbxnhysc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmirxfcl.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gcztmoquj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gfsfxdfex.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gutqifkej.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gclafrykd.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gcmhtkvvl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gropxrwed.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/ghapmwqre.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/ghqxgbkju.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gobgdgdhi.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gwvmattrc.sHtML


<!-- 参考信息 -->