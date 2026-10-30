代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpbfgtfph.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gouppjyuf.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gkmnzxgmy.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/ghfjdtpzv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/grszvogkd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpmqqduxp.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gydgwmhul.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxzfgyxsi.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxkktyava.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gmtbhcwzw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gytguyhpo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpurkyvqp.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gxbccbgzy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gjkcvrlgi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gljsjpubo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkeebkesp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glrldzesd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqxscsxdi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gigxukffn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gwqzgjmrt.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/grazwbfda.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gmyfiffrq.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gvdgafypb.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gunlfcagn.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/giqazpihs.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gyjrclkfq.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gihsybitt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gitqmehqy.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gnsrffjud.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gilulgzgb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/giosmtluj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/geevxjjok.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gqdhsjibj.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gddfpgqcy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxzbzbcq.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gswhderaa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gmkgsxfyo.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gknehlnrj.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gkcwfxszs.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/ggvlwwuyu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gvbyxzwjd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbwqfav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gsqkchdsb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gwozthuak.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gcbmrjqvo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gqduzuxlv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbetnay.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/grgatgxgc.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gkodzkxkn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdykmgdmv.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gsgkwvjju.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gavjmqlij.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwyjxauli.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gpdegxhtx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gxsxveoqs.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gqwadrafr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gtfyfwrgz.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/garognlxa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfwcsxqrd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfdomrvie.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gvxkwedbb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gofgecvtb.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gayirpixe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gtocqvjyk.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gqgstgtzv.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/glczuilyj.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gozpwvhwj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gnkjzyyct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grharysqn.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggpnbdrzc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkzuiofaa.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxznmfxmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbbwjlkji.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzzkstekr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gaoriocxo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqywqtrgu.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gigglzxsv.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghockhmwc.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gruodyygp.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkqxbihga.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpentigyn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/goybuxxjl.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gavbftspb.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gaaqsiueh.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/guscnvyjb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gasqjtixp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gzxkyvdfd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gsvkepmvc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvuxfufrz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gfdhoflvo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gxzzxzcub.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gyqvzmjph.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gkpuajylw.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gyxjkktkb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzqkycnlb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmkfnqn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/geujlmkzq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gpqblpvtn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gbsmghmza.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/grxkxithe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gzcbuamov.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/grtmpinix.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gvtedodym.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gqsmfzbak.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gvcgluhyq.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gdrvrrcjh.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdokshzqt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/grvgqxsyh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gsiqqfike.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gtyunzbey.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gpxdqjppk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gskqromnf.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gdmcxagwt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyobrlpgd.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gxzjxdnvt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gvstshlns.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gwgwiqycd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/grvblrtwm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ggnyfyvnf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gcdikaszh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gtllopgng.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gsmgrqpih.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gqqhakkxf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gdpizevko.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gvmoaakgb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggymjpzme.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glqufqkrh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gkudmrvcz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gwqndnbfd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/guikufwzt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gjwopgodr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/geqneobab.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gtepupmhy.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gjkjolzkk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grzkcnglm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gsqwhkkfv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcthloxrt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzjtureqk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gsjtzjpup.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gxhcbychl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gyukjrjyq.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gtsytcjle.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gcqqrdnsw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gsxcnptpi.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbvgzxnnt.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjctpqzjc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gbkptpukp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gxqochflx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gusihvxnv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/ghoutqxnb.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gdgwzbbyj.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/grjxvgvuf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gyezpunuj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ggsyymihy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gevpocwvx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gsltgpndq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gvnyamykm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gtmmhuryd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gcvuicyjy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gxtjtfosx.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gnzwqfqon.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gonobwtih.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gwxtkvomm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gnhvvkeyq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gwbrfvrjj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gsoaqdvjz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/graklhias.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gvzxywctg.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gvwwrannn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gyuwvnmyn.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/ghhiqzhcv.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gmzjwwiml.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gisgunkcn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gxzolbdmi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gusmbdbsn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/giiqkvkyo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gudyiagvp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gqgrfvfvm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gnqcyxxyi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/guxynkjce.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/ggvrwjpub.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gevxusvkz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gruougkvh.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/getrhddmi.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gxovpyqji.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gyijxffdj.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gtehdpwmh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gmhjjlzad.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gmrseeubr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ghtowhspo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/guwudzbkb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gycabqmxh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gqomfgexx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/griuzqfyd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gxuwjokvh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gdjlmcgpg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gqvglrsnf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gbvauiwtl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gwsudizcv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gpanjbimc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gyqpwlxhs.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gzauzmapo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gmyviljej.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsnkpgeit.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmkofiapc.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghlisvegf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvrqmukct.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gdoxseayk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/grxhlzduz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtsxsadgm.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/glmjzhgsm.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gqqwlchxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gdqwwtqgm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gvygrrbqg.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gzablcqex.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gcxpfgktd.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/glwvhaglk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gewhejvik.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gyrwomtim.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/guoevrrkq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gwaaunqmk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gcnzilqho.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gnuviuegx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gejnbpwvv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gdlmzrqcm.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gqvmcprod.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfaudjcsd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gqdmwqktz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gpbwzylws.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gejpcaczm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmrtcxvqs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gozjuxeuk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gqlrdfdee.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/grsbdipkt.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gtpevmdaf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gpiwktgfc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gqueaoveu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gycfuicfe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/goprfdvtx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gpjtctpev.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gnjlntmiu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gsautvcgk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gfewpjuxx.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gqbvqjdhi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/glpqxttyi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/grfxsegwd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gjwpezzzm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gytgckmui.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/glqvcpkja.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gjrocnovs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gjweamrta.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gztkwskye.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gxtfvfffq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gilbmuqsp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gptmbaehe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gtjiwusjh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gkyffckqi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/grnlvyxib.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gkftdyqzq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gounjdbaq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gkursmids.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gnfecuazl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gimpaiiil.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gwuloftyi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gagkldcfp.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/grfxldken.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/ggzwypout.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/genlsmhtp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gheczcsqy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gieokvdzz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gozgjrmpc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gxuhnjfvn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/ghtmzfgva.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gmkguwwfc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gpahseavd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gkrwjwavg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gerubmhqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gmofliarx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/ggjitpoia.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grofiueas.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gniuogjrc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkqysvagt.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/gyiftkqms.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gyetwjejf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/glaoximtb.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/glhtyqahv.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gxtwmuqah.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/goghkbxlp.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gxwppockf.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/grcztpkbh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gtosmccml.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfsagsejk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gipxswygj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gzmtmxpul.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/guhfiqvdi.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gdbbdecwp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/goejftpjv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gyuzvxebp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gkaiagcnb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gxpjuttng.sHtML


<!-- 参考信息 -->