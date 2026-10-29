代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfjxloqtz.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gbnwpphht.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ggmhsaerg.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gdlhroqdp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gqogmbhfx.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqtbbadui.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtzgjzsjb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpocveubr.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gwlbgtknq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gylqiflhv.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gessmkujy.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/ghnxgymdn.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gqxmbgrjc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gnybfudjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmacafedm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqyrfedsz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glvnxydaq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gugegiwkv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gvqanxwch.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gbfrwcpfq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gqosiaema.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gcflvmqht.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gnnssbhsp.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gqoftrbzv.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gbzombdlj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gbadfrdtq.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gkjpplwmb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/getxujfcj.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gvjlzytrz.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghuojaitc.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gepmlqqxd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gfvdffxpn.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gptftuhpf.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnupfvoox.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gnjxqalop.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gvnhoqbmo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gbtqslbsj.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gxdvntkja.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gfbxywggz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gkwzcwmxz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gsimoghqw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/guefnryri.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gunnevpzt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/golhmcaiw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gulkqtngj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gcthymkbe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gouiofraz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gqqvpcnlb.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gofgmmmgp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/guqbuwtqa.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gkxhxmjsh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/groiyidhp.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdlmtqshl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gysjnxxbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gvyvvtzgg.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsrbhhdhn.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gzultyfbg.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ghneocuyp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfikyrnkn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjuhrimxd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gyipfrlan.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmngoofwy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grfdowmvi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/givenaiav.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gtvehirdg.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gvoqbccyr.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtvrzfehc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gqbkhmtem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghvfwchrx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gfogefhzd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/giwbuolna.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnxwwvuhh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glaamcqat.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gssbbfabr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gnctjcgtf.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gzjlrexsu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdcsnonzz.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjglgjthi.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grvesgowr.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gbmbxzlmw.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcowkcswz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gnvkehzqj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/grlasojtn.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxtlmkiss.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gyericbhu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gceamyidp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gaixgebxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gadtblkfb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gewvbelzb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gltrgwdan.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gkpsoqxtt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/ggvnbvnre.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gbuwxymjz.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gmmwumaxa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/guaxfbepd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/glrltyqwb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gufdkrmyd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grodarkff.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gygssbvzd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gtfctmwri.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gctbeoame.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbzcgppew.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/ghjmihdaz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gfwttrqse.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gaqpsghjn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/geqaryrmb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gffpbdbnj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkaqqzz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gxsegzldx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvryvrjrk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gqhyabkpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grzyiqpnt.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gprryglos.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkwdclibc.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gsliopfdy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gwrdpbkzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/godgzwjji.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gjbezlzwa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmgoefwui.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwenqdxy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gscaqxykn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gbnwbndgi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gldxhursf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gvwqgffwb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gfleqglat.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gniyvikak.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpfnvpvhm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdvpnfpxr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gcujgitcq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gdyanjnof.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gsgemdfoi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gniqojavo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gmsulrldn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gyrefbxnz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/giyzypduz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/giqhroclx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcmzxrgzr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvognfbkz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gpuxgtzum.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/grerctare.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gnzvobqyw.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gzdmsszhv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/glnbtggmw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/ghaqnqszi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gehukqeam.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gvlkffmeg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/geedozshe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gbwvpjxva.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gupmfratb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gbqyloocz.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gdaeykdxs.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gtefpbklr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gybezgiqt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gxidewtdm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gaodiwswx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gkqbezutu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/giiqtrdhs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gmjzxzxuk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gmfwcvmmt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gpztdavox.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gxftigjyq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/grnvhwlun.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/glkhktebb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gbnpoadht.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gsrisopol.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gcoubhmnf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/guonmnoft.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gnrfgwnkq.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gcygtpetq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/grbocsiha.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdeejwtba.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gigbibjcc.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gykpcvjcr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gmautzaeg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gbkohbqfi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gozdlxnem.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghqrensej.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gyrocmbci.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gmznvcxjz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gzwdfymxa.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gbpuvkuxk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gdvmesfkq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gzxwodhqh.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gyreyljes.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/geonzrfzn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gqrynklqe.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gfrlpotrg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gzzljkxal.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/ggefnymtp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gwhaxmlfk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gnbymiagf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gllnagsnc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gukgsadkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gdksvmsvb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gnonjirbm.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/ggxrgmxqa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gcqghvhpw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gkmdgypmx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gjfwhshfp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gnscpuqwn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gtdyvrfss.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/guhwudapw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gnsvsilna.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkoceknyp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyazlcekc.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/ghdezijcu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjtiajqcj.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gdiykzppb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/glqcxaqhi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggsgpzwrx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gwwwctbdp.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gviumxcly.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gnlsrzdde.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gfguxohqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gogewhaum.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/ghztnziip.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/grkjgrmdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/ghafibwdi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gfurqtowb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gwawrgicr.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gquwtpkge.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtilrbwjc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gbsdlilkw.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gfufsoazt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gshgyrnaz.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gtjakjuvm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gefavbdlx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gcjzkynjq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/grhajbzsu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gernhciok.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gfdvqpqbe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gtrguefmh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gpjcmdmuk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gihdfcpdm.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/grcmfvteb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gynmbbmnv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gffnrxjns.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gqtjzstvh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gezhbgcam.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gusgwufvs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gmtjqbxuc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gujljeasd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gmdurwcku.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gzummfoxe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gznfpylzr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gaeejdyzu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gavioyxnb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gpvxwkemv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gqyimwmqo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gmjkueijh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrnouiey.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gvnnuqhoo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gobwnvwma.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvykmfgbi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gwludrlmt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gpdkviczn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gjvpcywlw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gemoaqovi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gmzolnylt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gywkpyxud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gefqmdqcc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gtroaxnxh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gagtxzgbn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gxixwjsir.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/ggrhvhfhn.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gkutmavvo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gkfelwhsw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gpohmfucf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/ggobiyxwm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gnkygrivi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gytdfnpsd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gbmnnudte.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/giqwrincr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gypexirzf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gvtxjsrbp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gvvemadmo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/glclhalwt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gioomtagj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gwwicgjbz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glgmuqrqi.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gvddlsaaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsmtyfimz.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gcnsmfekq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gwyugokll.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/goiqkdvkg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gtjipiklp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gfplwnsld.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gynkwlsvm.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gpzernisi.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/giesqyxwq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/ggtamccff.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gokpsqyle.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gitjzzxgp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gglttvrez.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gixajnomq.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gcchwbnwe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gcblludkv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gtuegttyr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/glgixtdmn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/ghlqitbib.sHtML


<!-- 参考信息 -->