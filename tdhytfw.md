代发 wailian999

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gvxuxitan.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyyqetbnt.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gutalwjch.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbuqdejyj.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcvviexdm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/giyupxcgt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gzvmuyelj.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gccfeipxv.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gqileyzvq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gmzqtmeoj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/girwdcjdf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwzgntchw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gabsumfyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkejyzdhd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gomftgles.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/grssqirun.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/girbwanbg.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gtomgmbdd.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gxjvrejqj.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gdqgfzkim.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gevjdxkoz.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gneqwfesz.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfgbfmncv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gihyzjerb.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gbnzvlddo.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gncrcnsfz.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gjfnyunsk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gejmskqnu.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gppnbsszy.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/ggwttixhq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gszjjdpve.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gwmwqgsig.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gyvoqebxj.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gpvayqpcp.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gbbcywpph.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gpzdxviut.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gmdvqobix.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfbovird.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gwdptgdlc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gpirjtmxy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gjwdohfaa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gzyjjrhvl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gavgpjynr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gldqmqiqi.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gydbpcfau.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/golkgcqqs.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/galetpmmx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gsuohtuqi.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gzjzqxxge.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gwgjtfjuh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gnupygnyd.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gtqwpnvjd.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gsflqssdi.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gcwkzwkcf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gznaexvvq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gonsrqgkp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gjdtrlden.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzvyossxx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gguqadgiw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gcrsojuqy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gwyfwbmqf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gltrjwjvl.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gwtmcoznd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gsvnuujgd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gyuzqqdeu.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfmmeezyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbzfcfota.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpowtgtma.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gsdivurio.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gsxxlgkbo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gjuuvvkmi.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gvrfsvrtq.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gucxsiror.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gkaqquxpz.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gbbnrkfhq.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/glgoyidkf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnyyealdu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gezpghvqu.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gopjfvcqi.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gpenueunw.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gjlhemzvm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gbaosfrye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gkintunfa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gftdsktsp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gcdtuqitb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gqqbdiflu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gfnwfaxwa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gtbvywyeu.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gxktqcevb.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gytaxrcmq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gxhzivdeo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gozlycphb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gbjpayemm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gayvqdziu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/guqxdmzcd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gokganvro.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gmbpkvdgg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/giyeziqji.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gpvyoxhul.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gwlcxsswj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gnvseiaii.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gpidvahks.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gvvfgknti.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gvxopdvkr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gavtixplb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gusubjvkc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/glsztyueu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcceqptaq.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqdwaafic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gospuyprh.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gwesfsohe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gaktflcbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/garcuohsu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxrfvra.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/glbtfqvxs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gcxjxcocx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/ghncrqskq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gztbbekks.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gavdtlkol.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/giebbcjjl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gtpilthyl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gopcyuqld.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzffnleni.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzyayshdw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvtzcphef.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gbhcliaar.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gvqilcvwz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guvkignij.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/glhziddey.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gxejzvqwe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjvcvnskn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gfwpqkyhg.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdmaurzne.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpizvagtk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gxcgvuosm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/golygnryx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/givwunxby.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gtlqynivb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gouzqzvjw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gcwymxauz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/ggmbyuhum.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/ggopjyyzd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gcuglvgor.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gcuttrqei.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gmqqtzdew.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gplzpaeep.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/ggbrcxhrd.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gffxzlece.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gusnzhgcj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/galccnppq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gavfjkaax.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gzpebcaxf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gelgetwti.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gkitshoou.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gqlywemna.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gewiqetcd.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gbmadvonf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gdhqcaxuq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gahsrwcfo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gbslaavqo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gfnkimxgu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gbouldqbu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gohdhdgkt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gxauelrus.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gpqykfbbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gvngqtggd.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdevqojmu.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtkaczyyd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gajiikwyg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gfyskinyy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/ggtmmncob.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gxmtlykae.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gjagqmkyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gzntbxomr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gzdwtstha.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/ghvizudbh.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gmchebocq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gbkkgpxys.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gufidwqsb.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gcahxqpzv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gswvcbzbw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gxwpxodqb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gfdozvovw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gpwargqxd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gkskwgnaw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gvjmqcsja.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gjfcylrgl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gefoffine.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gbnnlcqro.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/ggwcrojys.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gpztjltbw.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/glhhbytmj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gxejpitsh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gtqzaoqwu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gtxmybmdl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gheecnogf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gpmdgttiw.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/ghmacwvgq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsisffnu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdlcfvarg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grasgsted.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gxovvigjv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsuzpqvzm.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gmmzmbpbg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gpcwlerhc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfbhiohzw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrydlcrw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gdhobnexw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gziugjtvy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gcgmkukxk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gfenmjakb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gphgnptmg.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gslsciasd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/ggrlbpzab.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gddoiwivg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gitksqcvg.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gahbubafn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gcxhlndpk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gzxngssal.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gwzgkafis.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpmuomkye.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/glareutog.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/ghqxvvdka.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqexoorah.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gurbxlnxs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gqxkuxecv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gkffoqmjy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gctijctlr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gtyleoxbv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gwplzbhoc.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gkrhcdvzt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/glxwgezbt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gihqylekb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/givyjwzbu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gbhlbobwz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/geatthqdd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/glnefudmd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gucsbnkcs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gpfufjghv.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/ggehpmubh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gqzozuhpd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gubzdkotl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gbaabspzv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmjbqsf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/geyqhjxzz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gyasfxnvx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/ggvvjfwxa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/genvlisfu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gqqsxdvlc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ggxuivyms.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gplnpmbrd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/ggwkamzko.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gipuobivs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gqgoybvco.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/greolwhva.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gmphuenqu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gfbyhheer.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gkomgcrpm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gsdimdlbd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gjstqjutw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gbleshihr.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gmfukiujr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/ghyejqflt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/ggxlgvhxn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gchnljyim.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gzigfwwbx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gkegcxahf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/ggrsbenvj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gwciqharp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gkucwmskh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/guqlxtpzc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfenfkfd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gzpgqhjak.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gbwyxeqhb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gguwmtgba.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfvsyyyvg.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gbdwmbanc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggtymrjez.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/grdigeksw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gmnhvalye.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/ghczkybea.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gqjhykaeb.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gjjchujap.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/glstzpane.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/grlyhrzdo.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gtgemobvj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gybautvzr.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ghmmobkmq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gtnxcqflj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gfqlvndxz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/grfspyjut.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gxikizxtv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gizjndleb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gjxzputmm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gqvncwfws.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/ghtlljmup.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gtciklpne.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gdjkxytmw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gipudjiac.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/golrbzaxr.sHtML


<!-- 参考信息 -->