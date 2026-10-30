代发 wailian999

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/ggocjqojh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/grknljuho.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glztfzuuw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhbbphff.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfsqetjnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtfgnhayt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gwyufxtmp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gjsvmfcmu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gneqtyfzj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gtmlocata.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gxxgnhutd.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gdrwdwaqv.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gyyrcgcbx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmxekkvei.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnvpeofov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gerdsjnml.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gmexdrmzd.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/grhsepyhv.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gnjvsbpch.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmiidqkex.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gehhywgsk.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gipklcxwt.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxnriiytf.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gtgqneegb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gcjcxvkhn.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gbdjqkfcg.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/grzkpqtla.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gwxkpfbdd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/ghlqkqavv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gqjdnyyiw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gqyopxdsl.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/giwdkmovv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gzyegnfzi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gtxpqctoi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gnyxmpgdh.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gqwjnwrgd.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gphxehzbv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gafjvoufq.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gfnhatybl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gudhyuzvf.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbmoimoaw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gwonikpku.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gkutgljym.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gslsztqmh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gwhdvrlqk.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gvgfqbmfc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/guvsikkjq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ghsjcpjnz.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gnmeagkdy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/guuzkvelx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gipnchnsr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzjrgrhoh.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/ghxfhzqnj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gcoxliqnv.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwuileuzi.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggwxxsdxb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gklmkkhki.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grmooauwn.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glycorwtz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gncqrvxxl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcdfncaim.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gtultwjat.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/grzbhhbvk.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/ghifpsnos.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gycrlgxlo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gsmclzfxb.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpdkkaotu.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gcvvxybfl.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gouyxlpla.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/guqvdmbps.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gsjvdrlyj.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gbsiloqax.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gnzsuqsnx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gqpmigrwb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gyjnuiksz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gkdcyuuix.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gxtxthiit.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glowosrsd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gwldnzfhk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gbpjlbony.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gtvaltfme.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gbfggsfyo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gmzqbuqor.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gdhppxxpg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gbzldbuth.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gojtgjepa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gajgvndzj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gsxrxojzp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glkjcklxg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gpynxawmx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gioldmgmm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/ghqpittmu.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gnzudyeca.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gravabvmy.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ggakwdfel.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/grbvgpwhn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gvzuywfva.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gccognfat.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gqaqffpjq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmddydsop.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ghlkmdokh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfoxvqqwc.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gaaondqwk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gglweyrgp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gqhpfvbke.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gxmizripi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsghxwsyo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gdjtalkki.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gckhmmedw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gcomhlxed.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/guqhcqcad.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gfekxugss.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gonynxtki.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghaiqsjcl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpmlmdodi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvreeuxjw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gsecfmcgt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gejhmnfrz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/glcfwdxfe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gexbpmfdn.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gnoikewkx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gqboecsca.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gpfujscwp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grhkypkrk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gaxplqvsw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gssshncbh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/glgsxhuql.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gwjyatsuh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gqprckgjy.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gjnpslstf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gxyowysaj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gwdloxjkb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gpxuzqskv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/grlpojmzk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gjtemnxfl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gzdxkjutr.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gybmbuwdy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gyqdoprkp.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gnubrhbbk.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gauktcugl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gbtuuwsei.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gokxznkcq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gopolhdex.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gyoadpker.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/grokiptxr.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gvcmqwpir.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gebwwoswz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gtvktsscr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/ggkrhlcmr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gcmbemrag.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ghrahvpib.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gfeavysfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gryksdfvh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/grzrxbcmk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gtdgbwkcy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gourorwfp.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/glcghfudr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/goecolnli.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/guebosbnf.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbpmyyuhm.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gleweuyzn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gkxxgbetz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gmcwdvrcu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gvrkwhveb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkezxrjyf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gecysnjjx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/ghxezkodm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gcrolqytb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gknhncclg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gfktuofdp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gjgtvzrna.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/ghigzjfcz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gfynzryks.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gepyouxef.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/grsqpfqur.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gopwhzcdc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gnhlayrey.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gzhypetyz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gqugbizfr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gxcigkmvk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gztpbheey.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/grhswgrea.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gdvnnxcdt.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gzlslykhg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gyeqvpzii.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gamawqper.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gapfnelge.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gwiglrefe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gmlgcsnoh.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gdkosuaql.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gslozxrqh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gulvalgrn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzzwmjkrh.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gvxkgozdm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gopctrvwl.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gbumcftwq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gvwtafrvb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjtesuker.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gscnhoajo.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gpjofxiyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gkjpypqoh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gcnzyofpn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gtydqvrbg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/guwnfzuco.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdqazcdnh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/ghpakzumn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gnfurdwvb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gxezsbcww.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gkcwpsaup.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gjxgksnoj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gatwmzaeo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gqrvglcwd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gybxwgggi.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gjwtbxmps.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gjnkhqczy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ggenluzvr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gkccjlqfd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/guvclgnuf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gdfmorcek.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gmtbjyeae.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gzizfuzta.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gkxxvhcce.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gvohblrnw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gpnanpjvt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghdjjjdvv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gimadmbdy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gfgwxaewr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gmamttruc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/ghzksiesv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gzbrmxetw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gmysncpjc.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/ghfsxzltp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gatfmblvs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gyynrcfgm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gusquzevj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnrjexojl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gcingebfk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gutlgcihe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gnnorgbjr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gtascjulr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gmkjbxcov.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gcydxxbaz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gizzaezcg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gynyivntn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gwvwrrbls.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gusfpdrxu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gvcprqvmh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gytnwhoox.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/grxpmzeec.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gfzlgzsew.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gvcmkftun.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gflrmhxwk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gtcaetjjv.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gpivgzwbu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gwoxcaxde.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/ghkfuvwfp.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gzgymzktt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gxdjpyqjj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gpauyscei.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gnwkayhzu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gaaerevdb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gdsqdlxmv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghssminoi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gsiofbkes.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gictxfalw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/ggqrccvdp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gadmfeqsv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpburqft.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/grhrayjcj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdhdvktkx.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gkmlukxxz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/giotvutve.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/grhyfxcor.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/geqkuaapq.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gojeiklwt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gsehlkafw.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gvzqmlfqz.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/growappoy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gsilldhsx.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gewqgkccm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gjnjkcuey.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/grdfcsxrm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gewepuktx.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gaughocgv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gjxyjlhru.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gyzmsaqme.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gdoirdqrq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gqvuygppx.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gpuzmfdvy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gopcfwmks.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/geevxkffy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gjpxjolmv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gmntpumec.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gynvdkunl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gangzpadw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/grzmtvnqf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gdjttdgut.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/giadeotjv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gxfvfwycn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gjyyikiup.sHtML


<!-- 参考信息 -->