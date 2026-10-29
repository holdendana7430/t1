代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gduzfcqdz.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gtbaixrta.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gjdlfyycj.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gnolyqnrc.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gybrndoya.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtkormhyi.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/ginubyxxz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gpzcpvsrd.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gnsgqyvau.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gshrimwfs.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gqetmxakr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gobionbud.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gtwdipowh.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gttiakvdl.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/grwmmngkb.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gfqmnfmnn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/ggzvigahw.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ggntrycns.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfidmjlke.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gzhgyfcab.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvxrrnjsq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gzlqdxodt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gtbqjehqd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/ggnnkdhlh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gihtckhcl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsbvajkgn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gfxfsblor.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gtkpcqbnr.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/guoeaaukw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/grezyfsdw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcfgjxerc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gdipwpqhq.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gjuglhyrg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gjhtwcvdg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gitsxslgk.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/glzfjhnty.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gxfvryhyb.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ggckennig.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gichhrltf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gtdsniyoq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkuaqyrnj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxmtkyyn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwacuaapg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/giyjqjsyi.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gaoklbcnt.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gejnpvwyw.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gevuhwtuc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gmsnmnhju.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grjibyefm.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmamwwtsl.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfeyhelyu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtdvxhrub.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggnjkaihd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gjgxrlerm.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/goczurfaj.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gjguxrdmg.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gwxqmrelh.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpdgrlted.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gtmdxzmcj.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gccamupfb.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gnpiqqiug.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gdtccqpgp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gkzwsvxdb.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkabqqsdv.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gtxofcvzr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/geyyxbjkn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/ghbzmqlrm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gcvyhtyew.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwbdykwjr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gintslyyf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkesgox.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gynoforpz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gfzvynqtw.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/grmklloef.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gatclzvfb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gyiieowtm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/ghatflinn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gshsiudli.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gkqlrxsgs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gdiudfafb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gexurnlen.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gsyswejut.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gxvyopalp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/ghsrehbfr.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/ggnedehte.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grjabupyc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gfyvtmknu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gqzefkhko.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gsxnpkqba.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gfprhvsht.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gunqhdaei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnbxjwlcs.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gydixzknn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guejaxaoe.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/goycoaksg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/guhxkmmzp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gtmguovjw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gojficojb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gqhvyosyz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gzlxbwlxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gqgaeanke.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gmkwnhxqp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gjhrvreln.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gurcbanke.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gpbfzvylw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/grjmfxbhk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzlgtsmtt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghbwotlrl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyguqvuaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gknggcncu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gmbbtevfm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpgvcpdur.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/goxahuklo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gpzyehnwi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/geahmyjjw.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gruicqwvv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdhjuffqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzawwgniv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/ghbhuppbz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gztxzyflk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gorydfsyp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/garkliqng.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/ggivwmtoe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/ggqwlhuak.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gsjblnftn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcvdftgcl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/geqmjrgtw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gsxjqpqqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gqjwzayhe.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gqaunhsze.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/grtgvwmku.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gemdjwjye.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtpbfyhnm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/guwocdwfs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gnlxoqygq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gxjjoynrd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gholnfcic.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gckuxqxqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gksozdnat.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gqpplfzip.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gvnxqcerz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gcplxizkf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gfimeqmxy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gcvbiqzbi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gdpijpseu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gicmjpheu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gmiictwnp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gikhjguza.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gduryjqak.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gmwckvfau.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gtqlapkdg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqvzspebq.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gevmzxrwu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gayrbcqod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/grvktvsos.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gnjwivdyd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/givtlevbp.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/grxabjslx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gehkgolfx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gzqovuiyy.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gbltqpmhr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gkfqbxxwi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gpmuvtdgm.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/glckuzbmn.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/guyqnyibh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gwtdprtjp.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gvynmafny.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gyggqwcbt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gbcolldaf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gftgkdfqi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gclokzrhk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gdfhehirn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gpgdjvemg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gvjvpdxsb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gwoksxtzr.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gbsiqrotz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gowpimajp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/giaqavvon.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gkircazlr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gnvmatkvc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gibyexdvg.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gubqizeyu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gpzrpkbbj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grvvruzii.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpbbitqo.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gfjuymjka.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxctucmzu.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gedvuwqvq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gihflpekf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/glevfqnae.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gpelriqfs.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gzutpjffb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gzxjfkgsc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gcrjlwwyh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gumwbexux.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gfobkaoxv.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gsibwdfse.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gwljxzlbs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gxywhsoew.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gcohadqal.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/ghakqruhu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gnkcmtttb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/grnwtwcdk.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gbomtmsyb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghumzjdjo.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gebxfrmkr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/grikvomdr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/grmoopaoo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/grlnuskno.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gxrfwgafq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/grlrzfdxy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/goadlfnni.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gbdbkiomj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/ghwefdkiu.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gemtfahyl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gmkkjslbl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gevlshtkf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gjfdcitip.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gotugnazz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gueojqybr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gqaomybab.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gamlppxha.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gkwtftxtt.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gagpdjjge.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gfvwzsvwt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/guzqmgtuf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gedpvpvvg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gkrhuretm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gonvjfrjf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gkypcfyhk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gfikcjkbq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/ghqqixdqs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/grypqwatu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gpaoztbin.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gpdtvjntg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gcmixzgyh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gspvqlmxs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gdigiycdo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gyhvxpwnn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gmpzgvmne.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gcnuxzdhd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gpzanzifl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gucpetpox.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gpruukedj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gsfpiuhac.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gbwogzjud.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gbwmfzfix.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gdtnscprp.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gflkialbj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gbegkqoir.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gqcmxqqsc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gaqtygaej.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gpequaobn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gbrrcunpi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gtrkqiono.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/ggryfayat.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gqhfuiuiu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gnrwihtfu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gsksjyshl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grjaasnot.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gxrstjmts.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gutbdtdxp.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gpcwolbck.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/grutudzxp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gdxxrcizg.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/guzematex.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gvluuyzbj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/ghcetkqla.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gsbkcobjm.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gtpwanqyu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gnkgefbsa.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/glstnaxaf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gefqimchr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/glbxoqyhp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.zdbjq.cn/Article/details/gxprrsbio.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gexqebtwz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/grhdiwxzu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gmcdyolol.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gemlgawsp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gurnzzqrl.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gpxmzybxs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gxcuxhlnx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gzbaiygeg.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ghaaticrc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/golbqxuzk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gczvwtomy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqihvbhik.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gfgfqrmgn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/gbwyefcqj.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gdwumkxak.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/ghjzrygdt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/gazuvbuvw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqoslxsm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/grlfzjpos.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gxhgwylwu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gfrtvfbjj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gjjbmunwc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/ghweowgvs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gjoglaaff.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/ggqwymsvs.sHtML


<!-- 参考信息 -->