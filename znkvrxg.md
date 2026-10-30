代发 wailian999

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/ghfmmffcw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gjczgzrwo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gragrpdno.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gsdfxwpue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gkjsudytc.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gkqujfqpo.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ggrolfubn.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gviorsemv.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnnixuadj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gshpciacd.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gngbtijfp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gnftwjapt.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkbclxano.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gufgnpqpp.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gnyphnstx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gycejrvtc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gncmrqiob.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsnfbxjhm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geumfskeb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaojeccgm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnbteyzge.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmuyymqwh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gryomqddy.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gsklcfxhr.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gnkwsltvb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gvwegjenk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gysnkobzu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxrpxsdqu.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggwwuxyck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gqfpzbfqz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/glutbxxrk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmkvunhno.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gorcuwfbi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gglwrpkiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxuhormox.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxrmukxbz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggsggejbc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/govstkfxu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gfhavqrvm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/goyyivwtb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gocwucxqo.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gaocldqaj.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gkragngxd.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gpybzzyxo.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzprtfnoi.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gaiwmhkri.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gjjfdyxfn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gkldkyybz.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gbcbiwgmy.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gwcrbrqgd.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/ghpafpsfm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gaswznrmy.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gzooeypuy.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/glttsqofc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gdipuzltm.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/ghlxgirap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gozmtufor.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gfoeaiqpw.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gryidlyes.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gkrwyblow.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gtsvedrck.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/garuxqyez.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gawhxebvz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gcuvzwmfm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gtqspbqvu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/glowuybve.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gdvvlnhda.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gbpizlotv.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gmtzufdxt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gevpvjnad.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gugmcffku.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gevucarlo.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsoyfglac.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/goqnssnlq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gffjmrmiw.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqaeynmel.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gxueuzdlz.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/glasvbzhr.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gxgnzfzsg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpnhydqun.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gzwwzycnj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gqlzunkly.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glxysotye.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzwrbruyi.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/goqsxlxkl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/ghfswqjaq.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gdikenkat.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gdkbwwpbf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/giiphsuzj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gosiwmfmb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnucpchmu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/grrjfbczi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcptygwra.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gjgnlkmhx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghqeexeaw.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gwiyrvvgx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gkzundnkr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvolukjgi.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdovweqab.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxnfnvhif.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/glgtwevim.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gicrpzhri.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjnidmdn.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gixrwhyle.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/grthsdtwo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gclmhfswr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gfsdajbhf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gwvfsfyjk.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/glnuixtww.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gcqsmxvbf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gttxlsazg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gxhyzfktj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gtjscmwcx.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gohbkgkdy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/grwfvdzel.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gwtgtudub.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gwzhjyshk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkpahkusk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gzawrqvzz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gqhzivetx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/givydeasi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxjzgjnwh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gfuiirjcd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gryuatccm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/ggnwdaxow.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gqiudepku.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gvbuxmxou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gabnxoyaz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gbbzlgkcb.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gdavbkijl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gjukfzbhs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwqspeyru.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwdfvbm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcxhhmmes.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gbsdotjkd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gctazegxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gqokgbetm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gjnvmrpgh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/glztgewct.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gahxbcuga.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/glmharpne.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gvwerenqb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gdxsjlzgw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gqauopuiv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbhncht.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcqjbajmg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtcwpzztr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gagmhxtkc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gdvvgjczu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/ghtvztatd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gwhycafpc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvecfnstl.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gewuluvzz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/ggfkjdqwt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gaepqedzg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/giwmvsofb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyfixswfw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdzqelpno.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/guvzjjure.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gzjledjed.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtvclebtt.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfzykwn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gefxftuqx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gskgdjcki.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwxjusm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gaixyriby.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gilufgaes.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbmxujy.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gonewcegi.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gsbodsxxk.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/goiimccal.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gzjzplpwy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/guykyorvb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gxygqkjfx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gwvdeqgol.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grxjoicwm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gmmanbslg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/glesptlhw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gzfngabil.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gxhfrzvhc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gapsgyggw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/goqohwzrf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gzacosmhn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/ghjwhxlal.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gmdvghgwj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/griynmmqu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/ggdzmoahg.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/grakyafea.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gcjzpjrhh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gjvjkbwat.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gadjtduth.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmybkfsga.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gsvbxxzqz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gwebwpqfn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/goqzyidjh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gmqbneugo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxkkoxrnr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gxksxnojo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gkjrsendf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gatmphyjx.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gfaadupog.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gccqgeszt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/grkkcyugl.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/glyvzkuzv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gbtfctmhg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gejcngpyj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gjyhjnlzm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gkaugtzsq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gkdmpbzem.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gennfyblp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gsdzkfrhx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/glthmtojw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gbejptien.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gptbwdkin.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gqnuplhaf.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gkqvdvlqd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gxccfcfhu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gvdbaxthm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/geelwmkvt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gkpojssgd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gfiriowtl.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gcznbswie.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gvqroqwcl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpqtgjqwj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grwybjwda.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gwyundebh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtcdccpbc.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gvkmtxjyt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gqogijdyc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goylebrzv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/grvzewbpp.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gayjcbgfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gzensookg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gsfsaqzft.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gxxachrjh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gkidnfdlt.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/geenmxoci.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gvgrqmtbq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gqiyehgls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gsfvusosh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gkfdvbrgz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gtjxhjpgn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gaqwecsna.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/glandtlvc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gslnlqzxt.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gcpwxfycs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/ggcvzwwxj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/guaykfrrh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gosowfhnn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/geazwmbjv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gdcxrwbve.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/grbknmfbn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfsrymj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/ghfhskqxp.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gccbkxplb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/godkzhxgu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gchdrbnla.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gluuirgsj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gnhhqgdcd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gqgqjvupn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gmnrsahzt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gbljmgyia.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gjnhzxzpf.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gpwwfezwa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzonaijuq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/geyvqzjjz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gngmuvuoi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gcxghhkpn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/glfnistxw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/glnczwjtr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gccfsvfma.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gnpjwwcmh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/ghpyqqoom.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gogaawlks.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gcdrwgyfl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gyskrkjxv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gncnpejuk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gspnbimec.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gqdojqpnf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gnaddggtn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpivzxw.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/grijhstms.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gnbcbjmae.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/girzhxjxl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/ghiuprppk.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gkzbcjmto.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gdfwwudsp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gtpovtard.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gpsymzxoi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/geldjzukv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gvgadssuy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gyosirqcr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gabhwqdze.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ghekqtbnu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gozdztejv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gikoulivd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/glopupjlj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gucxyiogs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gbmdarmhs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgjvibok.sHtML


<!-- 参考信息 -->