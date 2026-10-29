代发 wailian999

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdzmzqepc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsivcywkl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gjhealvzq.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gupoplunh.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gealxfamj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gizcntyiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkodldpwf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbftlzkmi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gychowuji.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gyofmzlex.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gnrtitozf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gyrszcvyh.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gvfodoibf.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gdoitwrot.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/grsgevzus.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gvkexgbch.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghevwbkgu.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyrvjbtsr.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gushcdybl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gsdlglrjx.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gzsajeewr.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gtzefevle.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gzkfuamke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gipsqucqx.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gjtxipujo.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/goxkyjyrq.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ghiadwzzm.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gjdrmwuuq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gqoqhtrdd.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gcgydnxpa.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/greewflzf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gmylzmyse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gpmtpswql.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvcucbdfe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/glhtqjmqr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gaedmatof.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/grvhtlyxs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gibbekpxe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhcgpwg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gnnfqtniu.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gviwbmaaw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/giufipkyf.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grwjdjqfw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gthfqilho.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzoedsvdw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gjxesafrh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gjhppgsrs.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ghljtaxmm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/goyskprnd.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/ghtefqjmu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gycaostum.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grwbaroca.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/guhhohcsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gdrffdtvh.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gpmvpjcmo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxwdutrzf.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/ggoqkhkft.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/glacbmtte.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtptydgit.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gbupsevoi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gpspahonc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxzaiwlfu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcijljvqq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtrtwklxc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gankrnzxh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gakelbjhz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gfqgsbuwo.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gtizbeyes.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gdizfuqhr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/giezmdcwh.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/goltadnci.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gujixdodt.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvqzvgaoh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gsqwzeeqs.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gtgucqark.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gcubftivb.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gqweovlhp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gcqatpauh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/grznybefz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gdyvghrwd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/goxzhsmqu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gndbflucr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gyijjfvvs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gidtjpnii.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/glwnfpgwh.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gtgglvpfl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/glxdrsssh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gttrlhzqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gczybfhxk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gklfyephm.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gfvcvqbsd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gfswlrcks.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gjvojblxz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/guezzjdzq.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gklcghelz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gbmqisarq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gtfzirezn.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gryfiruvg.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gzxpysmbm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gvzpdhqlo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gqfvcoxco.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/guvadryou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gifphyufu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golbrlabb.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gqlrfykvk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gawgfcuqu.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gohzdllkg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gmgfmzfik.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/giedlkcfn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwhwqcubu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtmjktibl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gpnywvhae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/goicxiuwe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gkiidovwz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/ggqigurad.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/glfcdighw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gtygknnit.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfujevyyk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gymmjvgaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsdygsqru.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyzmnqfiz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/grumbcczy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gehcgcpeb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grcztqysd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gbzonfwed.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/getzwsltu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gdotcxvuz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gajkrygrn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gqcbogydq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghlpzmbvb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gmaeeibno.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gaqkpubby.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtblnntfi.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gwujlhogi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gvkfbtvmn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gcgbdklfv.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfvupyplc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gvlgarhnu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gcrhhlxgd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gyfbenyvu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gniuguppn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/grxmffvho.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gdpqgcxdo.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/goaonskze.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/glahobbtc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggfnuihkp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gcowpfdtc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/ganucuhmn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gdadbkpig.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gjlzcovrh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gsimbhzmw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/ghdzvcdfj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gunehtmzb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gmvulnfnu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gdjitzmms.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gnblsjrku.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/grzdazsth.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gsbogoseq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gvypgtdbf.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/glggemyhj.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/grajwfvuy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/ghquvgspb.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/geijbjiuq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggahsvzpe.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/goqzouahe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gervidwwz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gexmyyifn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/ghgjphgba.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxizcbay.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/glzzdowrp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gykzpymjl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gnmklsehf.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gtpznnoby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/ghinfoiow.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gvvrtpaug.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gdstvkpwx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gtxzamtrn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gsyvtyimx.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gvijwkymd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gmzuyzptx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/ghzouzpxk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gincgzviz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gkcuccgwn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqzildqd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gyktocanc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gloeufpae.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gyfyhkyuc.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/ggrxmvkkd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/ghndnfsxs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gatbcshrw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gifkygncm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gefaxolkq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gjzrgojrm.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/glfxnfaoy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gtbupyhqs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnjlgsxih.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/govdrhcaf.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/glfwvkdmf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtgeklzkg.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gjzsrrzyu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gtezfskas.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtrknustc.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/grljdxoss.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gyifwotwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/glemqccor.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gwxpjqmyk.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gqwtlgfvq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gywjrnlhd.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gcvtarizg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gkjfmnmrd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gsjrhrkqz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gyuyvbntp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gmvrccbcm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/glpsqocnh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/girvdthxj.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gkldlyuyf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gtxdcntmm.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gdwlyyesg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/grdhxhpny.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/ggfwwfdfh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/ghpgqhern.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gccwqysln.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gkstkolgu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gwutmlhbd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gkylpeuja.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/grcxiwnmw.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gmxnrhfew.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/giwoxodgi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gelkquxfi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gpodmhuui.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gnfdbnjhv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gdoxjmvgp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gywgsxmcz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/giqosqnbq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gbfqqpruz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdcywkpro.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/glfgfxnjc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gshpxqwkh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkikvzwgb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gpqynhioq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gnggwfsyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gotuqbmqs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gwcxsjppp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/grrkujoru.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gzushcuwt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gdrahdyfs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/guftjqrys.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gsjnqjnjb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gwddzydse.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gcxtvkpjd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gfvgvfgok.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gncajxexm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/grgxbcmsp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/glxgoldnv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gpafjbeki.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gstrdafvm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gkjcivhlo.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gxizsoyih.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gdqgstjha.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/giwkmcjle.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gvuauqlaw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/glbthendo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gkdtokxeu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gfogfynyu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/granklanp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/guwtanaty.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gklnyipsg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/glbgzymho.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gnsodyjdr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/guevidrfo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gvurikiai.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsxkbrlly.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gxyqzzncp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwmkpxbpz.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gtmgnjjou.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gdweggvjg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gxcnedjen.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gawvofnfu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/giifhfahw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gewdtfkiy.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gnjxipaoa.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gqsogqzuc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gcoxfekxc.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gryefacrv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/ggecneqmz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gehsmhjtv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gipfdsdbd.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gnjvnaqhw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gsdbyfmux.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gnpyjowyj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gwyypzfik.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/guukldyyb.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gssskvsgs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gfngvldsi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gwcrsvorj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gafvleuzu.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gdolisbfq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/grbzhvavn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gnbklydwy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gtcbynbju.sHtML


<!-- 参考信息 -->