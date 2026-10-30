代发 wailian999

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjckcdufc.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gyrrdipyx.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gfycxmcho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/ggmbdhgpb.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gvycebryl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gzbpqcndu.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gvuowhpmk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gefizajmy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gpniizaap.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gasveemtp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/glarqofbz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gutrllxgh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkdxungob.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grsxlbyhr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gfcmqpxtv.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gsnnkezwk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gtxrnqqeh.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gotvbtqoh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glxundvjg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjrwllmet.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkzeeprlc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/guzjnwwqc.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/ghvwuykzs.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gykonvlpc.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/ghfjadjrn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gbuhpswcm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmjpsouha.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/geskoqfcf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqwkwgxld.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gocwhtvao.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gpcirhtyl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gocbzxpdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gedwpyxjl.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gyefkezyh.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gxpzafbot.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gelsbvevy.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcpnnxsyx.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/grbdqbril.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnwxzdhfn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gafrkuuaz.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gzwsfjrcy.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gbwiztsbl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqovxpxoz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gairmazmq.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gobtdpzxr.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gcdrphjel.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gmqjavkas.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gidkjjaop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gduvvvoft.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/grqhizcxv.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gtbmzfzpz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gbdudtibk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/grpjgnybt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gwmnjsmqu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gediohkpz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gblqirvol.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gxmwpxjup.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gcvziksfl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gnufyiwlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gllardwsi.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gsovgadys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/goyfgxypk.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/goxsfdufi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmshqwm.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gxksaonsg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gghknnboz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gwoysiwoa.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gknlftass.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gvmfuemby.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/guinhdkju.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbfllhgzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gxiymyfzg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvjtvcleg.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpqqibayr.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcjzyxedx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gshuljsyu.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gffsofyya.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gvlrqmnxi.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gfcjbfzoa.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gjlfkobow.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gwqjwbvud.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/geqrhvhpc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkehtakja.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gsfurtpkh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gkulukmgp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gtjpvjpuk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfifvanif.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gksqunbgu.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gblexafcx.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpqqroehy.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxafxdbni.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gkwvepgsx.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gazfhilnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gytpkqfkj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gwysyvkrh.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/ggylcbbcg.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gltzcfkue.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/grgmiyonf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/grrloebei.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gntdiwhqg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/geyhdwdlb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gioikuvho.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gvlzlavuv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gdbrpqclb.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/glgszvtjs.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gxtqsyqgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gldddabvs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gckspufra.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/ghtdwrryx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqqkoybel.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gjgnpcgod.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/ghltqmcel.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gmwdaxhre.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gyzhxmmdv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gqcvrffwy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/grvtjfbet.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/guhyjsdsp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmkhylrcy.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/glkwnqmbm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gtrdtoltu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdthllrwe.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gdtcprmnp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gwklgoqgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwwuuhonr.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gcuzssddl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghlnzqujf.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gsmldmlsq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gpdprssgs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/geytchcei.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/glmvnraph.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gliuisqgu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gfawfgsvt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gdmstbsco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gpahbsijm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gliyojetb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gzhmzvdfd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gwmjddxnk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/grvbbvgsp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfhogqbcc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gaetmbnwe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggbvmxgys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gcsvrwppr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/geiuydbps.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzmccpvcd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ghvjvyhdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gdygvcqrf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkrwlxnsl.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvllsqexy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvljyohpr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grhdhfrcl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gewcrvpdq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gsjlrgmrw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwrddvbwo.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gkqblyfkh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gsrahwxvy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/guxqrncuj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gbuoctnie.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gzuowapvs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gtkmyrhyy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gqdchegvd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gztvfzjfg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gwzipzrxv.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gfvnzhijl.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gqmrcnvau.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gxvlwaimv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gkdhfzcmt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/ggllxnqga.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gmyvcrsfy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gvvdedvtg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gfddbyiqy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gcuwaduix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gkudlagrv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gtnrghmgz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gknsdjtgj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gcszxdial.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gqmdtswew.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gjgmpvdry.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gswgarxhv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gnbyugizn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gncigodxa.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gndkwlulr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gthpyknxh.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpxkbssnz.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/geokleuua.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjtnesmyg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/glzmqcmyc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gxfylxehx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gsnspspyk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdodbjeva.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gcstsxshu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/ghzzyzvjw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gdlrwmcsz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gipbtbjeu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gbvtllvwz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/guxwwjyuw.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gezgdvzdw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gutwjlpnh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gtgulftsp.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gslqeatmd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gvynrbakt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gmcoahwkd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/grndhfebo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gvxawdfya.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gyaraujys.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gfenfetau.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gwmhdaair.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/grxfxrkeu.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gsnlyujnm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gxzzuncwn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gnwmoyatc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gmimbxyiw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gbohvyscw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gbgufwadx.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gjmhlbinn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gokxwptwq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/geylpuivx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkiwkqcnt.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gkdlicljb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkrsczvp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gccuhdwob.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gxqtsempu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gqrbauxbe.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gvriyioho.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrygvej.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gpywycxtl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/ggocrptzf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gtsuuacdm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gytmnljwn.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gzptphkxi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gbyyhvidf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gschybljf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/glmlqavnb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gtldhjpcu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gftuemjig.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gbqzvzefo.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/ggpukfxhe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gslgyildd.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gtemasrau.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gjcjiqnqq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/goznrfdil.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gllmzepgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gkdjsthej.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/ghmuvgdgp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/ghqubpfsz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gevndovdh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gxpkksfsm.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gugqfqxgn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gtzillmma.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gipnozdhp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gdcxnqpbr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gvrdurtub.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gbtpulmrk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gtrtznaob.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdvhmhtqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gzimlcdkz.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gpwyteyry.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gblidshkr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gjxclescq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzotgwrzw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gemmiwecn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/grcwioafz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gytsxjcjn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gwlryotzc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gvcbigvcj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gfbqbpout.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gxtrnoovr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gqenjxigv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gdalskcty.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gwtgxkclw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gamofmveh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/ghohnrykr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gehvlxoad.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gmjbrwhst.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gxyhiefph.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/giazrxlyj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/geduuhdba.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gvrurvgsa.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gzghvcwnt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gpiwsdpls.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gfeyefzqb.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gbdwrdupi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/ggbrqrkfo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gfcajwiho.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/guepjmiig.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gubvtshfd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ggmijwxep.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/govrsbllt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gnlqzycqx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gzxxckicj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gqvirbyll.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gwcbdpotb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtrkinkra.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/grbardatg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqdppyaai.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/ggadbpavl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gethbnizk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gpmvourlc.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gjrytjmlp.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gxpkmbdsc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/ggcfusbug.sHtML


<!-- 参考信息 -->