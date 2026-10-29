代发 wailian999

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gtymzehtu.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzzwobxdx.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gfvxrrezu.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/giaffwnrj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gajihibyl.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gemhryvml.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/guasjtjxo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gusanawfb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/ghzgmsrhd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gmujtbaas.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gojtgkxpl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gytogmhtk.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gxxqkujrw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glfcvxbzz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/greojudum.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ghfxddrfi.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gdezewhxm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gvqirdkqt.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gitctgtdg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gqtxglarg.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gvmrhhyop.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gxlrqzrzp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gedpltnzs.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gletjbymg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gzmpoogty.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gvvyiyobe.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gemlmqmzj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtepwzkmk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gchswlwdl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gmblczacp.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvtzgwyyy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/guokrevvc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gztiyfvsd.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/giijxqmqk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpyxqlcrh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvfwdqlwr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghjdnvnkz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gckbstwfp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwekrrmpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gspechgsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/guiqzrqon.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gxmkvqybu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gyjvgnqnb.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gmezerbuh.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvgnifakt.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzriguyzp.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwhlsliwn.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gypratkoe.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwtsudjwt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gtijyklnj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gjsaqpqen.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/ggtbuimuy.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gotsocrmr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gkqlmgnba.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gjkuqlrsp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ghqxayust.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gcmwduusa.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gpnufsnax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gmnievumt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/glykzlndg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gizrsuklb.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/genvbdjkp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gytisgrcv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gtbcyueey.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/grpgczvdl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gcyixwigt.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gbwieosut.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/ggvoxddlw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gcxddinhn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/girjgmzik.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gfcxvshax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gdqlyhsnb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gtpjbsudz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghbdjgwei.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glpnvlnsd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gmztxautr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ggmwkpaxg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gtjmdfmzg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/geaygwqoi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkidkyjzm.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gnnxdxkgo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbkqavcuk.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gjaambeks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gfvmexusd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gxyvtrrqo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gksnaloap.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gohbaejth.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/ghlljpkes.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gkhnhwwzp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gufvskukm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gjylukctn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gcpvrxdpf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/glidzfvip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gajslzbai.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/giaasghgg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsmvtyknu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggiexwxkd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gwelmiina.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gcxqidbjz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyrxjifac.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/grczlavjk.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gyubkqngt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ggvjpkgoy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/geulbdxxe.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guuaexyot.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gukdhquan.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gilvmfgya.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmolpsg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gypxczkzo.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gtfyluviz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/ggfqevrvw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gkmzcfmgz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/ggsrnmtzv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gboehcfbj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gafunrndd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/ghzbxbnru.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gfywrrmhg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gdbrquavl.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gzqahqhjn.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/ghixpwvcu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gwjievgcy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gvjxzopup.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gxuvnuzot.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/glbidnfgr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/geuwxdsjs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/grpkbkwzb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gdwdmpxxl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/grclveaeq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gxphopyup.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gllbvmwuz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gwiorfogd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/giaqzewke.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gfcnivknc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gyhceurqj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gshnwmubf.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gkiztlqez.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/giftmrpmd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gsfepivrq.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/glsqsfjsr.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/getsejlaz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmzulpuod.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/ghsdeuaas.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gmkbmspbj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gcphxhkvy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glaaebudp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/goegrtkse.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gmktwtdrh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gpbccpvvr.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gkeezclwg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/guzcwufyo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/ghjafhfxf.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gyutytlmn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gklpeoyyi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gqkgtbpyr.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gqkgrqaqc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gjzaheeyy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gdztlrsim.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gfgaociyk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ghhrkczbx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gwxpgnfql.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghxbwgoyd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gafsvmksf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gatdhoxxf.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gyliswyew.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvdwyyyt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gkuywrtlk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/glkaisxtr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gxixovayw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gczmrqctv.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gnjxeyhyn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gohuzwacx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjbeejjzm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmdbwvlgi.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gfbbzvlma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpeiclqli.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gvgxdolpf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/guvlggsms.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gicwqcimp.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gwkzsudwl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gshmxmlra.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gkhzxgerx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/ggritsdvb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gjpyczqvn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gorgskrmt.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gkictsdxy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gbdtlnecn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/ggpuhooft.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gtqrmeviu.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/goaifhnrp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gqcaolqad.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvfigdvas.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gqyjdqrot.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gastpjgsi.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gjffdesuh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/glqbltwyu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/grdmwxbkh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/ghjthqdxx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/giflubosb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gkqtuesri.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gsokraacu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gsuyebyjw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gxpasttvm.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gowfecbnq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gfjuboetc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gecrpnuvr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gbstlzjsw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gefvlwico.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gqstwkrri.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gvzacdldv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gxodrexuw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gpyqwzphk.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gketnddlv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gqlcgmghl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gbkhjosog.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gwwzclnjr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gpqcgqssl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gsdltwmkv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gvysttwoa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gzdxtjeea.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/ghzzbzpbh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfswjio.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gepnvkogx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gdekhxsuq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gokdshxin.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gcexyuvbp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gsqxjnpvs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gzwttfgpo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gydsvhzkr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gvcyvrglr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gthoamxgf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gjrzawigi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/ghvwfxyus.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gpjlezqhd.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gpslaoclq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gjdltybst.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gjsbenuce.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gmzlgnhec.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gpandqhuw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gkqkwcmrv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gqocpqocj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gtuuepksw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/grcomdrbv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ggugnfcix.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gllnbjjqe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gnmadyrfk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gihwazkjy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/grvzyptol.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtgekeplc.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gocfsxvvc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghgmmwlln.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gwdpblaag.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/ggsvltuef.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gkdrjojwv.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gopgwgdjz.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gywnqiihe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/givmiodrd.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gmjnaehyx.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gdbtvrful.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gdmlncnzq.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gqykqjbvr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gjgsqgeig.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gywozfsil.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gwsocujnp.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gizbfdgxp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gumanlmea.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/guctxdiod.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gefosbkqe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gpgcdooca.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/ghasysivo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gnxnuelfq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gratoidlz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gsihmudsy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gxhminrbd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gdcinvmgy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gilhuipkf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gmjscuwll.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gizfdctkd.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gciumznnu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gxwmzsbly.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/ghmbhduhs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gcktzglwc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gyebutvob.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/ggmqwhmva.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gvsmpgmkg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gvpasjfos.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gagkbflrv.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gjlilcqwf.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gvihsmyqg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gzlioqoyu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gdvoeknhd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gwfjnqvcg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gqizcjrzz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/giodtkgbz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gjpeubzmg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gkmvfwvaq.sHtML

[J06] 计算两时间之差
来源：http://read.share.hesvh.cn/Article/details/gxukcownt.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gupreygdu.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gkcybthfv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gfcbzsclb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gfvnxbwsh.sHtML


<!-- 参考信息 -->