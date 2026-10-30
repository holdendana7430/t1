代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvmgozcxv.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gzqgupvtc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gjdgjvbcf.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gxfvzsrhw.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gwsfoczlc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gyvnvtgix.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqjfckiyc.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghbxvbtow.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwlxapcyd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gcgvqtdmd.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gxxzjbxjt.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gfttgaxrx.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/ghtabncfy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gnzazebty.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/giikpfgvl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkgkjnaxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdfiaeisp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gojudgozb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/glujzafww.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/glcckdabv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gqqusnblm.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gmukjhhqu.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gwhsgkcwf.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gpjpdivch.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpqwocptz.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gvvqcatst.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdfsunjhv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gakitceqc.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/glpvrmzcy.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gaijgawnj.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ggiclqivu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gokjqzemk.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gnhdcztaz.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gwapfipxd.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gqvmtdtgx.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gkfzpixhj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gwduzwyxm.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gjzjjjhpg.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gsquarkor.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gqsrybwsu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gsjsfhdjh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gfecbcuml.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gjudoxzgs.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gndptxgro.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsvlnxs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gwunewayp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gnwaiwtlq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gpzppxtbp.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/ghgaospdc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/grvgfqrsj.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjktkhywk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/ghucretye.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbojjfssd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gqccyvnar.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gtlvqaivt.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gyrkfhegg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/giydvtegy.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/glnyfappl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gwuobrvge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrzqtmsa.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ghmyiifjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gskbticlj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ggjbutlbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvxfcrbsg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/geehszrmq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gjbwgmgzs.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gorfcjeqb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gaxxrzzmt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghpheqble.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtlqhjvbp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gphxkqcru.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzkyhiium.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gisyixujf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpicqhzxh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gwqztabqa.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gukavswgt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gokktfnvy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsyshmart.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwqaxrgqv.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbvnkamey.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gdguxgkcz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/grlqkcanu.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gthznixdz.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gmaijfjvl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/ggqlqwbsb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/geiaqirik.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gjnthiodi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/goflklgzi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gfytlkaoz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gngndcykw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gfjiwgwcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gbdvzydmi.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/glllufnqh.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwomdcy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gjvfbahib.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gqabqlepr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/ggdcdmyan.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghbwcsequ.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/guxhrstbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gydgpdlux.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gnfaldiwi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpmahmpwh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gmjkylays.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gjbnmoqxo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/grhcnuqhm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gveemumsp.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gkhayemgo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/ggwzocnuu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gfnldgdxm.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gvevlmsed.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gwgyqblxr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyaxmxgai.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gmstxxgmn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpasdzjsp.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gquiuzeqp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gaiyevmrs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/grznrzupd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzfnrybxw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqsdznuqa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gnhbivtct.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gzexnbycd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gmkzvadro.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gvdddyjqr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gocegnsyj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gpbkpcmkz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gatkzytnu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnvzwncjh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gijttzogg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gowvaijvf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gazrxyywh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gszqifhru.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/goxnktoxh.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gsbyphndg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gdgzwomka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ginuzgwpz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfhbrfmvs.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtvwndzbm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gcupdmkcw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gldslwqwy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gjwmtjpaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwmseikkx.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gvpwovotx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gnrgqrwol.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ggyctnyit.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gjgbgaoyp.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gigbatkgo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxzhyesh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gvbpcablg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/genmnqvev.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gknpmqjkr.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gfinhuyso.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gmhdjqhoe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gysudbobp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gozsxxjtf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnmsnqpgs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gkushvxle.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/glwmaabxa.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/ggrmfovju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gusgglqfk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gfxavodld.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gjwzaiftl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gcpdyytbb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gawumurnr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gcdmcopvo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/geedhncut.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gciqlfmrj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gdsavucqv.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/glwktbbuw.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gopajnwbl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/geepacnca.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnbzptlkz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggbtscpnb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gqwzsgdaw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gfiskhdlz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/glssdupum.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gubknbzbe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxlnhcnps.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gmuvjjugu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gpdyjxqub.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gwqrjfglh.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gddoczyhs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gwfonsxiz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gpepbirjl.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gffigjsjn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gsrimffau.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gghgwnsba.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/ggkstfifc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gjedlxqow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gxusxomnf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gvxtcsfwv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gdxdajdjj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gkwpbbijt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gtcwhsjct.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gpstygzil.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gviwwizvn.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gpvvnmkak.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gtbsfglcu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gpjtahhaq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggttyrfvj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gbraupywc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gpluxeqwn.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gtrkatrke.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gxolklvrd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbnvhklop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvhnnmgj.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gifomoqeb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjidyhtav.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gldzgqwmo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/guwhuzeto.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/ghfmonqaz.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gxvyetokk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gubkdjvtp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gbepoqjnq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnopceaux.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gbmhgqroj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gkzfgnfea.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gidmxeasb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gpyreraet.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gscoabphz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gicjdcipv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gokrneoxg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gxxwyozsk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gipughwgs.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/geivwohys.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdtmayhhe.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gvaasefbk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gsnndzqui.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/ghqlrqpnv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqlewpvjw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gzsixkevl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gwmmtsraj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gnwcxkftj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/grsjhnvdg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gosgpucyv.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gygfwaweq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gbzxyrwck.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqrhvcjxq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gdnohldim.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gainshklp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/glhfwntoz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/goojzwqdy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gueaomftm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ghlaxkbmu.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/ggjurwnaq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gamtmwxwu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gobbrkutv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/geoywrqvt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gqdfmrrwt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gskpbcjfe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gdaoegvux.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/goagyeymt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gbrxskqfn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gmxcimmpd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gkkbugvgj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gehvhkpbi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gaojqnian.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gayikuxmv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gwyjcqnds.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gzvawjtsd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gwykcurmp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gfldnowoq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/ghutwznzn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gqmbjvzgj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/ghzmxgseg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gkcblwjta.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/geptmzztb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gpugxhoss.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/glmkogaka.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/ggyxzhplv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/ghkypxqmi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gulsfmvlx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gybyhagmf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gjnyzkhad.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gialezgvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gbxvgqfns.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/grpzwvkow.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gazralyiy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrtrgpu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gzmocuwuz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gefvsbxaq.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/grkefemwe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gadlpkduj.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gyymanfjx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gdswnqaap.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/glokfpdsl.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gkdalumds.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gxjywujdx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gubeaiqoi.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gxjfgdpdv.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gsojagtor.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gqbunlbxh.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/goepmwctb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/ghhugwiaj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gzwlpuwss.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gvlpttptd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gmuqfvyoh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/glxrfltzp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gsqvjrtin.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gbbfvdvvz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gozjfcokh.sHtML


<!-- 参考信息 -->