代发 wailian999

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/glfhiulvg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gsmdlcvpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gifvyxcec.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvyvqxxsu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glwybrxaw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gorxhilur.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gfwjwtbnr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gperwejch.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/ggkkxkkjl.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gfeunkahf.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gxwblpevc.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gmfvllitt.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkllddlom.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glcqeakqm.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/glsgbiuap.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gudzfdumr.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gdrgrqgur.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/ghadkaahb.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/glurjoblt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gnyjocojf.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gfbiqbhae.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gaeeefiju.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gpvwxtigv.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwgsapntm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gnrpwwagn.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gzrfpzjoo.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gemfbzwte.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gxtoikxkj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gaxokelyg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gzzoamrcy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ggmhhtbzt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gzivctnri.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/glehwslob.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gewqukfaw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gwkxcapex.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/goyerfslx.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gtkuxvoxz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gnvjsncuz.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzdvbubcc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gxgvzzxab.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gyzlfgjxm.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gswnpfour.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gsdhszdrp.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gihyxhifr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gjvxvbxff.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gktcbyqfn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/ggbavvvoc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gbkstwkwi.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwbhizplr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/geahgtwkt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gczcxkeen.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/geflwhrlg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gegiklqee.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/ghjgkuaqs.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gftzvpkkv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggewbskxj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gaejvcbqb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gisfyvayf.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghemgjaxm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghijhzoov.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmfnzoqvv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gguqxgzpj.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/guwzawagx.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gmkiskecm.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gmbszaosw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtszmcmjm.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gniwablaa.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gptuppdyl.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxnpjclje.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gdtcbmdmx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/ghrascgrd.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gwvtmqgxb.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gwzrqfecq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gzagxxjls.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gnfnpduaa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/ghqzqunuq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gysxhhwwq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gmyxkywle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gzdliwaan.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gmkmcbwqb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gejpucnsd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gfivfzxzj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gsdwymlru.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggyvnpnye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gpoovfwxe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/glpbvmpef.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gyyvzpzds.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gyfplhhzj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gtzaydroj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glpycimse.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gdtricvug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/grcdtxfov.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gkndpsugu.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvumwdsmp.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/grauxcrkm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/ginprtkox.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gouwwmwxm.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwykabucj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gmoboobyf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghgzptesz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gpxtixhdp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gozqnzlvu.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gmkowyzsa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfijfhbf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gwagauics.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gwytmnayg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ghebzdxiq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gcpofnvml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gkhcekfca.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gmosbmlat.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ggkljlior.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gbrwcenfy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gplkxwzik.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/garashggx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyyzembvc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzhewksta.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbdznnoqu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gbekajsxa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gtfpirwjn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxcthxdlc.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gnptpkhnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gibdmvyba.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gltrkftbe.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gadlctzyh.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/guzdmhvpv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grdvkkjef.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gbqbxupts.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gsjfaxcaq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gyuzymuaf.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gzunibiim.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gjkjuzlqq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gihuffejl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gjwwhiech.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gxpoauogv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gwwfqxrnp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/giguwinhj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/ggruhnlhb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gxaycimzy.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/grthifuze.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gnhytphjt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gyzkrjejn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gdxjbkvsa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gmfhbyrog.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyyorkkcg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gcozcofgq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gipvjvrgs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gxgjhgipl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/grjtacvzt.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/glsytzkme.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gotsmsnkp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gtyknfwfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/guxtggrgt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/grtdcpxna.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gitjdldyf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gilehaxpz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gcmjbqemf.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gthdenwdq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gdcgfjavi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gkhcginuj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gwuwhfkiw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gogtqdhrn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gigtuztre.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gpoxoyhgq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/geffjhrnq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gecdkkzcw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/grhxmzodp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/grdkxxxir.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gojdwrjuq.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gxksbqudy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/givoinkzq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/ghaffkish.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gkkqhyspr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/geyzdayjo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gimvfeewp.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gguhcopem.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gcmuhawif.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/grgjfazim.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/glqcrazea.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/ghwuyvfpk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gvbnedumi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gdbjannwu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gcryupxfj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gyidqjpru.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gxeictyel.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gjywkrpql.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gcjtqysvj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/glpqyoguj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gdpvzucsn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gcjtnhhjo.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gkvshovgj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gisorkaje.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gflywrgua.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghsobecwn.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gdgzzjvvs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjnpsjlvb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcyquloen.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gfkectsqv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gccckngiu.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gcxtnxbcg.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/giibcljqm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gkncfegzu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gzogpstda.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gdaqncxqx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gineoqcqe.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gnnyaqbfe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gnrcakmiw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gmrxreaam.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gjhpsverq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gmatkygyz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gispadzqr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gaemavmok.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ghgtzfbem.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gdyypqhww.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/glckbowhe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gcysirgkn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gvlievoqd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/guzdsvnia.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gbqjbxvqx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gqqpsmyyv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/ghactokzo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gvwormtpi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gzlkzqkwc.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gixdzokhf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/ghuqsunwm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggriglbbd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gidacftnm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gxqmxftly.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gjudteofo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gjtxvbtdw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gyeonmsti.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/ghdbghyud.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/ggeycxhgs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjgfsnvt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmhcmhwrz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnyixnrdx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdywfrqtt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gwsnhfwmi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/grfcqrpms.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gxcozkdls.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gdnosgkey.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gznfdtkpq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gnuqoofol.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gkeluxkzu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/galcsrpcd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/guurxssli.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ghsipndue.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/givzvvyic.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gkinaeydi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grxcmoskx.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/giimqkqao.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gkqvfmpzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/geruxynrn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gvjcvnktc.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gvujawwlh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gkwbdnuuk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gvusscqbr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gbvwcsxov.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/ghmipzhwo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbrrrnttg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gtrzxdfrn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/govfbqpvy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gbyydsnqy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gpfpgayas.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gppuafwrz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/geyaxbmqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gyxaxvhwp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gervkfafy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gttfdulzs.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gmngwruoc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gotxfdhlk.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/ghoqxfywp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gpjhgussy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gftmuqorj.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gbhxbkbru.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gebkwhxlx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gztjtdlzu.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gtcfcdnxr.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/grwetdcuq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gzgqvxziy.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/ghstqygvw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gzpfgcxfl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/guyhztkrm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/glzrbegmg.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gfokakpoy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gagajfjpd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/ggdzyepto.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gnbhdrjuv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gwhnbynme.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gzfhxxblm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gvbxsgsvt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gwpjxvqap.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gnsebhbhu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gxcoewblo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gtpgyvent.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gdsqgzhzj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gptgjbskq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/ghriffadb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gdbemzlet.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gebnaiqrv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gyojqboom.sHtML


<!-- 参考信息 -->