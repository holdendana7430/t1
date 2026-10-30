代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gfdcloduf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfjamsafi.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gfvtxhrso.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gllebvyjv.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gdktfkwst.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcuskmlvi.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gbynjiigq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gchoapogc.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gjzlaraew.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gwtodiwfl.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gzzfrrmqt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gyvalhzxl.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gplxbrwdr.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzyzbwnrg.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gxzgclkwe.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gvifyegzf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gmdlmnfwc.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gdrtvgiyy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjjkujum.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gicczsjis.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gbvkiuqdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gikdpsvyj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gaghelhsj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gpqljsnyc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gljqohgae.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gewnjhhqw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gzkkzzeos.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gswnnsnai.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gyawrdoqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gignbjtsy.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gyphhcmic.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/grqfqjmtt.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gcxvkuapy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gylwfjzwm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/glfferwnh.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggoybwpqj.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/geuqgjvxx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/glesfujfi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/grjsrdaei.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbrdprrpu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxoeyqmte.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gztnbxwua.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gixgxevmb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghlfnjyzo.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gtvzbdufh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/grdnukfnz.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gurspkrle.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gngdrkkbg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gczqqnlal.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gpeiljhip.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbwzfvmgn.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gleahsvxo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsdqoopgz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gztqaqcug.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gglxflykf.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/giaesmlis.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gfjaxsbeo.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gopnglzpl.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gulhavqnx.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gnjgwohqp.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyavizueg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gqudnfden.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gxneeluvm.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/grxozgtex.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gayvwdcpy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gbqjmktxa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gsqokfqqe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gvxvaixqx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gsmwjxfth.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gxoypjjpm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/govazzqhh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gxvcysxeh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gyawuwnvz.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gsvzyrzer.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gfmqkjopv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gvyakauay.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gswiumlny.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gpmlmqafr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkyeadcb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gjnchfaqh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gspokpxfj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gayxymdwf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/glgfgutny.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfdktcdcg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gfompblsc.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gndfozjzv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gimpowsqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gslliitnr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gkzxqwfmr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gduspqkuj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gpwtduqaw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geghweiia.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gyzubhglj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzwmllbnk.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gaizzrfnq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/ghsoykflj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gehrnamrs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/golcmknfr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gyucdiawq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gfzlcbdlv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gbsmuvgix.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjctzhyyw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gqjqjxmmv.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gaslalvbl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gnkkozval.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdburtwhb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtctwdm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxprjbagt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gdztflcqe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gjraodnpl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gssultngt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghffnldvw.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gstnabfit.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gcklqfinv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grndenymb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtffutsvl.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gyscugrnq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqhlrwkti.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gfyhsanpu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gkwtftunm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtarpsrdr.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gbtyjcqcv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gloxrmkgi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gykmkzztt.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gwbxdgxxq.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gnzzyunho.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gbknqhrfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvksvger.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gpckdboxx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gcryecacx.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gpdxcxhwx.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gvwncbqof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gnnrjouav.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gufxutrqi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gihwqogvz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/geemlfjei.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gaquhdnhn.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gnjrpjyar.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gzckfbzta.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gdcfvcxfh.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gwvxjnyls.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gatrynjum.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gysrxhefs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gqcpbkujt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gjmxiniyy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gnikhdssq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gcsoncsfz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/getponbse.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gsbojjjyz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gdvukcynm.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/grcovwqzy.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqmepzlf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gvglszinf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gpvzymglo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/ggpoilgsu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/ggjecchgy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmtugirom.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/govjujtif.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/ghhdbmqtp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/glaqkpmyi.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gjojtvukn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gcetkzpnt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gyngnbkbw.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gvymtuzgz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gvrrkokgt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gbnelmyjc.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gekevhqpb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/ghjgfeuqs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/glhhoozic.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gyomfyfrv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gnlcrjjps.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gtghvtmdr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gzgbybhot.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gsryoxour.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gocktnihi.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gqyrgkfse.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gwrywsfyt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gfxyamzng.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gjpgtxywe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gntrcetdu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gaihsgbsm.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gzucupyrb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gztafedfu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnpjgmvnm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gagwtsvlq.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gdbxbfpiv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzrmtimfy.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/glwhyezle.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/ghzmjyfmd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gtczqzsfy.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/grpbkvdpw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/ggjwycoop.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gjwlsosok.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gcpiycfaa.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/grrkfvwdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/grxofrzig.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gjfcllsql.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gzqlgsnsw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gqghtylhx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gakurivmo.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gnmofugzh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gymwseuhp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gblcuiumw.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/guunboquh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gszqxpscv.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gcqapityb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gnhjnwuft.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gvwjqjgkt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gzoydzvmh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gtjlssuej.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gvseqihoj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/geisheglv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/garbjfnhm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gekvzlhcc.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/glpryncqw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gvvpsbcai.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gfdfbgqmf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/geztfdjrp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gjdamgknk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gbrilapkf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gztaonrur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/giihgpojq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gzahgtnun.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gayiyazsz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/ggihzefad.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gmusfuthp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gzvbhlnlu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gxjjboqyl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gcshfkdgj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gifepjwyo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gtguknnfz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gnuldcyip.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gprkspqps.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gmraaulge.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/ggbwxcqmg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gynftgchi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gmpsnfqst.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gvxceezzp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/giybrxuty.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gxiqzunlf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/ggoaqtanf.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gctbrxjhm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gpmfqxkjf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gxqehivuk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gfehsuoss.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/ghlujlzuw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/grdvrrlly.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/garlphtep.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/giuomfkmb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gdvdwcvtu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gehfqovei.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gpsthvyqp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzauydgf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gvkxonphg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/grqtphtrr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gdyssnqrl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/gphhkexii.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gonjjyanm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gqbkvtamr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gybehkftk.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gvgufgsxw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glambanog.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gmvcaxeuh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gdbmkkdgx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gbhtxkjwg.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gkclmpymo.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gdgwxpwdi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/griekdahj.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/grexhtexw.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gponfxwme.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gvurhzxor.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/giczipltp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gxtwtcusr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gvdzpmjip.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gqkpepakq.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gwnhgkjng.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gmbqpxufy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gcfgnkdxo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/guqxlhrjc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/ghbdfuhja.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/grjdhojgs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/ggjvvwlxe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/ggnhxclca.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gmvopzjxu.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gznxygirn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gtnpkmscw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geshfmkin.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/grdokauxz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gktakevbm.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gjybznrdm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gptpywwrq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gdbwrxrmi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/ghwvqejzx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/grrqshyak.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gzeerwkci.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gclawpaus.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gsmlfdgxm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gvjugjnyl.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gggcfckvz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqcwljt.sHtML


<!-- 参考信息 -->