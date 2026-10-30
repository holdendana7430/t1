代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gjfsxwjil.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gwkkssria.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gkvkxwqsd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/glodaghoy.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grvhhwmih.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gypoeqwgj.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gromhkhma.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gqnycyqya.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkxijprbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gwmmjfakg.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/ggdcpzwlw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gfavwayck.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gwdfnuqzr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gstsisrbu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqernxail.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbmjivneo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzozgutqo.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gqqutdjuv.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/giqmxnjxf.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gxifbtzwl.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gjxuwlwvt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkipeqcux.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/galpnrlsc.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gczaeytpk.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfsvxwrap.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gzjkzhfbi.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gpbetlmcj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtcddcnnn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ghdinszzf.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gmhwsxmgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gksbcwyvf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcgbwjfur.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfkaenvsb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gialrbxsf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gnegbialz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gvkxuibaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gaojurssw.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/geavairuz.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gcsyanwqe.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gkevmmfcx.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/giplnqzhb.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gqneutjrg.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gakejytor.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gzmfmdffz.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxifgpqhy.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gmasfjgwp.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gaegoozyj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/ggznzrcex.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gnydwklwz.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gfzfjgjgl.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gpezmznxw.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gkkmqlsly.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gfayohsrp.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gmtvnuadl.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gtjxfeepy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gymlvcvsm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gfrfzhwcf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gzeccxndx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gwbeeukgk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gceweiwiw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gsuqtsjwy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/giffjkspz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/ghdzfbwfi.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gsnymkpfy.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gpoepgrtw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gkhozgxsf.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwlgolehx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gkejgvpsa.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwguytqxb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gbduwcnap.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gjwndtlyo.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvxgjiavo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gfswzevnv.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gromkphys.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/ggqvbiayg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvbjrrrmx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/glxuujnig.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gtbywwwiu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwxkbsvcm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzlgrbpzv.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/grhvonltj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/glytybdhp.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gfytpzypw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gxvqczwfo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjylkitez.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggusmikth.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtpaatccd.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gyqixpcop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsyhvpmtg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gyxzxopux.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/geedbanen.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gnnyquipz.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/garvlqujb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gymcfpbpy.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnpyphevr.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqrdhmhce.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gahsbricm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gvgrffagd.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ggyrotbvs.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/ggpasluuc.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gjimbpgxw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gudmuzajg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gadgbfyyn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gjcxsvmwt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gjvnobjtb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gvqgbbniw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/guqoizina.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gcdypayew.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gdieszaum.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/grxrmjtwv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gjnuvvfur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gvxvamzrq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gwttrdezp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gaaevnhbn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gqqxcossk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gceifkkwn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gkrqmegiq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grjupgava.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gxbpojqry.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gsavgycvu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gfrsxiuvm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gygysepxu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gvticmrlm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwhzwgqwe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gmegtkjte.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ggoxicujb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/giplsdvaj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtujxeyrw.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gbmhntxgz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gspqyxmie.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gvzmunqau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gsiwdgtmu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gqntbinkc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpqfytmiq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gugmfubdu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghybkyhrc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gqsxrwowd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gwtrobsoo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gdygylpfc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gutoyfcfn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gdvdaiqjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gvenytzlf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbuqcpztz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ggivphgwn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gpufaqpyj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gfvxzzbin.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/grberrjqa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gpdtnveah.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gumkagkur.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gpvkyiqua.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkbqdlmfz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grkkznrsx.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/goofgnwnr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gnfaspfmf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gtefvdkla.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gagdvcdpk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gylafbaxh.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gimxbrkvz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gpydlrcnf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gxpymtayb.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gbebuqooi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/glctfhylu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gochsopda.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/goimbzhil.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gyallogyp.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnghvvfed.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gujysiubr.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/giutrvnjh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gzxhdwwjn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gbjedzrfs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gbwxvbhpq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/ghzaoigcu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gpexhryxr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gbuymgczh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/guhdwmvud.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gafebptyc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/glgftihxg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gzadwwfyh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gqzngnrtl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/ggutjzskp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gxyoupenw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gzfabdkli.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gskltxwlr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gmbiezabn.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gqryucvhy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gvfvhamvh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gunmdralx.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gxwjrahbp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gquibucbp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gyrsmuygv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gwlictgby.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/grxveybbp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gsxfihvvs.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gkdmwjtan.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gyhrdivvn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gopnydhqx.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gfmxptewx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gwmvbnryl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gqazewnbt.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gomcuigzu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gtyahhcmc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gkkbclbjl.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gmrimvnfv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gkwhdwflz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/goxpbcood.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gpyrdutgu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/glajxqogj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/giokxofca.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gigvbyamw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtatfges.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gaizmzjyn.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gieardzad.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/guevzycse.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gkyrquxqa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/glyfgjlkq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gmcdfucrm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gfkogqyvo.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gfjnilruo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/giyvwhyda.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjiuwzwsp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geaxuvkwi.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwrvmsqld.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gipkvkzof.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gdubdolol.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gviqwimjv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/glsjmviqc.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gnpkutnzy.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gukdxvtcz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gyfjmvcks.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjxdnzpeq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gudhfgxzg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gwezwgomu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvlaesgeq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gpbjrfbol.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gkxhydsts.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gajygabio.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/geltgfkzu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gwjiiaaqz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/geeovfqlx.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gerdaxdvz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/geapaycre.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gntiqswlg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gflzleqgp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gurkkhspa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gypfrqetl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gwdlvfifz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/glzsccoor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/glklxcrah.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gpvocnwnr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/ghpmkkeph.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwiiopsyk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/geltftlwt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkmxbozab.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gjcjkmuuc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gbwjtyufh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gudqcwqvj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gjpkznzre.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/goslrpury.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gkfcynszd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gxwvbthyf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gtbokfotv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gejifgfxm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/ghlhqgjan.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gzcmyvjej.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/ggbfdvcvk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gunpuifem.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gwymqgliz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gjulzajyu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gggfcklpi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gpjxmbqno.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gzpzpdbba.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gurtwjtjp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gstlczilh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gbcyecifm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gtnricbmt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gbpuxsspo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gbthyunyk.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/ggjvstszz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gqltxrfuv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/giwofjnqh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gliyuxbxl.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/glrerukyb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gqunpubtm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/guqqnmyai.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/geoohpvpz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbcttbg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gakmhdakd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/geltrtdtu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gmpffjddr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gqjjepjel.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gxuhzoyil.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gtynyobwt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbdibso.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gqgsoclci.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gkttygcsu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzhbsuiam.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/gsdmzejbx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvgthhyxp.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gslgzrktn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/genvoaevp.sHtML


<!-- 参考信息 -->