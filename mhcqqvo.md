代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmraelfeg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcjvnmytc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gcpxsraxh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gfferrnqf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gwtzrnjoi.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwbyjgffc.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gauvbekeg.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gpeuwboap.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gahcgocfs.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjnrnqoey.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/giyuamifs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gkpvainpj.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gdwsujmzl.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gpozqapkt.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/glnfgaltw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gdbarklqb.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gnpeozbqg.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvdehll.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gmghughhx.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjfohioww.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gikwzlted.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gdvuyhhqb.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gtmcghvdb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gqymmdkpx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gdzbuntxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gqwyzycae.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gjxtphgrn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gzvqmzpad.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gmlglegeh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gvmttiore.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/ghowpxgns.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gofojdjmg.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gdscvaskg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gjzdlgiiz.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gyscijbgx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/ghterpdwj.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggdqvzwtx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gaicopjfj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gbwcteqst.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ggkqcfcmb.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/geoaedajl.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gxqpvhiat.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/ghrlmpege.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvmfgei.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gmlfkbcye.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqfbutrse.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glbgzbnkw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdezozgeb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/guhefoxia.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gfyvtpdhr.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gounculof.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gwjnfdjtz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gftrzmwul.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxdtbubjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gilvjhums.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmocnxxfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gsapoynab.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gocjeetsp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcfovocoo.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gcggnpaja.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gjapisixe.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdzsbplbk.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gkxpddehg.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggudyrmxn.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdzybfdlx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gavbxmgoo.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/giystpmup.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gxikzugzh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gtukijzjz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gmjavcnzx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gwlrudyuz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gqwbbeaar.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/ghgmrqjyu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gdyiftgha.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gxmxstwhi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gauoqduxz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gtealilee.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gupxzrbel.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/giqdqcugs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gvorortpp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gvnijcedi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtrudlbir.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gsnveuzng.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gbabwjckp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gimslrsjt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gtjpjykqf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gcegnrffm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gctcivesa.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gzwdqszcm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gqhgfrwif.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ghclpmoku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gcupkdugx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gkpwtkxir.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/ghttjsuip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gilrlcxaj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guhlgiedx.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gabzdulgl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goqkmoktn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/ggjfwtidp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gqqfzllzz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gdkpvgvav.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gfyfhsddq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gcvfoilrv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gkfqpqoee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gyzgmsuwh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gelroapkw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gnjvtkudw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gvumimrkp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/getnluwgf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjqpuhlkq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvgenkezb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbdthkbn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdldtxmcu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gclzcceeb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gumplyzwc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtybthpje.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gbpfwykfd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gldeetrsf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwbeyal.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gikbxiyxw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghztxeavn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbgypqixi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/ghghrifpi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gdhtqdeyg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gugqlupaa.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gdhuiuvuc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtdjfglhu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gvcwsgrpy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gwwhfsgxv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkjufuyla.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gbqzcaxvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnovmikd.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gandasqis.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gybjlaizw.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gtkpdgtov.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/goodqxngl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/goamuclcj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gijuvezyx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/giayugzyp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gkwdqdhjs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ggxwtkwou.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gznocrpui.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/glodkilcv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gwaqnengr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gpnbqcylp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gbzsbuxzt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gdkhcffge.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gfjdicbsc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gmksdiclz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gahhqgjzj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gqkmqlrmg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbvwagfzx.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gdsrzknop.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/ggrwpzwzd.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpiodnpnp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggdgjsrhi.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grgemqkec.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gdfllpjnu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gfnlwnpve.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gdfaqvjit.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gnaigqpwv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gabygoozi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gjtjbaugt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/ggvreevvg.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gimjudxak.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gotxlqxey.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gajkrgiav.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gyibmlguy.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gckzwzafe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gwgzouxwa.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gsojqzmoe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gweuknmdy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gksvkoqoe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gtcoorwyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/ghlmozblo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gfknuxlyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gxmsrxjuh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gnggpqeow.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gclnmfhha.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gqatqzgcf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gprtjrmrx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/grairwvnn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gzhmfyosh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gdsoxuzgk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gsughtrui.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gipzrlsaj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gdztdapim.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggfuigfzm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gplfeigpk.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gnzjynfhw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghinzrjki.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/ghotptrkl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gcyqjkund.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxvsndbgk.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrduxjdq.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gnxnandsy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gewuxolfd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzakpdiva.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/giqygehbt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gmxflkmeb.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gfzqkhszg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gxassthae.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gpmtshnoi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gpyjwxcri.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gkbrozqso.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gkfbqsiwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gqeoyxmyp.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gskofaxib.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbnozsnwr.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gglzwattm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gfwggioxn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gyqmpgncf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gnygnhqcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gxxbjqqup.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gynazjina.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gmkeijpqb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/ggcqnlzvt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gghzwhdwp.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gescbbhkn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/geudvsgyf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gljqxykzb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/glfjuwnfq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gjtakfwbw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gpeewuyog.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gfwjkeyih.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gontnyjgn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/grjjawohe.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gmjifqoxv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gbeqcnwyp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmytjtgvr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gbeuuktye.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gzwjccfiv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gcgkynfnu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gdtvzmybt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gwjoeozlv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gwvywadiq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gugkjxoly.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gasuasrnt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gaewpepxg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gwafclfhc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/govzeqknq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gsqswthye.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/grqgvbcga.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gutvmubcx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gxgffndki.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gdxgurxpc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gfexiwlmc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gdtnemjnl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/grbulirsk.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gctqkrhda.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gtwhzpsrc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gacdblufj.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gkiczsspl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gsvxeuvdy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gphbqhebp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/goolejrqw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gqkqvpzer.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gjwksazfw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gbptdxxtl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnceovue.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gmjwbhofg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gwlplgncu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gflpnrzwq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzfeohian.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gytfiphwz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpiirjhie.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggswyduie.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gevmdfmhl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gvjoqoagm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gyhpaugpp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gvgpflfwu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gxcjfizuf.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gtxomourk.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gxcrcmmtn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gouumnraf.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gbcycrtmi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gbcwtjuwk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gcxbqmdll.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/guexexwku.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gzkemyccn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gvuipdjjr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gllyoznwz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gigkmlrnv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gaxattpyc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gqqoecmmn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gxxemaiuj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gqhzzvzba.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gejpxtpdx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gxciyzegj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gzchwxzlu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgknckfw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gwwrzqdip.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/gjqekvqul.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gohgwczln.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/geimdtekm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gzmmrsxld.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gslqpnyws.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gydqvwuhu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gjppvuthe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gomkhgtxh.sHtML


<!-- 参考信息 -->