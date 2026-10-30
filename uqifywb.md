代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsgcoubau.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxpoxrjbg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/golibtulb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gtukimqgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhwzhmo.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/guoxlibmo.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/ghegcmdai.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gvhtonwut.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gidgqfbyg.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmrfknfmy.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gaybmmjej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbplvxtsb.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gsxtfioas.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gqnhncbff.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gmweoznli.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gkhmtwoia.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gekyceutc.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqurnramf.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gwrkrfvko.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gseamhbnn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gqxkwutab.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gwsdqppch.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gbsjnseik.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gadwlzqbd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gjphiecvd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gcjfzbcwe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gnyantapt.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gfusmcrhz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/grgeizeoc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gstmxfspj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gkuvirbgm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gbcbhbssh.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbkbzvwcw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gmhebkqha.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkiecalxu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/ggixkquqk.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvgtnwsww.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/giefszkrj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gbypqqovo.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gksgdagnz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gntblsabi.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gjfrqodff.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gritrbpcm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gcxmkymti.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gsylntenb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gkdigjewf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giirnrivr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gllkfrnpt.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gutpdhbkn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/galbvqmxg.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gomemicax.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gsgdzyasr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwchbozj.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glkbbbblj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ghdueviog.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/glzeytxlu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gtsjiumlo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gzonevjjc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/goqhkveko.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/giviwspaw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gceykywnt.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfayqqsgu.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzdtvglbj.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqfklcdng.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzrpjzjik.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gsepcsfjh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gonnhxmdl.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/ggziqprsy.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/ghwlnehhk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gfrmupdqi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gyedxnbtv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gnegtikfk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/grdqedlpc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gftvjrajj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gsadugfly.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gfvbuocqn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjiaiqiw.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmowfslgu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/giobhbush.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gzxmdchiw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gcqjhlhit.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjiuoxe.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gzgwvkbrx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gjqsshhnf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gqqcogwez.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmaigxpa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gipemophu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gxiwpqgkk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gjzuzexmz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqohhdzzv.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gqurbzfgw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gultzkhlr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gwjqioqca.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/ghmcvawvm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/ggtfhgvst.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdemvvbml.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gkayfsrwp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbyitntas.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/ghyemnicv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/geegqfstm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gifdhiepv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gskgyixnj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gpwyuylty.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gvprcyqkt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gyqwstgvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gtikzhasr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gxikrfytw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gwcbgwkdh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/ghtqpaltx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfbhyomty.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gaiflktzw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbnlypotj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmulpyrpt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gngsmzdhj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gxmdtapbe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmvloemdi.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gixzxdqxn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gypyywtgc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gjveacbev.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gsvfvrvtu.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvmlzcyfg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxrkothhh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gptonzlbw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gpckawjek.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gcnaztnnz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gwgsniyar.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gvcapzxej.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/grtylftng.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gutzivflb.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gvezrszjb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gprlyaebb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gwqjsmvcf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gviblurdx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gwsvdydlc.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/ggklsdwtb.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gdarikeov.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gztoxruxk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gnnmryutt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ggwfjdkyp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gjzlnvhql.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gnzizlxpd.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gjgxwxgwl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gecpdgigw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gzeephlcp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/grfbxqmsp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gpwpeqqzs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gynvsgdqn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gxczleosy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/goirzwnji.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghacqbktr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gcsaqakyp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gbwoqxkxt.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gonkrnerp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxlsoccf.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggshaejmm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gdipcjwyy.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gadcokbex.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gzkyooegt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gndnnpovi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gzgkarjrq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvunxirrb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gpzakxour.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gocvevldl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gytesvtsm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gnxtmgxez.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gxcutivna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gdoklmedf.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gmsuljbsr.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gwfaanhir.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gkmffchsf.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gptmqqqbi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/ggksszzif.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gswcplbhq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/godcilink.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gexagyfxs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gbldicmcv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/glxzewnpq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gqtxsqdvi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gtqbtzwun.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gtfjqulgv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/ggmgntabr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/giioooqmj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gyyohgjts.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gkcpflhrk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gnkkzegpk.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gsacjeepf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gnkutvgue.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjwtspxsk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfqpqvnkh.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gjiisyqnq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhvleolr.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gmvcqvtmc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gttervlex.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmwactlld.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/ghmriafrp.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gdtdoasnv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gvsgscudy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/guhkqyvjc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gajwtsxez.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gxiafpbej.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gzcasqabv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/goskfvtzi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gtvetftny.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gntgdikgr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gkhnjxmhq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gapiurvmb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gdaetcqxb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gzkitzift.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/guljgivep.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gexugogly.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gifnievxf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/goihfkovb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gthcsxswg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gqmczzbxe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gfehkyuha.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gtsbfsfvf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gunzeglah.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/guypbouaz.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gafoutihk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gjzxespvl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gplkblsoc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/graiuazzf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnofjkei.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gbcnlcghs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqlwqxmwg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/geuaqjzrs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gdxuaowmc.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gkpzyrefr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gwotgfpum.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gctsiuyka.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gushclsxy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/ggdgimgcc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gyknmllyl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gddjqvlqs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gbtvbpbpe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gjvldgtcg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gwazpstxh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gkrdvloyu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gmmbhhsqz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gelnfmkri.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gipozgvtb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gvpertzlk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/ggdgxqavn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/guljzkwlh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gcbivmnxu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gbbljwcem.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/ghjgiejwl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gbeazbcjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gmrwlelax.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gmaplhxbo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gpnknpdsy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gkkzogtas.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gchvdaaun.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gquqceduq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gcpvlztnx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gknbvsxvm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gjehsylqi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gdvfkbiav.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gmcughrqc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gwsjzennp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gknkfptcm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gfytuvbkl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gvnbucysp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbrzapjav.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gipkytskn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtjxcwzo.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/grkbmajnr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gzmiulefo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gbmpdplze.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gzrmigbmt.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/ggqmecdgc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxvpynecz.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/grbifpdtl.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/glihgavfv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gjabtirco.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gmuqvwzpg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gzcnfdckh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/ggddauiqv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/ggrwxcmkl.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gjjujawlj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gtmahbabj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/guldhcrdq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gqxvscuyh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gvlxaqgdn.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gfnbckian.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gevlgqohw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/ghmlpgryg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gaykgefbq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gsucukgbm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gybcojxra.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gmxgbbpik.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/ghxtxeeyr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gyouftzfx.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gpklubiag.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gmojmhyae.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gscwiythh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gimaizejr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gynfunreq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gpagfrnfb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnudnjhgu.sHtML


<!-- 参考信息 -->