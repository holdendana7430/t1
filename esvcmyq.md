代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdggupjco.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gsskxjlwk.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ggunjipvn.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gbceseaag.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gcfeyfyjt.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/goacgqqmg.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/glpyqtpfo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gsghkkuxl.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ginpbbmvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gfyhspnly.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gygeldjnz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/goistaxda.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/garvhstsx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqehwrseq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwwbuamzz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/giofksklp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/giwfxkdrv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gpioyojha.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvquapwhq.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gnnkkmxvf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ghwthqfsi.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnlitwjoe.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdlvachsb.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvbmedjeu.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/glyjxiqjk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gwgvutrhe.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gnnwxaxvs.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gmblitqfx.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gzbveqjmt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gttcrtywd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvyxstcso.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfpytktmn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmcrtcmgz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gukctneoa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/guwjqnrwv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkmojqzoz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gbffhoikw.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gvuparhbz.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqfxemz.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gnptjaiwf.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gujfdmmqg.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gezwfgweh.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsfdijhuj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gedcaehlt.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/govmfxyby.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gsstghswi.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/goaztvoai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gxrfflmay.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfxizavqp.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gowaoczep.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gplgzbier.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gaozwyejt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gvwbykvum.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ghnggckzp.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gegmfljyx.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/geamvqscq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gynakwnyw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfnyqptf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gihcjimzn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gjdkvenru.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gvigghjav.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gfzlsuabh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gifoceuqu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gatknnlbd.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gdzcasgaf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gvhtufycs.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gzrmhclbg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gkpixlpft.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/grgafxtrh.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gpcswskuw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/glxbwlpil.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwriqwswy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gwbenrkrt.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gidtdzkyw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gvqujxqcp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/govuhhrft.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gspspmqis.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gcxafqttq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gbfoylyjz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfnurjnvg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/ggldctdpd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gqkprucdq.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gvnjwncdv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gvapqomai.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmvvtoavd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtwzpkiyu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gluyoqcqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxfxqjtmm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gslsvqkzk.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gyvckmkmg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gldfuowhf.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gjtxbnozh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gpovzebal.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gykburfio.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gsnfcgwwr.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gctxxoezx.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqlcmuskl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gnjxnveqg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gbupsydes.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gzngmibyp.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gepahuhqm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzxqxqexj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gcrkodqyf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gmoizpilk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gfnthylde.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gnynnzbgb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gdmzyjnkr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gnrdbtgqg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gougloanw.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gshqzfxsq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gddeekwjy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/guhhjanze.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gxrbjaiho.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gpwsqndmq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gpjxkpoij.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gnuakejsm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gclnpnpxd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gaujrcdeb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/givizenop.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gjtlkdfod.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gpgiisosw.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmooraozi.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwruzqvvh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gwqyndxta.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gmkmgpvmi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkymrcdaq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gaqagbytj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqoatvlzu.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvamafqho.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goiufuhsm.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gksqtqtot.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gebixxere.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gyxegvktd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgybhnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ggybtmbtf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/guyjrfqyu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gcktxtqhg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/grxgwyzcq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gvvdryxyd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/glxmdqlkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gxsubhgod.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gopaefmxd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/giviinsmz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gajboykbo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwlpsxhig.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gtqozqlfj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gvfiqnmmu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/guavbfznx.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gyfauozmm.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gqyeyjvpo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gflbmrrbt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gihusupxx.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkwfqedtf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glwsozhfd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gdzkezrbv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/geerugdun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxglrfdpg.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gczwzkdqa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gbdwzglyq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gvxfzstzn.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gnmevotrf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gchppxbvy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gphtdjfxb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/guatokvqw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gryfaryst.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gdkpuaqwg.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gdsuwbbvf.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/geprnpwvs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/goeqqkdev.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/goiwssgnu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gulvswhoq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtwazfyej.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gvqfxwscu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/ghdgqbrqd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gtafoecgf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/geccwulpf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/guosrklvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gmjiedupv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glckecuby.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gpqfpxbwe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/grqhggjzg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gxpsvzfjx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gkasdpzkh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gexuwffht.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gjohwtybh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gmiluiwza.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gvulhpzeq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdboopeao.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gddpyfchv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gcmlepoxs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gpymxuiuw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/ggctxsqsj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gktvmcqaa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gvhwonald.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gwvtlgjds.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gbokvkvbu.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/ghynppnpq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gkhavyfow.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gujqxeyui.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/geltffqne.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gcnxnvife.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gmxsvhwhb.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/ggmhpmrzb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gaxlsxpje.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gkwzegtmu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gancmfnsh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gymylcluv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gdercxukz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gitjftbne.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gfvpkmkqh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gvdglykra.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gucqckouw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gwhizgcwy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gumyfbvhr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/goiceuank.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/guuaxdaai.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gbbnflalw.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gryytwpsl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gzmdofagv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkaleanel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gprrgkaat.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gvdshsmsb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxipitpqx.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gevfjiffp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gamootqzn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gcqauilmh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gdtrhovww.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gupbppjhq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/glqrufyld.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsuzoqxgh.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gcyrmycov.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/goyzojtwr.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/geamryigm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/geawvykiq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gajfvbpra.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gdrqcfecf.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/glemwsjmm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gwwcwcdtq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gnypbfjkt.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/guwbplfbz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/giwdxopnr.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gelxxzqtw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gttowvegs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/giayqhvyh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gwqkmuloo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gmjgastqx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gnysiubxl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gevnmqmcz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/glipomsgh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gnsnydbbw.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gzgxivdab.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gmfbbxxkq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmzgnzzql.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/grnbcsuhz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gocfvoxzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gkiavrwep.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gsgrpzude.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gsrdknkbl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gzfkhzypo.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gwjrlgqvv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gvrkpfiyw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gspwiffan.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gxauiqhjv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gqekikdkb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gtvegmbys.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gqrplminb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gynwqblcj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gxiaepdal.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/ggezmgrst.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gdohoojlo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gdxulskxi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gznwmsuyr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gwpljsnai.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/ghtugqhxc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/ghgekzcow.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gjrwvnxol.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gmtwkzeyi.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gxatfrmiy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gpyidlifd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gbqlasszf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gevkieymp.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/giswkezhr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gepyfrqbw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gxgoybzry.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/grhobtlcf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/ggxnveimj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gtlzacoah.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gnyhontlw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gcitlkgjl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gmfitjhcc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gildkenjr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gzayazimy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gvoirnewo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gqpdmlhhc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gczpmidry.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpznwfpkn.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gnnqzcnne.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpiwdszmi.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gfyruqcpq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gxyxrgqpa.sHtML


<!-- 参考信息 -->