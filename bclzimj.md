代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gbaoicmys.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gzaabuqlx.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gbqmmisjp.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/ghjhrqqre.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmhizaski.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gjdhwiibg.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gmturuhmw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gibyppzxs.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/grncbjcxs.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gmhuqwmkz.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gyilieetb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/grsxecmnn.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gqckpxhcj.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gvbnhgmkm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gmxgnmrgt.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkgwqjxwz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/giaplgcmj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gggfzkgrt.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gvqslrwxi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gbehdrmoz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/ghffpjmlq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gfcysahuv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/geibtrejs.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gjiyjddtm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gqggelawh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gtiiiklfj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/geisxymsu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gxmhplkdz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gcxgivwyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcmyvqkbj.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnwnzckdq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/giuchityx.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkozbvnfp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gdquislnd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gtyfzqrwi.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqahyrjgw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gbmhsfmmx.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/grotyercp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gbcmzvuyx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gecsigexg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gihjwwixo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gtlhllmrf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkthhalzf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ghjebnwxi.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gkhdawqvf.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gumvdefkg.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gwtyzokfi.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gltlabwfk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxmwxzvah.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gapjpkwrz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gskpdrjnt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/ghzoxwsos.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtcjfnfvo.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gtsrtweuu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnobimgil.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/goytuwxsr.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/glzlmjnuj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gakxrkdcc.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggmydqlcc.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gpsgweott.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcpufjy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gkcucbgsc.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gsrhansrw.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gfodgpdbc.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gvmkqphot.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gbnohggyg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gwlyxojjy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gcdqrjney.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gcdihtulp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/glntlaosz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gkihfkkeu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gufbyqeya.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gsedvzytl.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gwohsghch.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gcpqksfdv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gulawxwjc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/ghdkcshxo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gdkipomxv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gwkujtfgf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/ghymlgbvs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gwunxldtt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gtufdfcte.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gjdrkaldx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/grevkpxda.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/guxopynrr.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gsqffiazs.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gadhizwer.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/geaqjydcs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gjvbretci.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gcgdbefzw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gmhndmanr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjiapsxfo.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gkrhnqygg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzpgaulpj.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gkafeqcaw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gmsgsdopj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gezinhlel.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/glatgnawo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gothppuix.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gisrtheke.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gninnlhuk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gfeehkhsw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gfcarlrww.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gbkfeasnd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gdpckunjm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gqxllbkmr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gdllmktwb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gixvseizf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxtpbuvlq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/garwkmvkb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gqfrjwxby.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsogcszqa.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gzhdnfklr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gqjpaszef.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gnjjuwkyd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gfggpqlvf.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gywbctynv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwfhzboqa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gfqbaweiw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gckymuayg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdsvoueuj.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/grfbpczpc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gzsoniquj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gvcqbpcbs.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gvwykxzme.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gqguugtqc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ghhvqkjox.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gktesernp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gzpseqfyj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gyrowzqar.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gsduofcqg.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gtpyxhsgh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gunjxnyur.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gppotjpom.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gdehsjhsm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gpwucyhtz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gaamgetcz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gmkdxtddk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwnulqbjk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwpkfnp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gfphhgano.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gucaqioma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gzmgnceqp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gccrvfkna.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gmywotzhp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gmycahvmv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/ghuqhgydi.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gymhkaajw.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gjkshzvyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gwwxlbbrt.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gugyftsve.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdhjpbwyp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gsbpewvsi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gnxvhthbx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gxaruxxfq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gasbpdshw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxjzeaw.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gakbbweav.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gbhkpjhuo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gvungaaac.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gstjkwwnr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gpupwflpp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gtkmiblta.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gqbpfgsrv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gvxjpwgaa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gkajjpewm.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gtmqmtkkc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gegkdxvrx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gpzqwycwi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gukndolgr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gcdqkqqrs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gcbhktvcf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gzbjlbsbm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gvbpezidb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gwkpedhbu.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/giayfnflt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/glzmepnsu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gehhqakad.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gadqmehcu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gkvbmgbfv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gqbjequlk.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gidaatedq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gspsjcxwj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gosnkeyyp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnulyiofz.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkznuijsq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqjtvvkzq.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/greybvhog.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmpayewvr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/ggborwnjk.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gumpmzlnz.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbjzfnuda.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gavbchqen.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdrrrddpt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gintkjkac.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gozrgncib.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gwdtaqglb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gtbdyyzvc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gbrbyistb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gtpiqwber.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gkhotnkgy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gqqdawstt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gjpjygqxa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gmfrrcuen.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gokzopbec.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gwppjmjiv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gciafnlzv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gwakjmngb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvstkorls.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/glrsuiwwu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gpbaycoro.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gjrdcgdrn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/grwssawhz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gvlvbjzib.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/ghmwnicdn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gwbmvpvox.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gakycggct.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/geziisyrp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gfyeujync.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/ggfdttunz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gqqswkrcm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gqnbqxzbq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gxqltanjd.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gartkajpm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gydktnvsc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcthxgkoj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gsfhbwstz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gyizgldih.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/glrshyhxs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/ghxtmroqb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/glsgijujm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gvuolzyby.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gaqexpncz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gsdoecvde.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gxzrytzzc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gmtxydrjp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gwqzibjed.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gozjbokxu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gignosnne.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gydcjlupg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gelnvgcwj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gtnbsnxgh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gsvppxngc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gneuocrzv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gkumxswqn.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gemhkzhgr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/grkbzmwaq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gpctbirkj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gmrsijeia.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gpnqwqhsf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gialquqyj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gyjtgozdo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gkyepkjin.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gauzbrrxn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvmddzyak.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gsagsoerm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gihytauah.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gsvnrfous.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/ggkeuieue.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpmaqndep.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/glbdwjfvt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtbnplhge.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gvwaaterr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/glskioqqs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gnuglpxcn.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gfrmgzrhh.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gnulzhuay.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gikxouldx.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gdaiuaxof.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gvhhpkvxy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gcosvurmj.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gjjsaspyx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gqzsfusug.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gifgiyvby.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gjxmdufob.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gefegigme.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gyyxvonod.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gappmhfog.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gewcafdwp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gfrpbyqjt.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gimdovmfz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gsdqjauna.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvciajn.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gwuuqzeff.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gnnuwomki.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gatwjyltc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ghvolfoxx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gyhvegdjw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gqvvnbljf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gfputzoeq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gkzasbfyu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gevcknhun.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gsjbrzzfd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gvibrpkeh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gydtzdwho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gmhzpyqnp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gijejoxsc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/guzcqlfor.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gdmcslsvh.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gjgjwvwum.sHtML


<!-- 参考信息 -->