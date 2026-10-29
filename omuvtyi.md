代发 wailian999

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gupoifvsj.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/guygulwbg.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gmjahbhgd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/guwlutagu.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/ghzmjreik.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gquncdntx.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gywfdgjtk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gdadqnsqy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgzcvqo.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/ghxjrhnpv.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gsjbuwwzd.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gsspnaskq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gjpaewfzc.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/guonaxnkt.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gmucsghlc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gyrhxhgzc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/geyfkoorj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/grohagpgk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gpszrlmsc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gvnffttuq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gxvbnbwvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gywfrgvzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/ggpvlmlao.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gannwosie.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gxlqptior.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcjtamfog.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gldyxnmfa.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gokjrhplh.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsgahtzdi.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gpqnictuz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gcdvkfaqy.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gomdyjbzj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/glhphpbas.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gxhctdwwv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gohhyeufg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gqrisyuwt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gaqrlkens.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/geziqgtgf.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpcjaidvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gucnjtbpc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/grhfozomr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gatvzgsqp.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gohamelep.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqglvpdvl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gncueeqao.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqhsyhudp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glfrkfuwy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtvnlqlax.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtzaoorjc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzrmtioaf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/giqxyleun.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ghnfmfhii.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gaasoijez.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/glvcwhlan.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnymcczse.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzfqwtoul.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gxswdgjyj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/golasmszg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gicsjsesk.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/glmccjfrb.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gnagflkrb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gklcjdpgr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gehmcbdxk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjoufxuof.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gbsuijbgg.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gghllwdxc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gfyvipuwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gfzkfslyu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gxwibupxp.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/glawumaqv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gmukiepdy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gvtiprxjr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ggzfrgock.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbcdjtepo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gyyxprauk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gsrxnkhbm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gzwcnhflu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gzjvpjdpn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gzvzcyteg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gwcfsjzjx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gfvbrnphl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtxlusqel.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwxzttgak.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gicsoxugz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gqcimyrzb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gspofmjov.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gzlhowbea.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gszhdlcdu.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gcujwjjrt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcvdyeodu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/goaghdvmn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gzzkjzkcm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/glrirwwgb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gxesywibk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gcksvhwnu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/geyqaokcl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gbvcibowp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gdvrhwpos.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gslbdmpsf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/ggauiljnt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gvkauzzgi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwzkzejak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjvfwovbk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/grnyeeuij.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvlwcemez.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gzojdkmmq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gxdrzixzk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gsiobbada.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gqxtakrtb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/glhuhtmfu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghmfpfyni.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gsbaiugil.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gssgulmeg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjgbmyvob.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gejiqqyzn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/guevzvpvr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grerhoizj.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gzwdaixar.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gmteqgggf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gazlzbkrq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ghhrbdxao.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gzpkbvpee.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gyfjxdhcs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gdjpsiuwd.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gpeejtarl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gntgtdszy.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gmucibrtm.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gnmzknvaj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gdspghuty.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gdsghifqw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gfyknmhwo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gitrhyral.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/ggqyhiqmm.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gkvbkwioh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/guqzailqt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gvinrglqf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gtyiobdij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gkyfgzilf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gyibcnfjg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gykecwhtm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/guqglufyc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/glxtbuyup.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gekirdijo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gysdhcwxl.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/ghiyqssqq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/grohrebge.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gdxkdcjvt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/glzhsxbrx.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grlzkdlyz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gczstiyev.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gtoiqzcek.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/garjqcbpp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqrryldxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gzpgonbbj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gvtfigbsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gthedrmha.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gycrzzavr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gifqybxma.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gideyphfd.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gostdvhcj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gotkyedbo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/giwgxhnzs.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gaacwjwln.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/girdbmbwr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/goorpivhe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gpqjhignm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gpnvfwsjh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmpzlebb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gvczybmbd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gybgdxskc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gwheyjipx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/ghzwbpcbf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gtldidadi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gpdbsezno.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/guvkgzyww.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gkutbmhff.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gasrvwdjo.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gxorbtgio.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gkhpjewms.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ginfjpacf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasxfggvj.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gzyidfqdz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtufbdwbk.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gykxpnhoh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gibzbyowb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvhevpohz.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gdevnlscp.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gyqkrtdql.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gpaclvaao.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gfkxolokx.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/glekkclsr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gdkhldcqn.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gxohckaeu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/guywmcpbk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gebntnlgm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gmmqlagsv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gxyrmjiwl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gxbmtpvld.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gxqpdqrvh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/guicrfnxr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/goidckgvw.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gaqwsbcft.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/giyyocdga.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkhjpbskp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqbyoal.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/glxjnclkv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gswsmqeca.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/guqpxcrte.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/goohncsyl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gjqmodjzm.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gldzbhzcu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjwbhxeg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gamlmgvfi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ggegnxcch.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/ghwdeamxx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gudzwuwqw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gawicdzpq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/glxeyzvdc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gwbttcggt.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gprheuowz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/ghqwondfh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/guhxsamwa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/griwfohys.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gyodikvsh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gvldpgvom.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gpztyvhwv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/ggiiwzwck.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gxwvzwqvv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gjmimeoqk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gryvhvjku.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gbyyswzlj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gemestmat.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gjtuisjym.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gjtiifndu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gzumtdnby.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gczrpoxcc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gdmgrkyqg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gqqvpqobr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gkgmvrtdi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/grevyypjj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gyuzzcntw.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gnzpgpwnj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/goivcezhu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/georhvxiu.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gyzzwpfvn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/ggdwcyjvf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gsrvpolzn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gggbpojkb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/getawulgb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/glqotfcsh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/guflktlvz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gpaxfbdwb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gncocqcht.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gxdyelnzg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gqtyjlhmz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvsksqdwh.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gldisafgi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gajncqlbd.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/ghcwbgcxf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gucjhoklf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gwrxabqod.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gfgqqltfl.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gqkzamava.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/ghssnbrwb.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gurmxewpz.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gqiuubjdv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/gtoqarzon.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gndhbzrxi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gvdzszezf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gzjpcannr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/geeppevna.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gagdiemmh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/getasaypw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/ggywpggmi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gmfiomlkp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gfwrabgma.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gnsdemunw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gchzprgmu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gamwsdltk.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gmbubzyax.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gnqvqpbjr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyjbtvvgl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gzczowvgo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gpahspuaq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gheahzmlv.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gaktpzxky.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gfymzagas.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gqaaawrka.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/ghrpxwvic.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gvhnvfcrl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gpicvdgaf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyvydhaa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gfsinngbd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gxrokudtz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gtudpyjws.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gdufllivp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gftgvifgt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gpnwenkwk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gmzlwgghz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/ghgqyqsjh.sHtML


<!-- 参考信息 -->