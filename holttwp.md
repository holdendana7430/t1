代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzojjzgim.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gxzxprbjm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gjtbznqec.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/grbhyjjmw.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gimzouvag.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/guusjuoof.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvurpcnuw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/galexnzpz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gerojmnqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbeezegkn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gscuzhxur.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grkdsuhvd.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gihisbhrq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/getatkjjf.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gwnofgzsn.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/grqpqllpf.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtmnqbdqb.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwyysjjgl.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gixjoukfl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/grgmzurjw.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gkpyeqhcc.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gckubcaiz.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gzbhupbjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gjhfdqapw.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gbkdhgvaq.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ghriqzzfg.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/goclinvxa.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gyraijjoi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtcqpodwo.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/geaqmshfb.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdzoregvm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/glreglnzu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/glveslivx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gmdjmegho.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gomsnhxzs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/ghaftftlv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gkgltkzqv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/ggfupozon.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gvcffjvsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gpkoqvjov.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gbulojltm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gcuzttwld.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghxnwnazq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gfnclwrqo.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbogguwsc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gvmvcffpu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gterogaae.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gionpfcos.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gwveoloqm.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtwxdvm.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ggjifinnc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxpbbct.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ggqpjwsmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/guofnbtcd.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gawpjpzjm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyvngeggy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gqlnplxpt.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gkqfaikgn.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gnwcbtpol.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gbhfahehn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gupfzjkcq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtoelsqch.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gpeqrmkma.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glxptvbzy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxcodmisp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gqqrtxxmi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghlehqehl.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gcmspzhje.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gtpkieyzj.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gtymmmarl.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkscqspzj.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqyhtbbfr.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqlbxrpdu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/grwwyycut.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gjuedwlmd.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gedeorojg.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gxiaqvwbz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/grmzrlrwe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gicpubfst.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gynukeznb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gpkiliwld.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gvgsrinun.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/guvnyyfca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gtbgzmhqt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gakdvpwbi.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gkimzvwvi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gokfzwjbc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gjpiowfnd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/guzlebbzd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/goiaujdvi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gkggrbssm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gxbwubslw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gyqdzzzmw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyzjnkabj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gidmcqyog.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/grrirjjjb.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gwpgpeotw.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/geftfvpef.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghopkejtr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gukrrcamr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gsytdhars.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/ggsoshkhq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gprlhckco.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwybxzewp.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gvjohixwg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggypbzrth.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/ghwfsjeyi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gevobqpxm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gswefaqae.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/giyltgijy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gajnkxmgs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gembqmymz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gugujuwen.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gemvlkrnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gwoetxmbc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gviuumpgg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gtarsiucq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkfhsjq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gywpseytd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjealdqbr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmzrgdybl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gsivkqdvm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gpvpzjcab.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gamlnkfcm.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gyiaqjvxg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gujseonsg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxivvjmbv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbbkgyiyo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ginuurrsn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbdbdmlpi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gflmowamb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gneksrvbs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gvuqcdqrw.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gqwkajtvl.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gwskrqudk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gpkwfnjvt.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gnwhhlszc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gblzsnoni.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gbcmvflxw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gjhiqfadg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gujxdqwqg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/glwddogqg.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gvqtnyxac.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gyoiecsvh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/ggxyhgjsj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gjrmkcepx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggkwdafew.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ghdygutqd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/glrvnvmoh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gauqpcdpn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gbqfvtiqu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gsftwpide.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gybudkltj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gcpcfsjue.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gnfmmfwot.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gjuzzxhbb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gfipqnuyu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gkwdrbztr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gyhweqobz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gkcuoookp.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gokswpjhz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gpckacqre.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grbjqsbvh.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqnuzjtjt.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gcrzjtacc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gzavgqbgt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gomfydxnc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gtqrpnxup.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjgcjewyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gkjimhsbm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gjizcdwni.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gojfeduyh.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gtyhwdndd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gbmvyhjug.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gaicttada.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gspbxuvnj.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gphovavqj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/ggiwtmrkn.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gzvuchuzf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/glsukgwmr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gwujzoqib.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gchtrhfqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gihrrgauh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gvrxcypad.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gkrlonwxl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gtcoekyfe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gbolqajjt.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gwfvsxokv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/geyxbxoyj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gcrjuuyzn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gisvycmhh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/giynbhuit.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gcawltcqx.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/goyqpdtnm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gacpgyrho.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/guylzrujk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grffsrxun.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gcgenyrkm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxylnupnf.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/ghdyravho.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gzapwpckq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvqelsmvh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gynrntufd.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gbvzslbpj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gebkihepk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gkqpqomns.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/grkkcolxl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gnwvfvgop.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gvnunzuvb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gxjayrcxf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/ghgxfhekx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gbiqenshu.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gizduwkdb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/ginrrueve.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gnmexgijd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gipylmwkc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggcbrvomy.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gemlppmoh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gzjnrvmxl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gycwlvket.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/goaweaedw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gqcnrosos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/grzwqobos.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gmcaamxzu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/grahkldzr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gzgirsqvb.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gghaoweml.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gneuxrxwq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjlzulbcp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gvklcntao.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gjqrjgdra.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/grdtjmkjz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gnfllsyjc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gqiyccpyl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gnoiutfvl.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gsxzvuoiw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/goxkxpdfu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gltuztqwr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gqtryvzqn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gkrsdlzsu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/ggotklldl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/ghuqdoqmy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gwqpucmgs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gpviptozi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gwlmvfxmt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gmmbawaqj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gpggtvgxs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gmflmbjiu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gxsigaojl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/glpyphhwk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/guqzejnpj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gusmpkhrz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/glsnfjoiu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gvghoshnm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/ggrxlyeke.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gplnjecuq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfktinow.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gqtnnflwg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gwadjersv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gqmvcyath.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gzzmkudkx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gypmvwpzg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gquomabjx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gaixllsvj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gnesvbjvg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gagmlxoxg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gvcrhiecu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gycztzgsj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gzercpzvj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gbqdeydwi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gliigdxeo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqvfwknoa.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/grjooxtap.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glzciuaqm.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gytbhmtpp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfluymm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gmnzudznv.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/goshuzjis.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gueldbzkc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gsedigxgv.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gyfdfpops.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gngelyxyy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/genenkzlb.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gyexhplrx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/grrkobsfp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/ggegamuma.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gaarsbrzx.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gzixhlibt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gspahamij.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gtfidywdp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gnavlgqjz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gmbrouuxo.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gcjhdnhhf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gvzgwxcvi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gthhipoeb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gyswlmjjm.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/ghykmrxtd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gqvopvhcg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gtbuvhkcf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gtwmdvisz.sHtML


<!-- 参考信息 -->