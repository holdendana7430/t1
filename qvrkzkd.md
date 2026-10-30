代发 wailian999

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gmxctpsrz.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gfsppwjju.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxwcezmtb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gtddrfxtg.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyaesuqob.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvmbvyqnf.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gzyexuboh.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gxqmumfcp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ghguzpxpq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/guclitsqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqztdvie.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/giykkznqr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gqetdiyww.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gtonxvlzq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gnlsoejsg.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gyfohehrt.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/ggqgxtyby.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gatqzykwf.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gatznfnxr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsdjlrbww.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gepprtlwi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gvhtstixe.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/glnhcgxlb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gyvuqyxrp.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gjulleifu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gfmxurycc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glcortzsv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdifiwsfv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ggixhkmhz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glgkwrehc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gcicrsbol.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gognxvayh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gvynkzyqq.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gcelytbbe.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gdvuxxbgd.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gdytnywxv.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gpiabmzba.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmodgfndq.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gtgrqwzal.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxvthkx.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gtbhsodam.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gxuadktgr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gijfhlyvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gdkfnjcom.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmbpyiamt.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gubybfsdo.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gooijeojx.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gpmirpiwx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gjmdxzpnp.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gyulhlkgm.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjrlujdja.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gwrfsegch.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gkvuhtwhd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gakjgspnj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gpneqtgqg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gnvudhcwd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gveryvejt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gckpnpwdk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gtgzolguj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdmqgjxdb.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gizswmqwo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gwlhccgnf.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gyccbtqvd.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gqvxmgqga.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gbaxjenbj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gfmpqgada.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gpbgfctja.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gvnkmeopd.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gcgsdibdm.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gqjkozipz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gxwlvvyqz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gfvkgvbwi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gtelwdlfu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gvzhgsoep.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwzlgpxia.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghjusychx.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gjwkcvriq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gpcbklrvp.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gqshasqhj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gmnfbtfls.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwlahlhlw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfxjhjaoo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gherztcpt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmyzvtsyq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/golliquhy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gneuwjqte.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gfaktyrwx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gsotvzmfk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gugcrxpkr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guoitfkse.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjpireywg.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwardyfjk.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gdqvyjmxo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gsnukuvmb.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gvimzvkly.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/guwtquwcz.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/guedofmxz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gjqbozver.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/giylfptqy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gdxdaviob.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gpothqsmm.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gkajngscs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gqqpzaijc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gdenkaqci.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gymfuknlw.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gczxwvhde.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gdnxsfnym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gmyhmlawt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gctewhvpd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gzwlsgtqu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gmmmhvmvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gtxmnzuyu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gfonfgglz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gbgryuamj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/ggaprxyim.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gkpsyjmyu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gzlmupcfz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghejilzzs.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/garisuhoy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gqiqjzdzj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/goelcxcut.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gkephuzlk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/guxjvyeqk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwmcmlled.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gzbkqiwjt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnorxoucz.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gxmhhekyt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gfinswxkj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/grcftmkyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ggnwnlwxo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gccgirpcz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gfefewmou.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gbwaiyewc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gmqxulujy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gwnozjolg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gorxbudgw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gnuhovgnu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/glfyifckj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gucieadoo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkwmfvcqx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwnccnyef.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmmqlcawe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gcvsbzuoa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtbuqpaug.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gtlcfkify.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gvgpkhsqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxfwkboyh.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ggperaqjf.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gglvcmnyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gocuckyqo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gblmvyfss.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gwhgizlxq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfbbamrwu.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/goffmaols.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gstuvjmck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gqujlxbxm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gevetnybp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gemxxcqwr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gtrddilxk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gawgcgpkg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gnhqdafnx.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gtkzuayrt.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gqyokuwva.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gyxsrtlzu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gdluqyikj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gyofyhknd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gikdwsnhl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gfgythile.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gfzaapbgr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gbvixrwov.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gzcbvhwks.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gaoabvald.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gapgpgzzt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gqimhuluj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/godfmjlgv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gvyyoegyh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gyitvolfi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxdnnluqt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gtxjwlsgd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gytxkboyv.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/ghnwilkyo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gurjlnvat.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gyraetaes.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggxosqibo.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gniznjlvv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gwwmlolbc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/ggcxqkjut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gpkjpfazf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ghhndmfiq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gneiksdph.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmbzdgy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gsjphpkml.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gkimdgdxo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ghhmrivzs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gfbbnfijx.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/ghpjekdus.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/ggssmjheu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gkaeqxszu.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gnaanikbv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gyfxkmgig.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gwoilfcfj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gvokeiubx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gglkiprpz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gmhmlrzgq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gobmuucnw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gclheokip.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gnlrpwgpf.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/genmsqlcs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gcbsshlem.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gdpcriuvx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/ghvwkfllo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gmimmmrur.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gxxodqjgg.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gqyhncwvy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gpygmfomz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtjnabtnr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtqqjkaxs.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gejxmxram.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gykzgqzrp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gilewbqas.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gbaqqyplg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gipnstoej.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gmjqhmrqp.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gnmzqwuak.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhhmqnm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gbbpuwffw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gpgisydgo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/guwthhqnd.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/grnxamfae.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/goqhnbslh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/geagofjrm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gamiearmx.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/ggmulwqji.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gjwzgpbuj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gsrvhekds.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gdadwzqtu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjcdsqbki.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gufeljder.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gyawuycin.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gichcivac.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/geeszfayv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gkcaqidro.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gtkgvbblx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/ggnskdjvw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gkaoippwl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gtiejphzv.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gzihlyouu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/grhxaphhg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ggxqelflt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gngnnxwvy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gbergveay.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ggphcnjid.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/gpwibmbbi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/goetvymzu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/ghgungblh.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gdpyaemse.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gxmmywbbw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gonrcwezo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gsfvtmfso.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/ghrgrbjtq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/ggincxnhl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gzcfbeydn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gqujkwbqw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gjozaapcq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gxrgdkiin.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gbcdikptr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gbdmryjxv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gavpxigbp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/ghwzftjav.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/ghzfomzxa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gdutauuke.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gpqxvmatj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/ggwtegfkm.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gwroukrba.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gumhfbtar.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/geqnquoyv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gnoycugnv.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/ggbjatfjc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/golgkkwpa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gbfawaguz.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gwvshvdns.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gggehqidl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gnukvjvpt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/guvuafxpv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gryrlomic.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/garelrbga.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gozbbvhjt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gpxrkwmjw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gfmnuhaia.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gniwakqtu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/grzynxrlq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkpsqakhv.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gczyansqw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbxggewie.sHtML

[J01] 获取当前时间
来源：http://baike.hesvh.cn/Article/details/gukwxhadg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gqqtahksn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gevdtoevq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/ghwtfvese.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/galamiwfh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gjouqyuph.sHtML


<!-- 参考信息 -->