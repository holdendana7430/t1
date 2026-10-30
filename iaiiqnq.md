代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gexljplca.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gqbtuuhgq.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gbaxafjjt.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gtxfltpiy.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geeaobiof.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/glnvwqqpg.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gplgxnmdq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/ggkqjkulx.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwcmjckwp.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqvqdqgkm.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gocgzuvai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gkwoqxqjh.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gymiylthf.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfgrsczzz.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gwlmqpcvx.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gegtbxeho.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gabzajxsd.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gsilfsqbd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbhewbibo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gexvbcvge.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/ggansepzv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gikcagciw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gpouezyel.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gxlgijobc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gcznblwkv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/giwimsjnf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gyrxksqux.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gbxtdtsjg.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/ghmbpwfba.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gugtsyoas.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gbvpcokbf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gkuouibmh.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ghutkhuqa.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gsjsxtuph.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gwxmutuup.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/goybppegk.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/glswtleoe.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gubptbmbr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gmxnrllvv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdrmmwonl.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbeqohzne.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqaaldswk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/grkaftcji.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gwqrcmffp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gpfhkadhb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gijwddnmn.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gizcfbxrc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/goyjxrwrm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gdjenkkit.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grhkwcjau.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gyftiaxsh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzpuiyvjp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gmmkevqyu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gudbnzwup.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gyvcieaeh.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gsfzxkirt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/ggnrehmyx.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gemqssbpy.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guxtlucvx.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/geoftyfmq.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghktfrptg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gyfbvahjb.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gvfbpznue.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gqkngkwcy.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gijfomagm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gxdsxxaka.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gaanqsigc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/grwtpwbxk.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gbbinhzou.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gnyypeqcr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gvmoigifl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gzvqudalt.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gawboarbj.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gkkfxptmc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gkjsudpqo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gxinimknf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/guvqmjbya.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gznhffsae.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/ggbkaearz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gecfqggxp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/geqgoyith.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/glsvmrtjf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gexqgsuxs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gnbvvffpj.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gzkgahoyd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gypljjufm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gezzqumtj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/giamqqepw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gvlylcdvh.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gipdsdpky.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/grzaydzxg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghxubeqvz.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gfmnihufd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvyhxitzn.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gwcwhgxlm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gfnoxeher.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gykxjgonm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gxlywrbdd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gchawndvm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gtpnyjlrt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gcwzkaceu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gmxoqikfr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gfwxrvjzt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gzmwjldon.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gqdcysjbu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxuzxmytk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gscjlpbfj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/govwjsmrz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gozjulchx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gxyefmcjt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gbwksdmvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtxfepsqk.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gmvxdlfeo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gnplliawl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gachrrqzd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gzviqxcsp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ganhufsyw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gawvgzclb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gynvsisbu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gtfbqwhoy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gtgbuwcjz.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gtgofukri.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gqeecrekv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzzwmfvdb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpxctzrul.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gjdrfyjmv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gcrqglocj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/grwhgawjr.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gladjfnuc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gbepzvynk.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gppgeaehl.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gwmzjqbhp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gkclcgkqn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/guvdfpoyi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gucecrrwa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/goxxsptdo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gvgajtfny.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gnldgqnjy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/ggehcikgc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gzvuykjdt.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gqsntlcjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gorayhgdb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gzlxlbhdp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gnldiwnkp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gziooghsf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gnvhldcwj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gmntuopqh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gkagdirxk.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gyvadplqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gvktirybu.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gnqheyjor.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grkmsogoz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gfwfwksyo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gdgkmbscj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gonmuopon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gaezwtjiw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gdpjmbxgc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gnrrknged.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gqywbvzgk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gbdpzfqxr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gcqaulmvu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gkbxkwlmp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gjzanyjre.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/ggktvighb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gdlqucvaf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gyvtrvxhj.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gxyldqary.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gfvcvjbpa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gmwwdxvyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/getpijdwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gkzqynywu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gatxacycp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gsducmyru.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/glzzlkdsa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gplpzobyn.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gyhrujzjn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gheozlmba.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gwcfjtwij.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gqlledfnh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gavthkaqr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gpyrlbhrc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrtjlrv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gwervkexo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpqogmfka.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsykzzwus.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/ggrrenxtr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzveyonco.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gfvopldfo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gierqehhm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gbgisnwnj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gjbwmhfio.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gplytavkb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gshwhdqlm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/ghqopqhde.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/ggspwuztw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gmoxnwslf.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gccowritw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gcmoptbxd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/ghsvmpapv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gkthgkuxp.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gcvgqqomp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/giopdtjdw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/grwqqfyqk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeefccug.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcdkaqyfu.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gogprawjv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gjhznebtd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gzxbqwulf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gdovbzvxh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gbzkwsrjp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqucflun.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gnaeoyxvi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gvpiutouo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gprnplprh.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gwcnjtvdt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gjosdsevr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gukapdrsk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gqqjgtdzk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtahfrtwj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gxfwfdadp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gzjheshlr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gwtdbehrp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gziyksnci.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/glhrjgjla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gojhzffin.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/govbmfyix.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gohvhvjmh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gdybbmcls.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gmrngrxeb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gpemohwma.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gmwrpgnni.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gaadvguue.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gfadrxkzt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gzwvwneyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gecswkyff.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gsnnqjkfk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gahhyyrqi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/geakeaejp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gerpjsnzz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gcedufvzv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gcwtxnjrd.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gbmuucsyq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gistppvff.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/glnmfjebv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gjupnkskm.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gmiucxddc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/ggkoqwwvo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gtfbdhbgi.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gkkexhrot.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gvngwtthw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gvdjfvxaj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/goqxasobz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gwmbsckzg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/ghjgokubb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gnwpslfqv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gsridnplz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gshqopxne.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gifpuchzp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gyyadjggy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grlzxumfr.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gmevhqosm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjihvagky.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gmlsprtdh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/giqkjpbiq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gcgaiubgh.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gulmfjzmv.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/ghqmbrenk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/ggbrizpww.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gxssurvnz.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gunqyyyqn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gmkspqnlv.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gmndinvlu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gswcfxqip.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/ghtggvnwh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gcvqemsng.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gbqfcrdqo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gljjtntqj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gsmusiegc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gvmxphdhe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gayhtqpyd.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gqjluggqv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gjdytdkon.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gjgvjxvxe.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gluyzlrxz.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gobtszyvl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gzlkzpxjh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gvyjzejsf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gpijclzco.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gbotaokdn.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gbyagcqxi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gdeczyuio.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/ghgzykwhp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gigazjaru.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gshgvvxuu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcnnydcpv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gopwuxicp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gisslxnih.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gxzpkiprs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gyplducsm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvlbdxm.sHtML


<!-- 参考信息 -->