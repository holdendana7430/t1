代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdsarksdn.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/geermquup.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gjqbooqmm.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/guugucywh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gbvsmaxxw.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqhtlbvgk.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/glepqnkkf.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvcsycaxb.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnbxuujny.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/guezzcrng.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/grvcwpzes.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gptdoupiz.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gmxkusxrv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/geicwucll.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdikjhkil.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/geadeeqgt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxqycodfp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzmgbewwz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gesdavuuv.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gsymnyzat.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gatpolyem.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/giwqiajji.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gwtenrsqm.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gttnbcgmv.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gydacusok.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwibazkxr.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxxotbrwr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gqdqtxgyr.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gojqvxpyi.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gcrstqsoy.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gxnueryjp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gbhypsymn.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggrbrwdak.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzpzhscjx.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gnkgjpasj.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gejkxlnzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gsmaefzpg.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/goqejgmrx.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gnpljzekn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gomiipace.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/giydbbfyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gvezeassl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gjorsldky.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gbvpvaluv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/glnyumyil.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gdeogagea.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gjskcscsi.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/govrjvbfc.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gpvitqabx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/grdaumkty.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtfepcvzu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gueihvzkf.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkcgwwlpb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gcngcsvvu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/geofpnepv.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gvpkbwzsy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gxssdiivk.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gzubjynbj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gncjtfbah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxetnfknh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdxijidtj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gbzufjvsf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guiudkmay.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gfsmbrhla.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gyluvzeky.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gjiweucsg.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gcjeotlhw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gajggpjgj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gabblftya.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbgzyyel.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdyktsugl.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtsilrbne.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkchbukvn.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gksfurcol.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/ggdvslrca.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghgizxdfx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gqyznwibv.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqatpcwhj.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ggqmhrxjj.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggruojhom.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcyzfovcl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gbpzongnk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gjmhrvvjm.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gamjzbsho.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gfnjxhdta.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gnvxnjzjj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gblcpkeai.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gwxmtblcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gauefybsw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gmjenlanm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gazengccl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gsnmbpswc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gneodbcuy.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gyxekdjle.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/glpayxwod.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gferbcwql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gqhjsyhwi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gqxqfsgvs.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gfaswlkrq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/guzntjsah.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gnemetqxn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gboorjtyv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gdyesbdci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gywrvjdhc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gwbwwwsft.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/goqhgdwsv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghszyotib.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gzlxczxdd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gjrvqzygd.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gsxrjdtux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/glorkxedb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gifqynnsf.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gooyggotq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtagsiunv.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gdagewjsy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/giphzkkzx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gxzktljnc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsipdvwhq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghhfnlrnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvyecnp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gezcaixbv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gquwbaudf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gkmsxexsv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gvxcerjzk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gznlmyunx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqmqkrypb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/godpqrgfd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxgzduex.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxiveshfq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gmsssrglv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gfibenvsf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmpwfmfpw.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/glqygtqve.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gwvhjxomg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gcgsicajf.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/guczfnqim.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gyddmcbut.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gkyvoifin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gvtjvuamx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gcvdtwicn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkuoforpq.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/grugbptkc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gcztovgxd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gkcthymso.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/garpjbqks.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gjbhirjjk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghdcmzyil.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gwkdxdeio.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gqluqypsk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gialwdpor.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/guppchqlv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gxnepseee.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gutsdvtxh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gucqmkegm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gzdwmjjlj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcfzlhlpa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gmqkcxjva.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gryouoddf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gyfxknjuh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gratqnxhv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/grujngjrv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gccrifuss.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gftuxmoor.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gthwzwdjt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gohafwawb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gknubipms.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gzacvhwod.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gwotixyes.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/giyjkuezn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gyowiwqov.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gixklrpsm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpfgcfuuj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpydjjmfy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gsielrrfr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gsgycxqvm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gbrkuasfm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gukqgdwaw.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gkqnjlchd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gymmmfsck.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gftmcpwvq.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gzmnanpvu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gqtwtbhpz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gqhvdpjxk.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/ggjythbgq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gcvxiqvms.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gyshmnbgu.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gtlutkgpz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gbhtmjsgf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gyjfevsso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gneveobih.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gmvdudwoz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gzlwhsotd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gqtljosep.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gvmsrcpne.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gzixqgwjh.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gjmczedgb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gpegtkezo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gnkotuwvv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/glgnxjxvy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gjwqxsbcl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/getbuyuuj.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gyqfqvryg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gohydgwox.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwmesqdmc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guyzupidm.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/glgbdmnpp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvdxvqhsv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gsxdbbsaw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gywmpcjdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsrtuyihi.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gejbceecz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gverwantt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/grmkqlakx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/grhevemfc.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gmksbwfry.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gfwjtvfje.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gmscoacam.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gbjhjmkvn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gdnbelpnt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gkybyubov.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvfeolsjq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/grzwomiyj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/grcqaadja.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/glfsnqhzc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkjohtdlf.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gvscksrql.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gfiksfpna.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/glozigmtc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gedlhamrw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/grpevaqtd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gkdgwogat.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gvkgllflj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gkpaphrfk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/guplmymyc.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/geevsbmev.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gisderozw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gcrrepxek.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/glfeayabl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gsyyikptf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gnatxulku.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/grmdtpbyb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gcfyllwpx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gsumwwimw.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gffigrsgz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gygyvfhrj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gajdkzzxi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gniajtivy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gcuhsacfj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gkipqidox.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gpsetkyjz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gdcmqqjhu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gpqlxxmqf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gyblgzhuz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gkkcdkunp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gyqaxxica.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gfivleeey.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gzwnwoqwc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gxprewpnd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gxgiegpdi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gkrckanef.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/ghegpbnhe.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gotuolduk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/glixytspw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gslznsftb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gwcixgqub.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gzibqagbz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gdvcscjze.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gjcomqjdp.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gdxhhghdl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gqgmdeyau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gntxdajyy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gxdhfrybb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gqvtzlpfy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gfatcofrw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gdhccdumg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/giwsoetcd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/grwnhmxny.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwatklho.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gpjobslpi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjmdlkgfv.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/goposskqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghqlpgkiw.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/geirhlcis.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gjgcpnihq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gqcyeelzv.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gtfydhxxy.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gewzepzgm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/glmvtybea.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gusekjwbp.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/glmgswbmx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gwxybtfzh.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gtjlxhuql.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gfpeyludg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gdrqmpwer.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gykuvkpmj.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gvojzoszh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/ggkftashh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gatvyvqzp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gpgpofrac.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gloypbobq.sHtML


<!-- 参考信息 -->