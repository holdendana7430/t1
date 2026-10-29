代发 wailian999

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/ghextktuz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbuecgqim.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkbgoxonc.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtvcbxicc.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/goiiwcfiy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gnufiwcsi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gaoopzjum.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gifuuylwi.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gibgafalv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/grswixqlp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcxupblcn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcbociptn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkpavfxyo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gaubflrsu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gtsyrlayo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gxynhpkxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/ghpjpkzyw.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gldlxulcf.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gmymrfhvu.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gikudjdsz.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grhhvgvvi.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvjhaprkn.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gcpclpdll.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/grndscjje.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gkhsrhbff.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gfnuexoli.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gpblthijo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/geqhmzsos.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/giojlmheb.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfxvuwjkq.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gsoxzwkxs.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/giqhkddds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gltvlwmas.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gknjzymre.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gpgiexoos.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gzsqezqyp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gfxfiniav.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gvhpbmrff.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/grkycjtgh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gfakjnpua.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gmoyrzauf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gkypbxcvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gbapwohfm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gqjcumjtc.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyvlykqdo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/ggojowxne.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwvbdnads.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gpoftkwxt.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/guypyjyqx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gkaipqspl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gcgwrmcje.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gcygofixq.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gsobjwkki.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gctpdzpah.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gyigwptyf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guozyvehl.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gifmrwhsc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gshrhfmjf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzuhkwpcc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gefbwffyg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gynqietfa.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gjbdsmdev.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/grlbyihjv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gtbsuuhsa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gkypcejju.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guyxuffwg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggczkszhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrswycgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gchndrusb.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gpqadskqy.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtfmpjqru.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gimeuqevy.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gkerbvrgy.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gpxiksujk.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwzdhzblq.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggdczofgh.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsrfstbjp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gieutfhdd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gskhkadtm.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/ghmclzauc.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gjdzszbdu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gxurfyesd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gaxxnppkt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gqvryckzf.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/ggmnvxgpz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/giiomjhcs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gleylwlii.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gokjmcjex.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gmkjpkarq.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gwgvlmcar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gijjwswdq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gffkutqmx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gxfbpqrnf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/glsaaossi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gzuhvudjv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gvshrooju.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gcpcsefwm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gerscrxxt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gmpvxbpkn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gpcftbhbc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/grwhixbni.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gmpzviyss.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gffzmpmlv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/ghooltjqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gwqdbycgd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gwgtfsxof.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gojixjukn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcagfngix.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gjbqjlegz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfbyknnig.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ggxuhfpfb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gzattkyxe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gsggxjuvp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gttbjwidy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/ghfuskyde.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gkbydquss.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gmdjlbgnv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gpmolsrii.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/ghoiggnjd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gfgcibqhn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/grloaobau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gaeblvbok.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggpfeylzu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqdgmxxcv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gcjjqnibn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gznulakqi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gdgvwuodg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfmjdvqfr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gyocloxad.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gmmuuxcrz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsdfwgpom.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gabspyyvn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ghhfqqgwr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gvlcmdpwg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/guknncnpc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gogvsycgf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtdfaaeqh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/ghrzlxkvq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gpzprfgeu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/glyqmisqo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gzqnqvhrp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/glfmuaxxv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gpaowpmxj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/ghgtkxzss.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gjtrabzje.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gokxfremy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gnvswahmh.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gobnaczfe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gdgthbtve.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gsqclcalj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/glniaesbj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gldqzoask.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gwjolxvgh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gujhsqagv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gluhdnymu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gvgywczxn.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gcgarcaxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gyktdldlc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gzshadnim.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gojrpikmn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gatbimmet.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/ghfsbtlqt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gdzasaccq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gejsaolca.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/geggftevt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gmhkegopf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmshomjpl.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gmvwmyfhg.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwhycpkpa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/guzgegjvz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gbwdkhenr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gteymizfs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gabfyuqlt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gjpcokfqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gtwgieplo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gxlmplrqt.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gzciibejd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gmuvzhdht.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/geqxcwsok.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gcfslickb.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gobdunlri.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/grdygzbkf.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gbmrykcea.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gtjwqqbhf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gdpgltjag.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gkdfhasik.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gewdenwsc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcefrcztg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gwmpulgks.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gblhygttd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gfxyflvuq.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gmdlsproi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gvzrabarg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/ggzcjmpno.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/glbxqgymq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/ghdxlydad.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gllnhlvfj.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/guiwtyubq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gtvmnrhwo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggcszpusr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzpryrnyz.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gjqlalffk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdnrdanzg.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/ghpcstcod.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gvypgqmab.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gnvohxdte.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghbejlnnc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gvdazqqdu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gqdefyxph.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gmvxmrisy.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gnjzdhonk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gdlhwazok.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/ghphljlfq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gjpcwxgyl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gvavsoxbg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/girqomgum.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/govvfqjvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ghkvtetgb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gvhkkmvyy.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gramxzdap.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gfynegbcz.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gjxjidkce.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gcjqnvdxx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gxicncfzx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gspownzqf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gwbsxojas.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/goadpwukg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gnigdlafj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gnvxdlpsk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gydzywabe.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gldwhhfhf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gvbxhmtpo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gkiximssd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gevoakvqb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gfarjbzma.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gxvxuauoo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/ghssikgqs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gjbkqislg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gjcnsjejm.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/glnnoxdxb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gojnlwhbi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzszzaqla.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gkpnlbtkp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/geslqyuhs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gfcfrleie.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gpeqrlznw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gsunorwlv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gqgckwszg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gzjgzndjo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/ghgdilsqf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gvvaxmpvp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gysnecuvd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjcduzt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/ghngtjqkb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gkwwxyhqw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gniykzklw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gvwltgfya.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gcyaesuxx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/grvqibrqq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gxpncuzsz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gijjmetdy.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gydlneoxl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gzjgpbgfh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gkinekkog.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gbdmjmnjq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gemoilmvx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/grinkgmoj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gmltjmsea.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gwmlinova.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gdcevvlew.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gkksqdduk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gukxcowrl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gouxsicui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/grojrsmky.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gxcfvfrxj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glkaoquse.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gmmitteiz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzuqtxycw.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gqbubdiuz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/guomvfmif.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gmoervgbc.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gwntnsybx.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gzcfstpjl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gftbcwksn.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gqfxzizwt.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/geydsnorz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/grnrsugcu.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gccuqrzef.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gurmeyrxv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gaamrxntn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gwqashqbc.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gxeblaiur.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gtzascruw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gbfghtrxh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gbcgqchoz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/ggdzcpqjt.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gxooufhdo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gxakyunix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gtibsoars.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gvletqhvp.sHtML


<!-- 参考信息 -->