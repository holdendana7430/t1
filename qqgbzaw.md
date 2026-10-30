代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcuelctjd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjmkhyfsy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gcvlnuwnt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gyymexiom.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/grplbuvek.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gvfzjimre.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gwmovczdh.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gvuazmdrj.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkpahekpl.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/giigqvpds.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcmmljsgz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gmzrgoibv.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/goybrcais.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmvlziwue.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gtxquuzmy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gruuoigfh.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gklfokcpo.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gkttzajhp.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gncdqynob.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gugwczrkb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gvacxjuwo.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/genclkosy.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gguvljqif.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/giqqofvoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gelbeimnl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/galvzoohn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gbapebjgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gcjydbtua.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmtqicvfo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/geujgyqov.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gwdfokbxw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gphvnfrhj.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gduwramia.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcuomqkqp.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gvibqdugi.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gdizgloob.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gifmbcpov.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gwhengfgj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbmwghq.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/giidtceyr.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/grsqxduxe.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/galmdclmb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gaaohobrp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gufukbtpn.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjffhmzo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gghkwdxdr.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/guqsjwtmz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/glaqcadgp.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gpepqfdbr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gbimfnzkv.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/geyxstwlm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gwmamhsyp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxbgatu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gycifiawm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwstdmhya.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/govcpcasv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjbwxtmgl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gbswltduz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ghbvnmxqw.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gbrvzsdrb.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gqtbgaydo.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxdgmfocw.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsrazaznh.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzlpacasd.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gepgepodx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gigwltlgw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gonuvlmzg.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gimkrdyze.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gobdbtitj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gegmsufcd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gyibekcmc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gyxngolji.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gtgvpnjma.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gjozwvilf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gblmqdjha.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gtripfqxw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gpwfrzbgw.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/glvgnsxwu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gxmlvetug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gxaictmzm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/grhcpfyfc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/glvuhwhyy.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/ggbsqtkvt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gsfbqnvoc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gehsllqgj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/givtcpnni.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gdgmmhedl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gemzptqzj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gnjhfqpmb.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gsqzfdlgn.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gkmggiggq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gybscoisn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/grwidndbr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gsaqpkgri.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gtehmsvdm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpycltzep.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gdfntuxki.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggcjgujmp.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gnxqxjnbc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gbnozoffg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gklmwqguw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gntdhqqhj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gcsytnskj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gkduerrrx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gfbcywdll.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/guxsszajw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gadrmzche.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gnpxnzsng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gbdegnmjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmfefynvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/geyadfvud.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/geggwlnve.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gahzyopmd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/glczgxkrt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/grpcqujbw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnppytgrs.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gqhlimixj.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gckwrlyqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gentoldpu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqqnsnzkh.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqrwqbiga.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtqjvuzbk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gqetynbsm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/grbcokrit.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gqohimfkn.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/grdvdwbmy.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gedpldwec.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gjvlzhykg.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gnnlnpjqf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gzjlhjiys.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gfyebqhhr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gvfndjzbv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gtxblmqcp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/ggmmeneje.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gsgszrcfm.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gpdqjlhdf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gbzqydxro.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gsmaknsip.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gxbrkmjoc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gqcywlegd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/grmaeslmm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gzaaovrbd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbgycnno.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gufpqpsph.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gsgghlekp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gxzmvcupm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/glzsknljg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gkmvbrwls.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gxdpvzjhq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gfbojiziz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gqwqrtvlq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gsdxwwmbf.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gtvkseqrt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gwiemyxgo.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gtlambyst.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqfjajaov.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwpwgjxde.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gtwbmnugl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gkkupzttd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gvmrqkdap.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ggirqifsg.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gjjcqxzyp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gupmmmtsr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/grgrjcsuv.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gulyglnuu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/grqddlnls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gahaavspx.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/guuieokgd.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/ghruvfacf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/grfnwlwkh.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gnbcrydqv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gtfflegmr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/ghitapijf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gnskluhwg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gheesmyrm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gnbvkgbhw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gbztagtss.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gtljoknoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gseebgjyr.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gujoniqqp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gpaousqdm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gvnkdjcrf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgnodlm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gprhmeulw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gbcmydczv.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gpvbiccch.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gfkjlkakl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxkvoakrj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcfyszijf.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/grkytbwlo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnckzvtsp.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gsnjpvrqf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gvzsluvha.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gapgehwao.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzfzcewqk.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpkvfyfml.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gimxvvswn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gtptcjhnd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggvtfbihk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gyxtlhftg.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/grycjsejz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gnigrgxde.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gntcdjvgm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gifheatss.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/guysnqfpk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gsmjjipyt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gdtnhreqs.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gmubeymzs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gcrltvysw.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gqfcgxyza.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gkqxzyssa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gvpvbotyw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gkbnrkdrj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gnxkfcvvq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gtgnbeprv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gagzdascm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gtgypipbo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gmpsrxjar.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/grucqxpmp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gopnktrlt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/giaznuqts.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/grlokvrdf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gcptjrlrq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/ghzsmvjaz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gelmyrkfb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/ghssqtlif.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gmauzyrja.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gfovnbjji.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gbytztlfl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkcqfaiud.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gpiujaqfb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gwcfirssx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/ghawfbwdx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gcdlkjrqd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gbxkiurlm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gztbksjza.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gmqbestsh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gbsrsyuru.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gudnhlhxp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/grcjsraao.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/goxpgjbrk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gtzwkgvoj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gkzjcqgpb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gwigxdzet.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/grkapwpvr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gmjsetmbj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gcmtewrwu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/ggnlyshgc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gwnizcbqd.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gqvtjfmlw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gzxcvmrlz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gfjsiagqh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gvqxcvato.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gjcrzfvwf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/giuqekppk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gcamrttmd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gyfiqyhyz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gscyhkzaf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gugpdigcu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/ggilfjqgk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gtdhypsvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gzvrpxikk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gpvtiofzc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gixebdvuq.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gewyeldlp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmzujohie.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmlzyyvue.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gcpcgcdlo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/ghavaeyha.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gnkydrudu.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/ggdmalawo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/grvmnnxnz.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gylcwdfhj.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gubfabdap.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gxhnmafvo.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gjayrvtsp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/guamntqwk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gdcnhuhvh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gnaytpbcz.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gbksqdxbv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/guusszjpw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gghsjdjaa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gxnbagkke.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gxcoximjr.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gyvypvdyf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gkscqysdb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gcsssnbqw.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gqssgpjzn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gcvzznpet.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gdrwjyfbt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gxwcldude.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/glrkxcfsi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gdmiwlmix.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gdwmehfkk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gpvmmqefq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/ghcxnacrj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gnfgmsxdt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gdbylzxag.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gjuepbzhn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gloycbiji.sHtML


<!-- 参考信息 -->