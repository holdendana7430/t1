代发 wailian999

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzrkbqctp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/goakbtcqr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/geuqlvekv.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gsxnaptdy.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gwfxohpfq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gkqbmvcqd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gunwfvaze.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzvjcsocy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbxvvtfiy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjvkuba.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gbcvxqdtm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gvbjcllwb.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/grvtyrbmk.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/ganbbnrzf.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ghjiuezqy.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gouwsqkkq.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ghulorlaw.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/grhvsjrpm.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gsapjlssu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsekfywkg.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gldpopwvj.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gahchnuxy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/garrfmzcc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gprhpqjmz.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/ghxskiyjn.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gldlatfhr.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gvxbntwgb.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gsvhnogca.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/goanlcnjk.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/goswvjnyj.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gvcuygjuj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gisddtowf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gbernnhek.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/grexmmwov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gqdnpgzyl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gausjkcdh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gstpbqeto.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gxroernom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gkxxdecfs.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/glyjcitod.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/goewkysav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ggqpjygzs.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/grmeselkr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gcqfiiclv.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzgnypsep.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gestaowkd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gwqlttweh.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfbvlibkn.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gnpjhetpz.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gjboxswnf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gtdtwexqt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gfaqnrrtz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gddglweih.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqkzajxdu.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gisdnyvyl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtwbyfuye.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gjocjqubm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/guelznzqf.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gjmzhjsrl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gumowbcqv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdrvejctt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghypovhrj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcnieshgh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/giwysmbvk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ginildlsn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gifrgmajv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gdngfawez.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/goyxjpicm.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gxumavbeo.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcrffchzl.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzpxmhidg.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gwisirwxx.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkbpazday.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gtngffwdm.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gsikejpdu.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gtobykowo.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gfmvagret.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gdtlkkghs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gpsdsntmz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gkfoicips.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gpjtkcfhz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gdcclfijl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/ggqpjlqor.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/greoduaib.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gdyzuywoy.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gbqntcsal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gwpaqapuo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gyqerlzqt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmslrfh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gqxawtxrl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gkejmpeqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gksuozowd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gqdqalyof.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gkncpplfr.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gcchebahq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gaehrxbfa.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gpkqdadys.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmvpuojzv.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gchoxicjq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gaoxtahft.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gjlynxaum.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gsxgywmpp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gexhhvhov.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gffcvisod.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gaecmtnxi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gomorhtmb.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gbcnudymm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gmdpngjas.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/grzjutxgd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gktwilijv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gicelqhyk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gpuubugqr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/geypzvuiu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gfcuanwzr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gpaazytqq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gvnqxfzea.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gfriyjzhc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghyuriqir.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goanpppbv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdpsxnnps.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gwpjhudan.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gsisbtdwr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/grosirlqa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggscdshmp.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gwbjvjwre.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gtdivsmal.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gziqdciuw.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvjfzcdhe.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gfeftpopb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grzbcuptp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gabququmr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gwnarbaol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghpnhyfju.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gswddkaas.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/ghulnaknm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghmuvovbl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gubqomrmn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gsrtuurqv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gnfujoaar.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/goolhjtkp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gokpywjzw.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggobxfsna.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gsnmuiykr.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gnzjdkfbv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gojmpomfu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gftjvtrcx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/geejzideb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gvcjbzobo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gbdksgzkx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gxszjeubz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gpwvxfuso.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gniqsperf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gpbvmqmzw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/guzkxzplm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/ghmgkqvdc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gphoccpwf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gkaftyttb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/glocgbglo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvgzusk.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gprtelimi.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gzwejckbx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/ghnusbyyi.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gidddynmm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gnktbuzog.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ggysbvfzj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gfngmkebm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gejjmytnr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gpgkhpvwa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdxtyztfs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gtfajixjp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gxnniptzi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gpcjgyccw.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gbiqtywwb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/ghbygolib.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/glmwuzmnn.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdpmrsa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gygqtbqpf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gdxhpxlhp.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gdogogovx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/ggecbfbxw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/ggzkmrzrm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gsvvfjnsa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/ggspionnu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/grsefaecn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gaknadeop.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gbkzpoohb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gcsyjrpxw.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gshlazfku.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gomhfjgvg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gocpumkhl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gyphrsebt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/glucughcg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/glittdpqg.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gmwqslanf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlrmqwr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfvlnrznh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gencpsnrd.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gajacwszf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giqhvupbj.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gqhihqdch.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gthrpaskx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gllpjvhsa.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gjitywlhs.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gywtwtwvm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/ghsmzpxse.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gaezyaiww.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gclpcnybb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gxarfmlem.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/geakecnxj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gvcomneix.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gpegroouu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gyjytvyoo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gnypcargz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gbrrxxqlr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/guvzshfde.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkflupdoe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmtezrhry.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gznjssbbr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gfagxohre.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/grlvryivn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gxdjsahhi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gnccfxmpx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gvnpuegzn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gzjwllaob.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gwzopsklk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/goraifjhm.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpgiqwnbl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gowkwftea.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnpntsqlp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/grepwqlsw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gclrdskhq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gpnlxwuwn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gzlulgwof.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/ggzqnrxmi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gljhnbtcb.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gbtkpuxai.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/ghuerhtev.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/guflhhnfd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gdgcskyzx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gpcpadaps.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gvuvohovx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/giuhdndno.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/govkxmlrc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gzpcdwslv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gppphkvfj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gdvtysbmz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gpmfqnmjc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gjuyvajlf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gnuedlunk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gbnvwiund.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gmwovfdqr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gfqsdotqw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ggpysdrqn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gsztpxduk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gyuflcpip.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gsgvzxhcb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/getgtilnq.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gixozchle.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/geedvpfxi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gqjgnmwlc.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/ggebgqunb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gdaypbzqs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gkrwaubdo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/ghcykedio.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gfeazftsa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gbitqozcr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gxikavpti.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/ghcyhbfoy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/guejixqyj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gfxipwxrf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gskbedirq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcwpdrfae.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gjasxnyxb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gycgmvkbm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghxwtfviz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gnycrfodk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gczefktoe.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gpabmfmls.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/grcopfwyj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/grlatsosx.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gdxzosfdv.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/guxkicdfd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gteqlcxzo.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gzvwyakor.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gwnzduxhb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gwtqtkzfv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gsfvwpofa.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gspnnsqfp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gpvwkvirx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gqzeamebd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gqepzleje.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/grnbxneia.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gwfmcefxx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/ghhjwqpsz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gdjtccseo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/guwentqch.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gzpfltuws.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gormelvti.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ghrqetvug.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gmjevxywy.sHtML


<!-- 参考信息 -->