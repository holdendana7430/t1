代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gkzyzgeaw.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gjsllcryq.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gisihhqzg.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gowsvfayk.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/glmgsvhec.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfrlebqoh.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbwtptzsy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/guixgjfzo.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gviswryib.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gakiuohhs.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gbwcpyylf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gzerhhswd.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxbcrgyjo.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gttywkumi.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gwloizweg.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwprvnvpo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gmxjoipkc.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/geaxiqmfq.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gjffliwue.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gizxljozd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gwdmxddxc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/grracqygj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gbjzzxswm.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gzkhmxcow.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gpfyxdqid.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gzhvqndek.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gfhwkczcu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/guplpdvil.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gnijtxidw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gpnzznzqe.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gsliqmhcc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkfzukl.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/griqabgje.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gqvvsvhfw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gwlacwtng.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ghyowwpgm.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gcftagcjz.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gbbhunejm.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/ghovqrsyu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkdbukjbi.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gedprbnkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwtsiyjct.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gigmryppp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gakhoqnsd.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/glqeohstj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gacujcqaw.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gdhyvtcoi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ghvbknjrp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbmcrasjc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grtxcudxd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzsyndfpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcxautqat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdunirhur.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gecgapcku.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/grghzmsmf.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/glavxymmc.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/ggtvnkylk.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxvzxuvsa.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guempplko.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfaagsylr.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnhfsdgut.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gzahbeipl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ghjvgptzl.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gapslyyov.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gbpejzzep.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gkdagotsq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/grqkehflc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gxdqkshqg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gjuquyoxc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbqummvje.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gnfrouamh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/goqedqhjx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gozhkullt.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gwzxcvlrf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gpkhatnjt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gkjwnhvoc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/glrjafvrl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/glvuzfsyz.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gyjlbzeab.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gfhddfmng.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/grgdrybvg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gmbxzxodh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gtqqwpmol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/geyqxrfam.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gdplledao.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gjlnpqwhd.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gfkvriysd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/geejqqsyx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gpguhowsz.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gyefilyuw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gzyzlmnxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqzoeruyg.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gjjftwldt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gijpgtzvq.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gixvxzrnw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gkbqzbkrn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gvmrrhgdz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grhkvsrkg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdxaaydns.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gdmetyfsj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gllpdvjjp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gkhzvidxg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gplwtvpjn.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gwybkpsdw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gozqaxibt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gkwcqpoan.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/goshdpgva.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjllzoeao.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gnprmpyhu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gfwefxsui.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gcqhugtnq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnquhnpwm.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gkgjndoyv.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gmchsrauq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grztyzgbl.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gutdxvvls.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbcbnrsgg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghkypgfeh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/guennqfdd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gkxrshnnu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gihkzkikj.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gkphhmowi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gadpjsnru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gatywxjhr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gtekxyybs.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gobrwuqml.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gxxdackkq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gvressjap.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gqvchqoqv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gswmipdnj.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gfywudmli.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gpkequhwq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gumyvvdjr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gdurhptss.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gehjvrdwc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gcxeguwoi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gcdfhvetv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/girnwstpq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gocvohgsk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/ghvwmmyct.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/geoquhhqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gljtpzgkv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwvkugoxa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ggsbxpame.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gfahrxzme.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gaopmrugh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gahppvhvz.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gccxpnjiz.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gbiudruyk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gwiygxvlz.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gpevbpxpb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gulfviojx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gzmjrvlnv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gygeunqlc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gccclmroi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gahpurmrt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gcpbpmhmx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/glrbtntth.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gaufnpsnu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gchgrfgcj.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gdzjmvyrv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/govxwsuin.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gsqfyhcgk.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gjeaeeabd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gujlcsrcg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gnpsejtop.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gesierutf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gjtdxkplv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gpveemlwx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gpavrfrrj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gwxlxyism.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacpqhsph.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gaqjschuc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gxqghknes.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/ggnyuakxg.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gedbqrjeq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gfegipruw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gkbqfriyd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gmdzoibyy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gdycjgavf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gjxrvtohl.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gigtrwwqe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gzbwxyytb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gboxolkav.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsyineyub.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gsyyetpmt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghixtwtas.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gtkdjhahz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gvsrdthts.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gbvaukvww.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gdqdjmjwn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gnaqiltlx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gqgqxxbci.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/ghbrtqhzj.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/giztwnohd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/ghknhoimg.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gcqtoowfp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gqwfvtqwi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gpdkypcit.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/glrpvwvav.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gmctnhrwt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gfvczkbdk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gwqeemepc.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gltnomwjm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/ggquvbmhz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gpmaoszwt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gryasdmlm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gwuicmsrw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gphuwbiwo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/ghyzfeehs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gghrywejq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gzfhcafpd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gkkoeyyjr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gdxsoqqmn.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gksxtmvlq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/ghaywmovz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzcclhytr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gfeurjnub.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gorhjgzbf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggwophewf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gcrlyysut.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/guckoxkhn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gvdkseypd.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gqheyogdp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/grzaovuuy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gawbjutbf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/ghcfhlnme.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gzwfiyhvr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gdjvkfcqk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gwpewderc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gdjcpeldm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/grnkhnlpd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gkxnimvnx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gphsxtybw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gymyvquwy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gqgohzuiz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/giausjmrc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gfpevlwko.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gghxtopef.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gidoizwix.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gpfofbpip.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gesucigmx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gtxxvddgx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gyrlzxfjr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gjopgdrlc.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gqtqrvaok.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gwqcjatdc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gzrcuvuuk.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gseylmfrr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gnuruhbws.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gpsmxacqz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gjnhiuzar.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gfepvhxlc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gunonmnif.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gbdtnyvjd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gfowilbed.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gvuqabfgz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gktonbjtj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gcwrdrsce.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghzsomfdn.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/guhdkyngb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwiqxmolb.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/grzynlhtf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gbsvccyio.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gqwtkubqu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gkinldzgd.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gkjcjbygn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gilgzeruh.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gyuhjpfki.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/grbsblcuq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/guuwrrduc.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gmeuldwww.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gwqttgjxv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gzjfdcwvr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gbabxepri.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gaipgzhyi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gepnpaboy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gaucmruap.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gltndekfq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gtnyhqkao.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gegcotucr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gcpdvukzm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gljztakzo.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbimzdjbb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gvilsgduf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gcjebwflt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gjdjmummr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gmweilwwh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/ghzaudeau.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gyqlnjulb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gvqibfawj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gexmhjvxq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gimmpjifb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gvovhcrxa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gnwcweukl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqesftjaw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gozkhghmo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gbdugcirx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gxuiweyrq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtaufvot.sHtML


<!-- 参考信息 -->