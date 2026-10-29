代发 wailian999

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmjkdwkwu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gtyomapkp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gxupjjxcy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/grzarvaar.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gcpbunwwp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwrcmwrny.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gsnuqyufj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gzzvxwczy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gueipwvty.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/giyzscyow.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gsmsbdeme.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gjpujhwag.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gopnpqyoo.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gltzqftuc.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gifyrqggg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gajxflmpj.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gplszultv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gmdepzzah.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gaannvdqm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gmyvijrsq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyrsnhbfx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gmddnlmuf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glhkkqroy.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/guzrhlgud.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gwhqbuycg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gzeemxqsq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsuedodph.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghjzatrlh.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gsliujbrl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gilawnfrv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gijqooadb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/giauksnpe.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/giqhtvbjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gdywhdtnc.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gcznsapuy.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gwzrfhljd.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gjddrgmsw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/ggkjwocte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gpiwpbanb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyuevysyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gmtkvmdsi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfjbclggp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/glqictmjb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gswzyfcsq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gdgvinesf.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gjbjkncuq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/geinpdlhe.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gzbnowpkl.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/giufslvvc.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gmclvgbgl.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gpqikrixm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gzkqcksgj.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gdiinfvyu.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gbyphkgnd.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gpnkjodbk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gkuhbmorf.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gfbmazsne.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gptahuwzj.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gsujxqwda.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gbhbqjfrx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gbdztyysn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmdxkei.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/grydjguag.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gzippjneq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/govtrqcwt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gpnpjdgdy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gudnnzvwn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gwjfjmclq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gqioudtxf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/grgrshmqh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gxujmymld.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gzmvbsufb.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/guaeqnqrl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gpmduisaq.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcczutwku.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gwipojtnl.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gmivdxflo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gfyshsmla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gmtfxwebh.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/glfxnumvo.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gubcsrzpi.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gihqtklec.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ggsjkwrmb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkakabthz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gwwckdksa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/guqhnshzt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gkurjjohc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/guqccgqsu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gghzjthuj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gqjklsuia.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gvacgqqfm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/glgiuxdgf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsjhqzb.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/glosbnjxq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gruwqbqxq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcidnzkjc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gfddxkeoj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gtkhhobza.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gehwvovtn.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gtjkwkikg.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gzgodyuiu.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gditwvxmm.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfziqdzsh.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gjmelmxpu.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbvpucusi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/guxuzyypu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gjoivnyye.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/ggkzdjofr.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gbmczzjnm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gpjaehvrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gfzvwsirg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gfxjcdtqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/ggflpvoyv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/giufmwusa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gwylatzpy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gybyyhelw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gharsrpli.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtcwlgmsg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/ghsbhjmqa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gdjkhtgje.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gghchksjm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjltfddgm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gaqbyvfae.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/ggjbzgbxf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gvozuemas.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gkxxhmpkb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gmutgouif.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gqabnlxes.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gwzpkblef.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gkidpxuvl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gtplnajqg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gsjxryqng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gbutrbjzg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/glcpcvcqn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmtgimkuq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glyksrbit.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gnyhixhvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghxdizsxr.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gksmzrkwg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gqixzjawl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gqfootino.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzfmdmcom.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gjqjdraty.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gurjhpyah.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gaisnzdsm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gtbpvdwiz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gpuktuokf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/ggwphzluk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gcazeyidj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gltkrsmjw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gavlzmaui.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gplsguvni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gpixvxpyv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gghybhwrk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/ghdfjsigv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gczsneksy.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/guvufcuep.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/grjiuoszu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gwnsoflfi.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmzfrmqbx.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guyltuqaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzhxdxrtu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gcrpyfreu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gsibzenii.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gsaivbotf.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/ggmobomdu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/giuioxdzo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gakfvchrs.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gbxxnjecj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gkssjkxvw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gtxrhsgbf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gcbsdtbfd.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gngphqlxp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/ghsfkdeyv.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gnqsfgcgx.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gapcpwuaj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gvvxddjtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gbgzblwje.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdjxgwy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gunxljbec.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gfzwdahbz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gurnplwmy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gmcriiraq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gwoaqcswf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gjbmizaqt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gviekqtjh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gjdpvzpls.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gykjbueyv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gaefutgvk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/ghgpgrfhr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gbgaxinda.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gyqtcpvuj.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gwylizkmu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gywpzduny.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gjwtmekkp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtojaalwb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gjdrgrked.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gxlpccfnr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gmsxxpwsh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/grmicsddi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gitssdpgy.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gabzguhwe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/geehnczti.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gymoecvzi.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/grtasnych.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gwfkhiati.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gdqymizby.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gnxybkngr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gffhqrsnx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gnkobcgog.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gueozwtid.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gjidzwops.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/ggungklzg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxikizie.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/giiykaagu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gmscucvdi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gzpnhrhqv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/glwnffmkr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gexdqcqhl.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gbtwcvxvj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/grgetwdgg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/ghakpjnta.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gewlegdch.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/goanlavcm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/ghgnnzeel.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gtfwfswsx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gsehrgegu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjlrvmgmi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdpvvlxvd.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gmpvcabco.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfmceyihl.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/geambnyzk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gxsgtdzlw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbnsanmmr.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnzwdqldq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gxvdkmqlu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gvfqrofgc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gjnqjlgst.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gxdoyzwpd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gfhcxyvvy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gojborwxf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gquvgybty.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gseudizgg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gbvxmbank.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gxxaownvo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gwkjdqgyr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gguiarbrz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gwyqcearp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/grbykbgrq.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gpntwhpkk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gulagojmp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gxtydnvpe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gxifcaggj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gkwdqflzh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/glhdoarzt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gneugofqf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gdeslforq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gyedkputy.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gwpcxjggg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gkyoptghd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/glzxkjdie.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdqnftjkp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/geavlqkzs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gcjugejpv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gahprqlwe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gtinchmqx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggnyzwmku.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gqdsgdhqg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gjtfowukn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmblkkzve.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/giwhterqi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/guzyeckfj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gfcfywolq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gdxdhjcxy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gcxctltmg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gtozpuxhh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/ggcveshcl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/ggrmpkewf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gdqcikxvt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gtmhgnpmh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/guqszlygz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gnravmqwv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gacdssueq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/guhluerqt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/goammress.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gtyufjetj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gerjpchmi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gwfutbrtg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/geyxovbxh.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gcianaats.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/ggdjugwqe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gapxoxhlo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gyjdrqcow.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gcelqeorj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gozujcsfd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gtpykwyuu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gtogobpnr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/grrkddlcq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/ghnhpyvxi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gmrufhahs.sHtML


<!-- 参考信息 -->