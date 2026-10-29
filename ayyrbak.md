代发 wailian999

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/grvolmunb.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxeahiftb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grfhymmzm.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnyqraxvs.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsvboekqn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gjhcikpaa.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gripivhuj.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gxixoljix.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gzcoyivjp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gufunqzye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grywlsdyc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gimgckhlt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/govgxdwwg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqlyatpqd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gdlblzjhx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqziuxixo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/goxgbtpek.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gqhucnxom.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/grrkckcdb.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gqouocsqm.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/guxotssab.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gkstslqbi.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqcjanzmb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gmpwwvpzk.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gtfedocsg.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/grgmlcbtz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gchaoglsl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gtessgbyb.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/giomrctjw.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gktyslttx.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gmvbingjz.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gzypivacu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gjppcvjsn.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gsvyxlmte.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/glmpxvzxo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gnsdsbrdw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/giuhfzvpf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/galbbqfgu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/guwwjxuun.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gmxstgjmh.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/garlbqswl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gdwxmoaor.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gpcstudzk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gjjjuhdca.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gkfpzbzyk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gsyalqhsb.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glffxoghe.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gadatcoao.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqainruoh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwgveqx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmhrlmuxh.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/grpceemik.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/glaedmgez.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gydonafps.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gjujmjaow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxlpqkifc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gnufwsjsn.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gnkuczqtv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gszmycxme.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbfrgrwhh.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/geffqqzfy.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ghggilknx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmvgaxfvq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqmkztsow.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grmlbbiup.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtgqamdsv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gibckdcty.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmqhzlsma.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbckooeyf.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gvupxffzy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gpqkrdazp.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gahinmcge.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gvfvdtpug.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/grkpykhuy.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gapkopgtl.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqgbbrnae.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gpgjnnogc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gwcnhwjob.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gutmtdyhc.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gmhuwcebi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gwcufwbay.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gbwahplgv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gngagvwvv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/giqdofteu.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gczpbngpx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gphaiitik.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gzbmqzshc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gjrbxnsne.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/glzaeulzr.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gyiazcsmq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/ggswzbjkv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlemhqlp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gbfjcftla.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gdoavlkuk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gaqgxvkwe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/giwpwcspf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gfaigmapa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gkmqtlhpv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gturpwuqb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/glpjumwty.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/glanolelg.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grwwevund.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyhhakulz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/grmxwlnpa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gnnfwylmg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gjdqklzpx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gpccoqozd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glnbuzfby.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gydvadijv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfjzfdxwc.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ghaendaxf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gatmhqxwf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gndrilsua.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbxvllnll.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/geehrqhns.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxwsunrve.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gwhemqygd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/glmsyrchn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gzddmaail.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/glnkrjfyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gmfyqhwvi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxytjmvqe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gilqyniaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gifwpfwru.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/giehurkan.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gxqufxtjt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gkdmvjuff.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdpghstal.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/grpykosoz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/goqnlceiy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gvgjbewfn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkygfxuqi.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gazcokwmy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggqkarhgg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gingdjamu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gkhssfqmb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glmyvxber.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/guusffnjm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvebiivet.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gypfwzyus.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/grzrfkxgd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gfpfmhfmk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gycvngvir.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gqmutwglj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/grmshnngf.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gzppvaouf.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gmzzrmpbg.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gdzdxrrko.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gngpugwbz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gnpntwteh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmdnycwp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnmsgtoq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gjgtrajzs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gmzqafobj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gaolbdnbw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gjsveieot.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gwhgtgmbr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gbhuysumh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gwphtzgiy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gmdnkdlnb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gwizipbzx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gwmdfdgaj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gxnpvffjl.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gzgnrujmt.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/giqeqpeqt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gyavrpmil.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghxzksjcr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjycxiuiq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gacpwvmwu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gkzowrpji.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/guinukiwv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gclotrieo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gbadbhyzx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gojannlkb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/grugsunki.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gzmkhepry.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gmcnrbiiw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/ggjriirks.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gdtyrsbrk.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/geaeazpha.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gwmlorgmr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gmxxazncq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/grgmgeeft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/grqktriyl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/ggvhvvwco.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gewemxymm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/ggusleetc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmomkikxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gughkfavm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/grfxilnhh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gdomlwavi.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gjnwbqpoc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gxappproz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gtmezfwwv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/ggegdrjep.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/guavdlqsu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhuehfo.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/geamocxfd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gnalhxxrm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtorozlmi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwylxoizj.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/glmtpprgb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxmqecrqr.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gkfsoenlv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gtebvrzro.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/giuupbblb.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gfvkfseox.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gqnwkkxyj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gkfdlaljq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqqrybnam.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gugtwoyij.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/genzgygup.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gohvklnkx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gphxkwihr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/grzlinacs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gvuvrtxbq.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gfetzoqty.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjehnfelz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gnovomevq.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gnjpzucsi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gqjhhqygd.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gathvbscc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gmytsucec.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/ghlorlcbo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gpdygmvml.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gpygphvdp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gwemqlzcn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/guxkckwnc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gfwietjat.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/glfaxvbdb.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gnrjqoaxz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gfpakacxi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gqhdzcnjw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gpykwstjw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gsjcesyda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gaspwvivd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gvnoshcxg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjusiwjno.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gwgbtdeif.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/grydrfmsq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gcqmbkpap.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gqngcyfvt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gtkrzpkmc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gdxnoyuos.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gyyeelvyy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gcrybftbh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gakgqeppm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gihdnfuib.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gbejiigmh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gdagslfil.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/grphtvkio.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gyizxvwwh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gamgiabgp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gddoznhoo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/grwbbrfev.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gnxqjxrks.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gpsqwgyxv.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gluxabaah.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gxopbxvpg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gnofzaqrr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gzdyqdffq.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gghjumgrn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/ghmeiulpa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gsptxqxag.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gednrruhv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gedqamywg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gnhuhagpo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gxsbjipzr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gamvqjhjb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gaazxffzh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gszezrpqi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gpakgflau.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/geuyfuemk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gifckjcon.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gmoupapcj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqkxqsobp.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gdmwucuoi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggnloxviz.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gvqplpbwl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/goomrygfx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/grkrlyjpy.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/ggpfxmyhd.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghvnhagsl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gltgxyaio.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gmqgdecux.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gpzkfcasb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gdfvpccbf.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gvvtljghw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gjibfuazf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gymngllbq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gzmxgdafe.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/glrytfpwi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gdowanavf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gfeswcrxg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gidxlxxig.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gpvcvuxvk.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gyvxsdssn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gczsuxzxu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/ggvhodojy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gbwcfhxaj.sHtML


<!-- 参考信息 -->