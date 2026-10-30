代发 wailian999

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gnarmxfmt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/giaxgtkyc.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/grxajtwex.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gsoaqcmuh.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gkreaingp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gqoytless.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gipblzmfq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/glopjwziw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/goskjhdzs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfzclgluf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gesxsdvss.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gnamcwern.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/grplpbqrx.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtbjbiscc.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gkhebkrig.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gbnejbpfy.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gfzphateg.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjjzfosvh.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsgrodnxj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/giwlglcap.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/glnduvlya.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gkamayvka.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gjdaxploi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gtwjdunhn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwewdmsmc.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/grzysjawg.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbunliwjg.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guessatth.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gwljciwtw.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gnmmuiymz.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gwnbchuaj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gmqshplgk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gvagrbked.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gekpyqfqi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gtpaebqyb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grlkyabvn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gdqqlefah.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gcktqpbcz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/goteyvqqp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/grcgmnsjn.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gutifsuzp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gwvsugjuz.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfdtwszbo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/guugrwvjk.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gzzxwolkl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ghlofvsyl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gpvlddakp.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gnpopfsba.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gekpwkgln.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gctprikfx.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/ggrlzluoc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gihcqbniz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gaxabvtca.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gpgqagyuc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glesojwmd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gssabqswi.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gdoicsimx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/glhqmzgkc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/giabweyxg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gwvjtawmh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnqrzprpr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtrvxsbfn.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grhwthyfw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gawqpwvwe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmppxoakf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gadgzmdbx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/ghgoxnhbt.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gvzgmjvyk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gsknubjrk.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gllnepnhl.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gleqkhrya.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gaqjujdls.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmrpjbdfx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gisfldmse.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gknodseku.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gjspgjvuu.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/giedbfcsw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/govwyxsdo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gyyfeqhtr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gqgbqsntn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gldevhdaw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gfmzsurpj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdfdhfhlp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gsqdqkwnb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gonjtdzbc.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gsjinxiyo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gwyctuiga.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gadmpbfhc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ggcxlwocj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gawatxobl.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gmdkjneqr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gwdwocrwx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gxofqgngk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gzxgcuetf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gpltvwlsw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/glxzjhoul.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gwhjbqfax.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkrdezbda.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gthjtfegz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gxtksymlu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gzkmwlkhv.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/guibrxtwt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gjgndtrnr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grjcwqsda.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gddvaecyq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbcvolhgv.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gfiuwosid.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gojfcyemf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gpejqwbmi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gahnoqmyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/glunejrfu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/giuajhgfz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gfqnpuriq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gjesustqs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/grccvnbbj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/ggkhfbkao.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfyrelirp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggrurlvyz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdqfrpskc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/glkjfscyh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grdfztoyg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gwwgufhxw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gjpvodznc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guxssvzgs.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/googsfwnn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gzqlyqhoj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbbetvngo.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwljjxjkw.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gudgjqmni.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gkircphnx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gdqlbxauj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/goseydhsa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghmccrcfd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/grutshoum.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gxumvjdbq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gjjqsdhzu.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ggheymbkz.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gdnjvequj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxejqkycv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/grxmypmpc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gjjilsmkc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gbutmmkxy.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/giwpjbqqv.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gkludmrit.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/ghrkgahxw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gblejjesy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gzavrfhqb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gejftzeus.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gtyjmzoll.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gmusxksph.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/ggujlieuf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gmhtuhcef.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gehviyzry.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gqwigpsob.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gjbtgymlo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gfgnojvgf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/ghinhsfag.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/ggroarozh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gzeayyohw.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gvxbbrssd.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/guqwfhcyl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gnqesralh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gxklqauwg.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/glhtsfckl.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsbblrkww.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gwuqujyez.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gqqbsqnug.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gvkhknxyv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/glpzudrfj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/guowwnfbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/geaafzjsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gcltepaej.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gvazmxqmi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gwqdgyhzp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gzwjyrcco.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gwmpkupol.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gqsycmmta.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gzswdruhb.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gplysxrqg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gqqzyqlfl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gugvsrwfn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gtfqcebyk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gjhneldkn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gctiakyos.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/ggfvxvday.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gprievmcu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/glrqzgasi.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/ghyplpcha.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/grjsdofdu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gqmunuiih.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gzmrrjlto.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gaepwcftt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gytoqjrrj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gthnwycaw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/grlvqbgeb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcpkhqnvl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gujbodaop.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gftszwkkp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzpjvelsh.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gnzmtxrjh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gwrxkcxwv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwyufsyxa.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gkifinufs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcckuxdky.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gbeadzokx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gpueyenis.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/geqvmkyuo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gjjouzfnj.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gjgupqeuc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gkfzeelkb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gqeloxmrc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/ggqynqhyu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gasraayjh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gwsovicuq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gzvgytqpo.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gxytrjdex.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/guydpiija.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gfuewezth.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gxoktpnzp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gqakzlmue.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gvlsqxtnm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/glwrscbxh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gaeeostsb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gytlppxvc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gqbycsscq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gvaxzkqre.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdezpqmsn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gidhpwibh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gdoercblp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/guwzvcbip.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/giwpgkqyr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/ggehgxkan.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gmmoqfjya.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gwbyhpsho.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/giirlsjpl.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gjaijeehi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gamohuhaf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gxmcgxnbf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gldwzvxlj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gnxnbsmbe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gxfpyyrah.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/guinwlilo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gkboccvsp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gtfdgybzo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gmyxkmxle.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gtveenybx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gauydzxbj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gwznuxnlh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/grffjjkov.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gobxeqpkr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gruqfdldm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gpxxdcmpk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gggcoglcr.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gedguaeaq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/galuqaqwv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gqscqlkzn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gtcllqscx.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gqticbvpj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gruyhrsmx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gtpepphet.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gnszmbwol.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/guryydfka.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/goffabdwr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gklexwrnj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gnxnjsezz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/govezztoy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gridsgfss.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gsoewjeeo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gusswweza.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gbhhboouz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gcyvzueip.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxyibvfws.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/greckpnde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbdbddslh.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gbycgtnkv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gnjkenxmd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gguvluxvg.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gwvjuessa.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gkimclsph.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gcmihdcdw.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gsonraisd.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gfpvhmxin.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gscawazpl.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gsayaexkc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gofrinvkt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gcedjhukn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gdfkberfw.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gegatizqw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gjfgeapjq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/givtmbhqj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gnbfwcjep.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gxnmfekfw.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/guipjedrt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gjcnsxvsv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gheqawvpr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gykkhbumk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfuzlqkk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gfzgsznxk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/glofeaidu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gfrbvjxlg.sHtML


<!-- 参考信息 -->