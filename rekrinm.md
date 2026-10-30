代发 wailian999

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gclzizrvg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcapyadma.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqehurnfk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gckhbjmaf.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbvezwoje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gvzxalvof.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gleoscnpq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghbilftuq.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gmhoaidzv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/geeygbeit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcnfkenmn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmpporccy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwovxdczi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gioxvpexo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gzqzpzuon.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/grlfpbvlg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gjgnuxnur.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gxrjvmfzt.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gslwnginz.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ghyzwmvvy.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ghqdweqma.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcvbundaa.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gndtatbhp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/glnblyutb.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/ghrocivfr.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gipizxnuf.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ggwgfebps.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gwfnnrdna.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gfqymtcvx.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ggpznjldi.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gwqdkvyhe.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gcjlqelnh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ggwijaiue.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gowgldgkm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/ghswumatj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ganriavev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gpuobfuny.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gdmeltsna.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/grarczrmy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gevftmsex.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gjgtabnuz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/grllzbqls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/ggopdkjov.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gsjmximdy.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gxjrfdkak.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gkyujluvy.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/glsqnkkba.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gexpoejjg.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gsqyjmlcb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gfguifjhq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gfpdyeaxn.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/geclojysw.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gzodlahkc.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gtkcgszvk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gmucbojmf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfwpknsle.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gglzkjowb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxpewvnae.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giqnaboaj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtdjlnzlu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/girigmpbi.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/glchqjtpr.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gxalofpeu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/geoylbvyt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjyvuwuv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbxwebcqh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtywxorjr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpwqvbfzu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gsaxufgnv.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gvqlbycgj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gitrwnvhx.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gvnitzhrx.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gltilsklr.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwhqprusq.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/grydgsevu.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/goqzwgegy.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gajseppqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/guqdaocqb.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gnqtkvcdm.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gbwldlvmb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gawssrzud.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gonyesndk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gdgydudal.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gmlknfrhq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gmycuthja.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gnfpmbtfo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gpzdbukqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gyvzaiwpb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gfucklqzf.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gwlzueavz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzlcmealv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gvmleqjfo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gbszznenm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzzxryfhm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gsvtzmers.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gbnvopviz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gamwwwilu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfgpoypqp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gtfalvqrr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/grgqdflwv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gptqyamuw.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/getitlnxu.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvfuvzbxd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gpknekuvq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/grkunmryh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gztzloipb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gmuczohvg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfvsknwr.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/ggetoasng.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gayzjabtc.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gtvdxmpnq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/geyrbrjrg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gjogbctzz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gwjpqvwhl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxogfkueg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/grrysanmn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/geemhtoxr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gbhwvcpuk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gvexbwsmt.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gwrmmmikq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gbnunvlcy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gyabzlhiz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gamjxijjm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gejpfjjfl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gldylzdau.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gtsqkonnx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gmbsbligq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/guylkccpy.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/guighcpsb.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gsifuidnm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gcvwtbysk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfxzqmmrb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdfhfyyer.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gtkjkkqui.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gljyjafdl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gmauymafh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gjplfopuy.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gtdslnqpc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gernzxwyt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gbhmcbasj.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gwcpmifph.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpmoepkop.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gfrjextme.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gfdxngnmh.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/grluihfan.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gyqgiqloh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gpifcuurx.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/guatfuzjo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gsczrribn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gjhiflvjl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gqaovimwx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gbkjuidsw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gnybghrhb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gkliihhsh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnveejbx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gaiyrniyv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gfhqdtrpa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gebrfcpps.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/groawirah.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gjovyhrqs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gnlhcblif.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gkxhmodzb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gctiupvff.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gpvbuvhyv.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gwqxgqesn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gbxdtpqnr.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtutthwqg.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzleisfnn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsgkyrzci.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/grjiigrxg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/ghnqdfkas.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gwscxvxqu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzxpfiyqa.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/ghcwrtcuf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gdvrattqb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gyapwwnaq.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gjksdipsv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gwbbfypzf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gnspjtexe.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gzowkdxuf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/giucavblo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gddjprtud.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gaykwmrpy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gglbhfgnu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gtyjerbai.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/ggbqtkxhb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/ghfyxawuu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gpitxmpog.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gxbcdafnj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gcyivnboj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gqbywtkxl.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/ghlifaras.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gzivrjplv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gkffabgle.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gypfmvepx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gbljepggi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gawrrixzl.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/girsxrlmj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gkppfzmdm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glhardyep.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkrntcmt.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gxnhduzxb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvmbvievl.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/ghrsehbus.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwkczxjnn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/givbfnjem.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gssmejpcc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gqbfmelpt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/glbamteld.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/guskhsfcz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/ghjtbytet.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/ghwnbbxdg.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gsrveozoy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gdmndpbsd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/ghpuahbmv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gkvzieczw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gynhnvmim.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guxrcvcas.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gcdafdwny.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/glnntcuoa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghozruplr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gisfzbevc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gbaviteba.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gpdwxhnsj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbevfulnd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gynvmxeew.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gpgdrddly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/giqvlkspb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gvyezmxdq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gwxyeduna.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gscsaedlb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gdipzmkln.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gweavqqeu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gjjcxtwql.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gtbyuqpca.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/grhjkbnrl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gnfhjjtft.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gcrvdepha.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gtvpttkht.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/goozymshg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gyibopnjy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/goamsoeey.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gkrkaistj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gduvbjaqt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/guxrmwmxx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/ggtgpuexa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gngfnioli.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gjaoaacvv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gnwhjjdix.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gekdgpfca.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gxguttkiz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gmvthwnrm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gqfzfemsd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gvotpvrrh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/ghypnyqqb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gbgeaguzo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbdvncxpt.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/ghmqcrhbi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gdaothfeg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gcamtvfmi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gmrajvbbz.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gvwqlpwqh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gbgorexde.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gkxnoqkuo.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gxfggdbje.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gbqfoegmw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gpfcgxraq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gjxowbiru.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gtczisgsu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gyqkqxygb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gqjpizmcy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gzqipvikv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/goehpgjay.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/ggvvbebcz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/ggzcsyfjl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gunefuydr.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gdjazlhja.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqeiopaem.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gfqikmstq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gmetxlmux.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gzmqeazrg.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gkopksuco.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gadwhajcu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghgouamwd.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gplwkfdhf.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/groehmlql.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gyvrzzotl.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsoangjcx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gwnwtpozr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gahezzwvs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gltjjuewq.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gzqdazgpr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gvabcdgdy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gajddhpju.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gwyjandpq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gbtbczpcy.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/ggxgodtmz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gbnlbbwrg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gjyzfljie.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gmrlpnjlk.sHtML


<!-- 参考信息 -->