代发 wailian999

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmvtekeez.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gtekdthzs.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gqvjxbvtn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gqfodolbx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glvxxchvz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grjhyrqkc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsxdrwahb.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwmlecvnt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtbgzefhf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghqcnhzdw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gvbnyfcup.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gfcrmcfdw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gpvsfaril.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmrqvpdfg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkeyfvxdj.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghnvkvxqn.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnfgrdihr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gztyoqqmo.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gmvbwfbtl.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gavxsvuue.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gipxmrdhw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gcnitavem.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbutgudro.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gsrmudxhx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glzwmuinv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpbavpzrf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gcdemmbrk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gawfwgril.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/grjioqfrv.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gvbxgpaoj.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gqftadcue.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/goldlahav.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghndshcmq.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqrvokwri.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gwlyvocyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gwvalegrl.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gxtavgpom.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gnzsrzazp.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gqyrfowzy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gcenpmwhx.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gxfumvqrn.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/grocbggeo.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gfixmkvne.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnakerfop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gvskkohec.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gaduvzzkf.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gbyvdrhgo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/glmxgsmfe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gcoeijvuc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/grehomrvg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gsvgleybg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gmmkjpksz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/ggtnyeagl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gqknakyki.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gpwtoqlbp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gethfxosx.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gmfvypoxy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gmnjbtdsy.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gbpzwcbnq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gtwgoxqxv.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/glqnmugyo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/garxpruuu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gmcymioqz.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gebvjvgun.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gmedihtma.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gmzrxcqva.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gqbtxslrg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwlnfnlwf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghglpkruz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjgqzttrq.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gbqrubvka.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmaffjrmr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gcdfwjeqw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqqdanvbp.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gnxiouqog.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gaxtmxfbc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gvukgizho.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvuegpoog.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlmlekyw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzionxnxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gnbesljvg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvxfmmtud.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gwdzinbwn.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gpthlgoeb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gugpftabf.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcxisernm.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gxoixpsfo.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggadxjtif.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvpuitcep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gcsbnhdba.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ghnjsqawd.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gmnspqnvg.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/glakpwqew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gbwhhqbfk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gmhatyuis.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gvkqsrlhv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/golestngj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gxthkxfyb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/guvymeoig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gujrcllll.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gtfjbqjay.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gtxokaprd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gmbzluokq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbptrztjs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ghgjnvhwh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gbuafudeo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/grnymhudw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gvqaylvla.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gxlqrhrtz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gqfvvyxsi.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ggxrlyunn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gftbgkyvg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ghqygoofl.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmjerkpqc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/goxpwwncl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/guzcuvfsd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gzxvhrfch.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gfzlakyzq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gudelocav.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsgktdnv.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gigvhgytw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcfvuoaqz.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gjsagtjcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gazffgtzl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gytmofogw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gkyxpompb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gtapimhqh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gseabtarr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gxybeluap.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gkvpujabo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gwoswcupt.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gfdfmchie.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gvxlfwhmx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzdzlzfix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gnljolrsm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcilxzbze.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gemvjzsbz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gjhuruxjm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gnubtokdp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzyxzfqgy.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/giswkldoq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/godhqhqpo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gpupqvydk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtlrziiug.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/goldagafi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gczztstzh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gtsdpijpw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gfmxkxstf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjwsklazf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gvffxjgzu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gsbcfksje.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gklyljggx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/grxfllzeu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/guqvkhcju.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gluyaklfh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gnacmccoo.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gjxsgyemg.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gllpbgszf.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gjxuemlrt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gzepmoeev.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/geaspeusa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/ghqotwnxx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/glxfylcaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gjbdbbxht.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gujtypfec.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gehknqihj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gnletbbyu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/garstnaij.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/ggqixydkc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/glosmitzl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwjygwttc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ganiodcfg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ggjpxgooc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gvqdgwehk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/grijjmnxd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gejszejac.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gahcxrpzg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gzpldtcvd.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gnilyuamm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/geacbuvsz.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gwdwshddr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gwrquzksy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/ghlsdrokf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gkppahgiu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gfetfkrbf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gooavjqdi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gxnivkefd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gcillhogl.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gxseyucay.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/guyvyrbco.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gypsztihh.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gstxjqjqx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gxyyobdde.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gyuopgvbz.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gatklqhmx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gctpvqrha.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gdonmcfra.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gqpwzasyp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gyjhyqytz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gzxfgzzga.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gkfltbkdo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gemzgpxcl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gljjevcan.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gngespoiy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gtgjymdzr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gbxgaedyp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/ghafvwajx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ghwexfyay.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gtbwuttdt.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gvxeicynp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/grhvrveyw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvfucgefl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grphivryr.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/glijitykp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvsjdkqcc.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gnkezxtpr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gemiciglj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfdacpwnd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gsognydvi.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/grnhrmguq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/girouwtyh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ghrdxuhzh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/goeoayjpl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gdgzwbaci.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gixgkgdqy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gitqypyuf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gwfmmtnzw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gidoiwite.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gciqwzaua.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gbhfrvtzf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/givjlqzed.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gpcxmjxdi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gctjaanpf.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/ghgemwvbp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gxlmtueyx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gdhommikv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gowlaygxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gcntomcmq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gmgmbkawo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gxrvneuft.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gqrpigysn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gajmveeap.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gujmdwrzp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gwwqzsgso.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gndnudais.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gfzsayhuw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqlobrlfz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gxmurbcll.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/grkltslsb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gjrnxhptz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gqhiiiksg.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gffpifvvt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gfoncvdoa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqlubygpj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gdlemtjzj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gvfsgrrpr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gcnvxpnxl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gkzzulivf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gqnabozqb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/glsvksbpm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gcyrfogty.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gzalafpvn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gegfviifs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gdxkwqpsr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gghddnlzv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gjlklefrk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gvxogkktk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gloktbxdg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gxjoxfjcf.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gldsuqxsm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gkczxvzlo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gqogxoory.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gzmbzmnez.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gnvoqffle.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gqfopurvg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gdsbydmxv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmzimft.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gxltqpdgt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/geaedmkpw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gafhdprzl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gswtwganb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gbslnwssi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gcfqgsywf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gsdrkjvwu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gjmzrpiml.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gehoanigo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gsrfxilgn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjxxxqjcb.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gljwczkls.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcridubld.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gqsfzvgzh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gojsgnjgl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gpnjiayfc.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gejbhhapt.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gzkzehimb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gpjzpliaj.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gsjxudfri.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gsikntlbq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gfcxbward.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gwshgwjvp.sHtML


<!-- 参考信息 -->