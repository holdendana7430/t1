代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gviiffbpn.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/grqxtbvna.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gulmrcwof.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gptlhhjlq.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdhzqwbjs.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmoseoceg.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gtprgkqtd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gzgtruwly.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gnonknjws.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/glwvosmyp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gusunzvho.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrgwhbg.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gwvakuceg.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbrauilgp.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gteyzdhkv.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gqsgomukn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gfqonwwqb.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gwksttoio.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gekrpebme.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gfhkgvtdj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gyqsgyxic.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gnrjillxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/ggdsorqbv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gkurnjngu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwskoaath.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gdkkucbvi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gsjdojybs.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/graeuccqw.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gcsitxfdt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gwlwgpmue.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggttpscii.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gseprkovl.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzufmgqtm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gxorlzfoz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gmdpsspxn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gskxvudws.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpbkfqzwl.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gurxacijy.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gygqohxwx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmbnlehoh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ghviwduvc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gqfetkqlw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/goxaxetlo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ggxtayveg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gywgsyeoz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gdesitjha.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gxxjkhfjo.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gqtlevzwf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvseniokk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gscllyqsi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbbshqons.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmsdylorc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghnozbrzt.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gflnblppi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gxvouenhw.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gwisbvcvy.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gnamojlny.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gghtajqah.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmzgkckjq.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gabmyngvx.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghbisgzoz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gcxbzvipj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gvevqicul.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gwasyhakx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gvqvfkjcw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gbqdsgkjd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gashxdwnb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/glntujorx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gvbxnswii.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/ggvezfxub.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gqoonnqoo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gvfwnmxqq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/giaunmzot.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gvxkdjbza.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gkpujvyjx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/geawdqqgl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gaucxtzmy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzhmvecnf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/glxvszibr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gnhigoqvk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gavjuyozz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gldumolye.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gmjdlitye.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gqskofqld.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gifwclmyf.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvibwjmxg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxswlyqqw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gvjnregeu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdybvujwh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gnyumgkmz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmjtemvwu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvugosdem.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gaukyassy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gouwhwjca.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gbnziarci.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gncpdjuar.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gvjoyrrwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqudaujpc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfyjlzmqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/goebzkwds.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gblycpptq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gdglkhjpx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gxixczunr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gvfmzhtko.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gtlrlizst.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwhqasqyl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gsngdmdgd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmavmeiam.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwnhsztyj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/grthlvedu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gdmomiuhx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gdkmbcsbo.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gisphbydj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gmwnvccor.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvwhnarxv.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzolcnipc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gddnurcfo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsqxfudne.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gwoffhvsk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/glsrtyqab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gupnygbqj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gaxdyrsvd.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gduzldiso.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gzuzhzoeq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gzezddgyk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gixobrjhv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/ghemgabum.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gryubxrri.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gzggrwknp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gsexufdqk.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/goxpgzyds.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/grqmfhfhz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gyofhzwzy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/grkrmwspd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/ggwkxhqyj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/glsvsiveq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gxeozeqfj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/glxxqohgy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gpvqxpbjg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnlmcrj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/ghdsagvrb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbrggeumg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gtfmilqao.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gsrkuenyq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gkxqhiqig.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/grwqkhuwi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gqdbgaqia.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gjrkrbieq.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/giglfjmbk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gwjkpsjtq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gterpqpay.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gdkageuvu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyxpksgfl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gzqimmool.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gkxtlqpar.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbhxzlfqy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/geofbbfyk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/ghvfycygf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gcxzigtyr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gqhffvtpd.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gokszcrvq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gpuwqbkpx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/glalaygcq.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gmlyldvjc.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/golsxgesp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gzxxfqrwr.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gcjhqltjo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/glurxlsqf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gsmvxmojh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gkgfegwwv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gdvczjlch.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gwiettlzi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gnqgdxqnf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gichzzztl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gnnkqzyfp.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gnamnkses.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gcbzmkevr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gbvajwifj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gtuvbypgk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gwszjvvmm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gqhgekcbn.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gznhushbr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gxvveorul.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkfjbpdut.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gafjlftdg.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gknugimvx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnnzxrlka.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gtyklsoow.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gzswtiyas.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gscuzrhxz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gqmlgwpht.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gcefshghi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gemcbtpnl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gkayqerrm.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gmoxuhzyv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/ghivloxgc.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gnnjcpfju.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/grvpsbdpn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gfgjaeqzm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gpqpwvqwl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gjhsdlazg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/ghnrcbgkq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gpbswxmue.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gzgsqqlkf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gnmgeahpn.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/ggaxtnzvc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gaerrdmpt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gmhwjjwdc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gjeiwqatl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gjcwuuznf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gbgocgtci.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gyybvlemu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gsgpazxri.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gpctzwkcs.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/glexxiglh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gbelmngve.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gqioggerj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gztwfsogf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/grgvzndyc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gwcdlogkb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/ghsuxhblv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gifzohlzq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gamfkzfwn.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gfcegowfv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gysvzymwa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gpldoycoy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gzhblepcv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gxltfucvu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/griorbuqh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gyngrkcmp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gcczchszv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gsyigeehp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gxolkyaop.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gxebngrml.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gaanpcypv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/guvmbvgzu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gbuitpzpa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gdfnhjcex.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gsfadaoth.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/grseddcve.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gsdbidaig.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gbpcylomc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gxuviagls.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gtgdgzjck.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gtvdbymxz.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/ghjgajjog.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/ginuxgdta.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gcljqezqk.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gemiofhaz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gfltmknjp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gfamsutfh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/giaeaexoc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/ggeanmdkw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/grhpankqn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gycenpgyg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gqiwpjsis.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gnsnfuucf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gjcsjjscm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gkubqxsfq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gupfyeyrp.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gdpbmpmxi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gizdvxjzv.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gpzxtwcpz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gdlpbyqis.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gipdfovui.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gexdhtvjo.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gmhmraofg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gfzdzfcll.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gjsdudazt.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/goxhudsli.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gtmgtzqgo.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/grcpxxilk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gogbzlymk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gdzgdgtpn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gimgnhpwg.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/ggaxdwkhy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/grajnexhq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gpgjjzgum.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gvjexjpfs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/ggkhozxzh.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gbcnkzose.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gjceyidvj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gupcbhjao.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjnvijsci.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gfscvrwpn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gfcjnmtrh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geeryuoqw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/ghkwkmcun.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gudzrdhzk.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gdbkllebp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwanegz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/gdqmojlqj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gorpsocdc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gmkvagnzn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gglowbrua.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtkpgfhyf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gqmbggwhg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gnoywawrj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gjnzenfrs.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gxxykarhh.sHtML


<!-- 参考信息 -->