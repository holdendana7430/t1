代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/grxdvszwa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gcmylzvcm.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gjbkifzzv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/grxgnrwuv.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdfhqeuun.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/getddhfpp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gxnznmnru.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glyjwoakq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gcywuojgb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gptoinivx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gleuhbuwz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gkjmlvoyl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gzxenrzlj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gvcqqmdwq.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gqubqdzjn.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gdvsjvlhf.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtucfoeyx.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxiopksmq.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfdiauyrq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gpgfeiqcz.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gtjdhwfuz.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/ghxrdxygl.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ghnsaapbj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gqssompok.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpvkelqbl.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gucrcpaby.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gmdiqzzyq.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/grnzgwduc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gnfotwryl.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gfofqwdzj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvjrswwho.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gqvkyeggh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gbgvavkxg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gmuemglcp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gtyggkiqw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gqhcsacbd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gtfcxtclm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/grxwbnfgo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gvtdisyck.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gvoiuitga.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gynihggpp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gwgbiumik.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giehfuofx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gxricesoe.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gsopxagur.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gxcwwarus.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gybrjlxbj.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gcuzqunmz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gkteqrpnj.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gkfjpkkue.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gdqrzrrny.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/glpjwxaou.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ghbvbaqww.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/ggwkyyzqo.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfhtomgfc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gpvhewzcl.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/ghdtexhfp.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gjktupptn.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gdcanwnik.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ggfikilcb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gujgdgnda.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gqzotvdrw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gahrcegkz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gdrlxkuzo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/giykyuhnp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gphxgomqp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gbquywymk.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwplfuhjq.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gyepfcceh.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnithbsxk.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdmhgyjyn.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gjwqxvjpq.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfpkmtz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gicqwqqro.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gogublaqm.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gtfeqfjcp.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/glgejjgxu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gmwkhgffk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gavztbghe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gnhzzrzsu.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gwycfmjll.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gtoctjrax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gkyeleaip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gfoottzew.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gyieuwafd.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gdrfgmclt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gryaknbta.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gtkttjdbq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gkvheywzc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gnvkqqbjh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gqrdqypgp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gqjhhmodv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/grfemorqw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gvihtnius.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gazdrvlvh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gdgnudfsu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gqvhnmvmx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grjxexxak.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxppvagqq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gssfzsbiv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ggnbvnqlt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/grfgdmypr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gcwawrwrq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwhsqpwse.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/geqogospc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtapeakag.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gqldvdbxi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gvfgyljmh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gkoybyryi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gezszjacu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/ghskuxlxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gcblwxgiu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/guzczvlto.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/glikszmwv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gokdmxair.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gfudetbwe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/ggnedzxdm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdpyenwjk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gimsuojix.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzgnjexnm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gguxdoijb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmcofwcoo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gubtnomgr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpjdulmze.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gguibcwog.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gvyfgaqmb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ghruyteey.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gpeatdtqu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gokznlknd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggdwjzuvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/goynhewjt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gyzjadcka.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gwvbzbkuh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gbyzrgvhv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gnaighzpb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gdlhewklx.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gvizumlsa.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/grncxedun.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gkqyxgguj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gvktofxaz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gurogweni.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gilzxdtjx.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gdlivijqn.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gannsqqkw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxxenljwp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/galkywctq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gevddsagv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gfcnpbfec.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gvyxvmlzo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ggyazdlel.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gprmbuqdd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gkzjcwbsy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/ggwxioekq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gkklnowna.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gjrhlqhsz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtoufxnuv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/ggmhuxblk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gfiskudht.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/ggnfdgvys.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/grulbxjwf.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gjhnusqou.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/ggtxcbphs.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkztqwwbu.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gynrxndsp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/grqacbmly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gbpolzvcn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gewlykncu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gzklcbbei.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gsiinbzqv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/glrmkhqar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gwxisowar.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gljumdewf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gwrvhehrc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gllvvglip.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gdkefcazi.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gjjjfrkku.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/ghewrimdb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gtylayuru.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gooitczxq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gqbxuzopw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gakabwnor.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gxbfqxllm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gofjxgpjm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gdinwlwhh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/ggczpdoot.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gaaughabs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gozwsocek.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gzdrqifef.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gripxtfis.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/guulglgxx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gdfjhtrgn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gtqmrsaus.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/godwifljt.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gkkylfamt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gbqdtgnye.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbymdxfnm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gassnuqgr.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gosgzydko.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goukakyrv.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gjptdqsmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gfsjwgets.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gnlwvyjaj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gdxwtrilb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gufghtsuk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gcextjqcz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grfegufvz.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gevdrbwrj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gdaecsqaw.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gsxqurpqn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gtykxjqqh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/glkasxnhj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gyzwsbusw.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gyhrwubxh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/ghkfsfnss.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gsvtidkme.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gjrwumkyg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/guidkpese.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gdfgnmsuo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhgweom.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gfprsyeri.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/geqrbqsrr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gkiekzfmz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/grkgmwsaj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gykuhfybi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gkpjydcfj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/grhwzxflt.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gbhggaqel.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gkcnqstpu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gvbvglunr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gwcnnxoai.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gggbkeafv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gawiczwcr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/grsunzgal.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/geyjwkhqd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/getqebyhm.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gpurpcezq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gqbhigkne.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwtlkglgu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ghzdentks.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gmkrertpb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gwzztjxmc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gwujkgwaz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gxtiipwfx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/goaeopbvg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/ghhcqjvrk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gqwqpaxrq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gesetzwsv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gqwldqdxn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gkkpckvxe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/guuqpzdpe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gvxvqeqea.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gctyshzce.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gpgrdznwc.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/grroxfssf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gcxtbliuf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gwukjhwek.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/grthjrfdb.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gxoxmpxdy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/ghbfhiksj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gnzonjxsu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gqcdabnjx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gjiixvyqi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/goditqdqd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gchqnyduy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gjolcviar.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gopqgjfsv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gezutqcef.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gyhxammzt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gebeostnk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gtctzdsth.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gmsrebrih.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfcyqlfed.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gqwlewyqf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gubvzefyz.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gkggrfxsj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gjoymqvkw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gpsocgtlo.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gczysgzos.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gopzonlyf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/ggdrtjtpi.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gvcrduaki.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gpsgmfzwi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gjrsxfkmi.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gmidixkdg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gojjgvkze.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gybqllvns.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gimxrfdcd.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gyrbjtwjj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gpnrezrup.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gnlgiimct.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gneydhhjx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gutlgmxcs.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gmbsbnidm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gcmecesfj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gqdcslfce.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/goyzuxbzz.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gmsuwfgvc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gbyqrryay.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gwjprbpnb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gotlfxczm.sHtML


<!-- 参考信息 -->