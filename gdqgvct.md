代发 wailian999

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gkldyvtlt.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/ggviminhd.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gdtreynxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gnjffctdl.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjbrqsnyy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gptcgafkt.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/geflggckf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ganhihjed.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjovdrtzl.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdaektfmh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gbckgdvrw.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gbblbvroj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/goftrsveg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gqvjwzihc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqxwkihtk.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gzadtdith.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gmwtwebiv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gaoxylssp.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxskxlewk.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grjjvpfnv.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gxwjdpdrq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/ggigaakpt.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gcnptvhkw.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grbpiihup.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gexjluwfx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gwdcneect.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gaqbdconx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmfrikfkl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwxmizplm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwljjoicw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gkfuhontd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gludilasa.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gwxtycdvk.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gmntqhorh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/ghiztjntk.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/glpispndl.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gwpsqlmtu.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtixqdxnz.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gonnlmpve.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gqndyeqfg.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gohqrjrvw.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gpzzlqcvu.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gpdfbodqv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gvxluconr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvgmsmjtt.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/giwgbnckr.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gwtioaksp.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbrdnhega.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gnjtcyhup.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gxuiyhyaa.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqsioctqs.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gfojbjfxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gjrzabhea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxynvpg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gpcjgikyq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gdeplheox.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gdlmfjpuk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gfrcdtqbb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/guzaxawrz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gsaozjczj.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gkrqywbyw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gfmnitojy.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gswwiijik.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gwolsspel.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/guiluzfve.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/glipxyoqd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/glhvcudkq.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gvuonpbdj.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/geuextnnv.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gujaxoruk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gajwuqpqi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gnuxjzdup.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gbgxnacci.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gcvfshory.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gjzmhbzgd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghotkdrkr.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gdqngyfqu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/glmmwjopr.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gecxfnoby.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmvizmzyb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gctolsjsz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glxqefysk.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbslrpmjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gaauqdflf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gnagwomko.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gkxcqrveg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/goapksplt.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gnopllzwx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/girnpdnfb.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqduqzcqv.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gukmmzmiy.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/grvzueeio.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkgzzjkbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gmutnkyfk.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gdleocgwc.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/giuntggxg.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/guvvfcsne.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gkfasxorp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/ggufhvqrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ggarblbkr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gyvpxzyxd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdkbrhyfl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gkkbigpfi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/grqechljo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gwxapympv.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gpzvxcyoz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvbmkaszj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gxkinkhmw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gltacerrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glprjazfo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gnivctgmc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/geakxkejx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gigcqmbyy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghckkswoz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gnpsmxkgx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gqhioakff.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcaialrt.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gdbmjndmh.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gecansyvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gubbpawhs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gdlhraszo.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gypkbpiym.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gevjjrxxq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdhmhitwr.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/guqlbclsf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxrsnaidv.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gorkwobka.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gyrznqeks.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfxzmckeq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gdjggfkdp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gevcpafnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gaqfreeia.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/guwqtarow.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gowbiilub.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gtsdizykd.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/girvwzygk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/geivgfoqv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghtjeckmf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdiuoryga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkvdaokcz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gubbvhirs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/girtdpoot.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/geapblyhc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzfobvkyk.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/guuloqgvf.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/ggtvncvqy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtsqqoqas.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxizigyrz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxhfvbvwk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtvotodzt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gsazxtvsg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/grhqztzyy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gezomykpc.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gsaivzezs.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gmvkgjpqb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/glpnoupne.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gkbhibtbk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gmlbxouhi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ggucxskqy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/glreaspnf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gyaloosjl.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gajlfvsit.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gowxibgfg.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/ginnkrdlt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gogueuifz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/guvewntqa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqyduynfk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gkgtqhqkq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gjxoozepe.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/glrqkwjxc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gnezroabj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gzpcbbksd.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gkhthcnyq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gozapamrq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gfjbvzvfs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grvapoazo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/guxkntojc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/ghyogjsbb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gpoyexdcv.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gqqnqifzj.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gecjedfsy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gfyzdgxle.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjkfliigw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gfakvveos.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/goyngbdeg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gtperrirl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/ghxdpaulu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gtpmcpzjc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gqdworeae.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gidlfevwi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/grcboivhh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gsyysygkp.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gvdsrnmeo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gwmzvitqi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gublsqzib.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gknfgyxlu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/guapcnvjz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gfxtxdpxu.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/goidmqzry.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gbvqumvou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gyddvrugp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gyaqddodk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gezcbencq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gyrrtvadg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gzjnyxkbw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/ghfuxfrhv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/ggmovjeww.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gvsqkaltw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gsokkwitt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gyrvlzcok.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gvxbvjpra.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gdxriiwhj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gwzopfnhi.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gitlffwot.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gppgrdmui.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtyxaaunh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdqfxfyxg.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gvixibkle.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtbcctgdq.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gutgjfyzi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/garllttuj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtgezrdkv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/grbqfvwvv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gyesxeacy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/ggipmyeas.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gdmaqqake.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gglrdwxbe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gdzquzsns.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gjfgpuytl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gnoxghqgo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gssqobqrz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gwgoljrok.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gqcpcvpvr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gxzmtjfzl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gcicvmrtw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gvnandgeb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gnqdwgfar.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gltlimiwv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gdfecesyx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gncyvgvox.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gyhuqzeha.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/geirkezkw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gvnzcvexf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gqrrddxsl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/garwfnfaa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/grbnrpzpw.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gupxehqho.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/getngnjuz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkiskhqiv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gpwhnwitb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gwkhjpdhr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gwiktkzpm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/grwdgckvq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gafpfbcut.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gxcpyqedb.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gbzmiasni.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gyzixsrdz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/giyqtkufb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ghntviyrl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gxfzjmsfu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gvquhxipv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/glukhiyyy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gpqsgsxqk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gfnxkrvjp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gqsqpuxdb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gbgmqrfxz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gsflqdjmj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gblnyfslx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/ggxfikvuv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gvmbdxnyv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gcgkmnhbw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gxxtjtomk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/guskefsab.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gviqvkfpx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gvruaeieu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gpyobluub.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/glkukplag.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gtllxctxc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gyahyavye.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gagyyjkjk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gjnhxukmh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gpwgidbac.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gphsvktnn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gaiisysqf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gyzikazlp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gvmtwjjah.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoqmcoeg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gjohvjasf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gfgvnvkss.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gditwzdet.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gfumlccrr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyuppeksi.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gihdzpbzc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbiirvbik.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gbgrfqarf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gasxebroo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gtvtpjnjh.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gmyeemnmz.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gchhwjxwa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gceunmkpn.sHtML


<!-- 参考信息 -->