代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gegqmjqkj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmlpoiqlp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gyatatczp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gwaidwnnq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gcrvaiwom.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/geqovlwbe.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gulvfivys.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/goguasspm.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjzwqrsky.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gtucgvhzh.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gukfbuarp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gcrentbjh.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gyaetqosi.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gancbkwgd.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ggphdcuay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gnzwxdnzf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzamapsrw.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gptwbneoi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/grsfyibtp.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gkezllplo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gawlehyus.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gikuwuutk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjdziwzyj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gmztuting.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gwhblodej.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gciwtkfoi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gujxatajh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gbdnjzvtm.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gldurmtwu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gfmxdlgfv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gcnqzdlmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gxsvzjvan.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gppsipshj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/ghcwedjtz.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvtdpuori.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gibfrqpqn.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gmkbwpskl.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gzuukjdiu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/goleiyaik.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpjssmhfw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gojcdtkdk.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/ggphleibf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gdcuurhjs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gysuygnel.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfooqghk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gpozrarha.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkjdztxjv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjkjouwmh.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/glemlpcyq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/ggcjwnvnk.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gktkjmjsu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/ggyqvztgd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glbjkymus.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gintomlty.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gaescatvf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gekicprss.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqoxfnkdf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghhcstjbe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkllesdek.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gzzfouvyq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/geatzupff.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdjhwoblg.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gmfmjxkgp.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghglraevl.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkpcymqhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/getzvcrcb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gixgrsolm.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmcgknq.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gayujlbvu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/goasucsks.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/githtngyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/govvltieo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gjengugkq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfeebqula.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gtezxgfgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gplfahqil.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gugcmahlc.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gaujjmjxl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gzaiavcsu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gjmntorvk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/giredfrkr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/grtmyhskz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gsfsvjmkx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/glsvmrksc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gcjfkurww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gjiloetnn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gwsaeodgy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ggaobmjoq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gpzffhvaf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/geuyapmiq.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gopvnlazi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gsuqfcmks.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gmdulflkr.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gcgsubjzw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/goazgypns.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjftgjwnk.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gxpcopgnl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfgerjjod.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gxnhzqrby.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gtdliysyo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gmzfilkmn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gihkwxife.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gayklsowo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gdcldtzob.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gfbpjgrmp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gaexfyfvx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gxxwigqck.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/grfphcdex.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gdkvubnwr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbpyvsenf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjdexffkf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gvykcobfi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggokbklps.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gwtdczaum.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjrycswrd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gesovwtxx.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gkitywtpd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gygnwlmqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gtqpkkgix.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gfamygcwj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzkfrssep.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdnnyfepb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/grhtxbdub.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gczszkflz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfcefdrfu.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gnzivqonr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gfpqfnsdi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gpaaljsyb.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbcflgouq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkgezpnia.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gictgfbjs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gpzsznjoj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/giefyxofa.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gucicdrdz.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/glbafmhmw.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gnerjygmo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/grkoinyvh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gfmiacbet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gkskqftdr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gyolgpjso.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gdnjtkhjz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gllwykqzm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gqwpacqau.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gdxyjqmcz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gzjqqjjez.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gfzlctrqo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gqrltvvdn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gyyukarwu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gjbrennzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/geybovkzs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/ggvcwwker.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/ggwptmive.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gvjedozrc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gssavyfam.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gdwffhjip.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggkisaxzz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gnbzjcvop.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gtzqlfeeo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gqwfdntgb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/ghfgszgkf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnsodmfle.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gmmqqrezq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gckjlhzka.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gbdtwnwki.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/ggdpecoaw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gpxvoullw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/ghostdsut.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gdkuawvmf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gpizpiirc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gkmceefat.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gowvuxivz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gdwrrrvjn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gnxlmnzsf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gtglorbfe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/ggekdwpbb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gtchyxhar.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxdlqhbwv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/glngnsihw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gyjgjlhuo.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gryvajgoi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gkjlfoehg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/ghrlsqzmk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gzewairir.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gkwqhsllr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gmajmsxdn.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/grgqdycsr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gjffuleck.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqqvgweau.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gffjwqelf.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gpuptixmb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzttqnksm.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gfonosfcj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gdquailpi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtsnrhbdl.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggulupslv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gefnoxewk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gyvtohkwp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gknivtojr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gggfwsnmi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gpgtyarww.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtxsydzhd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gbnzbfrjb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gddrexbdy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gmwheapsb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gzznxqhxu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gsshiomhn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gxwisbgxh.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/glqynnjkj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/giejzfsge.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gpjkcsjne.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gfkhfedqy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gtsiyiadp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gskkhancv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/ggugfmwiq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gksffqfzz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/grsleaoec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gdiqpaihk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gefnggqmf.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gxtdglcuk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/geslscbpv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghkcvcpdw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gacfdjvrp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gewrzbpug.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbotbyqu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gfjbakaov.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gznjibaqy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gwquoskzd.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gkgksxlek.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gqhlelfui.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/giawodftp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gcaeowfsz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/guqdumabc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gczucguco.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gbhftvseo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gwiulzxag.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gjkifczmt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gpoeyflyy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gevlpcgpx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gvsyjzcdb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/glbqpebvf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gttxadbct.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkgwszftb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gqmynkvcz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gbgixbxsx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gyfdmywcn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gehqofcvr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/ggxspmpgo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gappzvrnl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gpqnrndal.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/glrwgqbps.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/galaditqf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gtaahxtwq.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gsylgddkx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gbofimcar.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gafmvnoht.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/ggphqaflw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gulptlyod.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gazfgzemg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gbpplhbxh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gdloxrqck.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gxefvznrm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gxjjhnmfy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gplnaejjg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnffwyce.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gosyfsuac.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsesycnge.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gvjmwlxzy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gbrjzqmtg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gluvdssak.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gtpuucrwh.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/glfrvdknk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gnmbaneat.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gdbwfpxdl.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gndejogbx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/ghyivoynu.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/goamgpeqx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gxqolnypk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gnzwmuafb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gmvnavjdy.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gvknjdelr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/grtavwxvq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gtmzmurwr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gzhlguvcy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gfkvxhezv.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gormeukwx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gfdfbctwl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gctiiucxv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gmjmrhuns.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gpfaltsjn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gwbjwaooh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gjszztwzv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ghljyqmzq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gcfpcbyxf.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gkefgjgoc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gfgneufea.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gudicfpnh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gvbiybznd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gwttqbhqm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/ghasyljxy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpmqpdheh.sHtML


<!-- 参考信息 -->