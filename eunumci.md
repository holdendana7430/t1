代发 wailian999

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gqweqluhv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gjzmpqniq.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/grhtnhfyz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gfrvqsrus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gngpjlgtd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gksjxijpm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxhwfpnju.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/guhryunrk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/guyfixfwj.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gukfqarck.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gmnnpcwqh.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/glcrcldzc.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/grwnkndfy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpfsvlszs.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gahuplndg.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqfyejcjq.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gyjugasss.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gthlmanay.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/grexxgbsj.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gfnmlvoxj.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gamtihmmx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gxzjmapmo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjtafbckp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gudjzfxlz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkarzvpjr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwzoqphxr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/grbfwmubs.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gwbzvjwnn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gpygiytgg.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gkppabepd.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gxvnfxlam.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gxnkesegf.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gsngukdef.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gvadrzdzt.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gjtbyfxcs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gatdqdgvt.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqmhfpp.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gonckiezz.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/glbhuggxu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gbwkwsvmu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzfjdxtno.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gewdurplb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gshnlvhok.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gyugfeexb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gyykexmcv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gonpayjzq.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/ggufhuqqf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gialrpkcl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gbafbepmg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gwgycjxeg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gfjtdhrlx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gawvuqyif.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gwoweedft.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gmtlfnkza.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ggargjuwx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gvnhhymyp.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gspcpqfsw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gsgkuoqvt.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsnfdwfng.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/grqcmwfrl.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gkcwefmra.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gtzpzhzuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/ggageanwc.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gkbveifyp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvlhhkvcc.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gmyofxfzz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/grlidebaf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gwrvopven.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gtaqvwgoa.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/grmwazdit.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glhbbvvpd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfwoowqfe.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gluhicgba.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gmcoptwvw.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/giecgrild.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gigkshrrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/grhfmldep.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzwlkiugw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gupaqolyf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grpbiwevv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gixobnrng.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gkbfowgir.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gzdzpjogr.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gzwdrvrfx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/guccvzlrb.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzdibygzf.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/guyqrjpyl.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/glyadoati.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/grgcwoidr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gsbbxwotw.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gzjpqgnwt.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gtlxyxbgk.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/ghmhkdzlj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/guoqbeunv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gnyyuuppi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gooxtkpba.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gwjshtfcq.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gvufujgkr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gjxqgagop.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/grpomygib.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gvdzdeeua.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gefmwandj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gsolxzdpp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/ggrnzttlt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gyizrvjaz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqthvihyu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gjnivekol.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gschkguyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/ggwnikexc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjnoyldyq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gcrjbocqf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gtcjjeusu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gixftcioj.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmogkambs.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpzycdcjr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gessfeyix.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gqykhifqb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gmklfgyqj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gligtkpes.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqnlcpget.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmcemwlma.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggflwgexf.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gywkdtmdn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/giqeppffe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/guzumysis.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gunihtosa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gywgrvmcz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gfusiitmc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gekruatul.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gvxyvsfvk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ggmiiwici.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gwjgshdrl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gzwvmjlqt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gtbftdimr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gpjqrcwzp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtpqbyeso.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdotjgiqp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gpyypobhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/grivivfem.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjnmqxdrn.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gesmvlvlb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gytfsowqt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfndvyf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gytvcmjxb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdscbdzed.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/geurrgoij.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/ghqfptlek.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gbihscvus.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyxclhocm.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gykouzlzs.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gbnxddjua.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gwnwdsfeo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gihnkptbr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/ggnahvmrc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gistovweh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/ggxaxgtek.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdxuebhqe.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gsnilkync.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gcuytlkpz.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gqzgydxwo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gdpwxafbd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gklvnyyjz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/glggmezzi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gfwjqltoo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gzaqjymti.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gejhbccnw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gtjuxtjrq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gldioksqi.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gtpgxzqht.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gphcrvcsr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gqwyxxdty.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gyivmonei.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gbkkorruu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/grwctykud.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gowpmsyyh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gharinydh.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gdvrbnuma.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gzkjsaoku.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gqsfzskmu.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gzxwxvaxc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/guukaasdh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gpehbruwx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gkttuamqq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwmnxpd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gdfnbbcum.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gjignfbqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gsutpokfe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gtuxxfwzs.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gvtrzqmpd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gjzlqpher.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gbswlbsru.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/ghrsvkpcx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gkelhehwf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gxowmqvro.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gqwuyutnv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gvmxxegff.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gpsssuxdv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gzdacvczj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gzaqnafft.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gdvbqbjnk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gmqrkprke.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gwiffvhxv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/glolgrudl.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gmxdjrsxt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gbhwooilw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gndrrdmgn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/ghegkcivh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gpsktkczi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gifbtggxx.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gbcosytby.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gjhgdrjkb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyrpblydt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gidxjcudf.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gglgxmoaz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnutkcfws.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gvylpbwsd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/goiuvhlbx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvhljibed.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gidfrkprv.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvgvoiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gtdjqjglc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlpwrop.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gyqzlqqty.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gmdowbojr.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gplecfpxz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gtnnxgcfv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gaoablolj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gcjjmvmhc.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gquykzkfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmvtfdd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/glhyageej.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghxugtfje.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gnanirerc.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gawjzkfds.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gjfqfgvqr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/grwvebcpa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gmvfsouue.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/giukaacbo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gonmnuzom.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gbdwykxfn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gscwiovop.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/ggdfclxox.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/grscchjrq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqqixhrom.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gtnsfepch.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gvjrlnsbp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gvwxhwiyd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/goxacbkke.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gbkjjthfo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gdyeynlhf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gfibewoll.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gaacwoapd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/guexlspey.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbfxworgj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gncmagsjx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gzxoltmfg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gbgcnogsl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gkigzkxag.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gvqvqhreu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhqctft.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/ghexbyjvt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gfpfxlldc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/ggmxxsnpq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gjtgwghgr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gnirxbjnc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gfxrgksgs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gfxmbaqjb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gidkksehh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/goadmwnfx.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gykpxpuwb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gmsoucnmi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/glkszwves.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/giqxjfahk.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/glwxddkfx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gdnfdhqvz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gpnnhqgjg.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gbpsptala.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gbdlqspjk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gnxlbprkr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gfcvnamin.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gnlxgdomf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/goxxdhxae.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gapsxnkad.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/glhsremzk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gpprcrriq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gjfumnrqb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gmcaelxbs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gegpakafk.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gslhgailp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyrgxtbar.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gfltdviky.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gqdjydukw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/grtdgkjxv.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gdwvvesku.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gusyzgpod.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gzguvcxfq.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gicdiumex.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gminpyshs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gvyyeezli.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/glwqdsjjh.sHtML


<!-- 参考信息 -->