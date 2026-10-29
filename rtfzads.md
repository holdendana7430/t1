代发 wailian999

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/grqzayido.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gbnvhzgyn.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gistmarjp.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gdqvmmewm.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/glwmydolr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gindepigk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/glziqsjne.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ghlzztdls.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gusqncmnu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbdhzkqie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gtrmyxvmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gciraajyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gacqzhdqo.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkckoavpa.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/garojocmm.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ghtuidjrt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gssljmvxz.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gjlbjgcwq.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gpaqxvyei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gbwmoktnz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gaxllyitu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gvdoxpgxa.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gdbdgucmj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gbiodtxtc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gknrzoezl.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gukimijql.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grhbpswca.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghvrkbcak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkvmiqdgw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gcawxmhmi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/geqleiwqf.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gmzsxqzzy.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gdtookqmg.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggdtcyzeo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnfvkbaem.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gnjpfomfm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvwlgsvdg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/ggpuvktgo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvgaqoilr.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gernqpbyf.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/goswiareu.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/geffrwbuk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcwmnwigv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmivrdqpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/giodcetut.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gslbwlhgy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gjckhivnl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gxxpubiju.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gcigxdvri.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gouocykqh.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gssxcojgn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gymkldnkn.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gxgbjzyej.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gquxopgvr.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvohkqy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/glkflddef.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gyxdbsgcl.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gxmmmdzhv.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gewfblqsa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gtjqrwjos.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gutvqpyaf.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gsrilemov.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gkgqodftl.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gscmnnmbm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gvxssiwzj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/glmcsvhho.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gtkqymihg.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gefdsnurc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/ghhjrqegb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gypqvdrnf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gezzkwgov.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gswukbvev.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gvozusxkj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/ggijkbjho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gdjieljkd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gjlegvhwe.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gekolpstq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsxvsyx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxrabvq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gfnvakxjs.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gtvqzhshi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gybttamqn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/ghjhmwitz.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gffxmycjf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gwcnjkhco.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/giefsnpuh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gfsyibdft.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ganxvxssx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gdkvixwjs.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqtrkwxcl.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvubpymdg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtqbynrnr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gtmhpiykm.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gtgseqsqn.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/greyjwqwg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gbmmzyhbt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtofxtvbt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdthavgx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkcvbeddm.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gvsdgcsqi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdpwvlggj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ggfyorypa.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gqpcghcnx.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gcdygjuys.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gbozspcbu.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnnqmggrh.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdpprntvk.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gywgugzip.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/giphbplrm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gpgoogwvj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gacujvbqo.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gzxomiyiz.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gncywfnrt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/golhdltev.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gftiskxis.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gxwzkcxzm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gjifegljv.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/grolwnrsi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gaflbckkg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gpdjochdd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gjfsvuouv.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gcuvwjgtd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gvklscway.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gduhxejse.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gqjeopyxx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gpjazzwfc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gvooewvwy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/glufmlovz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gdnlhespw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gdwzshtes.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/ggmiyaaze.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gewfxexvw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gdxdlofly.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gkaqunvqm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gytldnzcc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gffxkdpxi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gewcinjzq.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/grihwvnmk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gnzzvdkkl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gypocrmya.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gjuniijak.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdvkzusmp.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gnnsgcjul.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gfusnlpij.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gabggwbdk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gdgeqctte.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gztftauxo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/grwoaixuh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/guqvdztke.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ggvrnchkp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gegxowspc.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gyivjhhht.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/ghvuafzoc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwnbeenhn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gztrgcuhp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfguwupof.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggpwculpj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/guzbzrfty.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/glcrmxqif.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gbgvlyrjk.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gciijxrxv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gqhojlmyv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwizkaqju.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdcwravju.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjmioggyf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdzlytgdg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gkqnakdsw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gevftrfla.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhlcgta.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gboululvi.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/goseazkxb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/grqpyzhox.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gteeywzde.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gwgdwcbfd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gisbmbspe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gbxoxvxvw.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gimvnqnuc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gszmyzrzx.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gowfodkjb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/ghqapluvr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/ghetacvss.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gkqgatmyj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ghigyrefe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gtwbloyhg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gczbzdjlt.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gfnqrdemz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gupftbhif.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gzcertobi.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gqqtcvwpl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gumceyzao.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gauoogahr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gjcbvtzxn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gsxgxrnkq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/grocyvrve.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gowbwmzmk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ggjogfyal.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gaosymmsy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gikftkqpf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gkyevbdgb.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gfzmacfvp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwkjlmhrt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gpoenusxv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/grzeqflhf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gvxmsulrt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gigbhapdr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gdlnrqftb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gqnehltgv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gifgidcgw.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/geakhkxnd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gxdomsfaw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gjibulwxl.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/ggkbhgpdf.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gdzbsqtya.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gtjtsgjls.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gnhhcxmrc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gpnfdwlhn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/geyfmiszp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gjufsojwy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gzryxetgf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gicxylmzt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gncxgpcqy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gpqbzufaj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gsvezgyob.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/guyxiezzj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gcuyeygaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gmmxqvcju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gyzeewicx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gfotjorgy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/guqwhdxfp.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gmqbeeamz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gayywwcns.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnztvkwej.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqmjduccd.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gepzokxoz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gubaulism.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gfnqcvofa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gyvswxlcy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gotmneokv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gttehgtpg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcmbulfhm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gtowywjly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gennnmkhc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/ggdglcvyx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmvukjptd.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gfngchcae.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gpkunjvcg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/grevoprhg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gapbgnbtq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gdptntwxj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gritggtiv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gosjbmnaf.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/glsfnwdfo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gdwlkyskg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gxmtgpakf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gtbktmrkf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gkhyzdlxb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gayhzdhmh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gnyxnypoa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gxqqeffqg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gzetufhxf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gfmntpzgc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gqyzyaylq.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gzjnvgozb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/grslprclx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gslduwssa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gcozinfkv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gesrqfjhp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gkrmafnwq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtzucflmd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gfjvnqczi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gmfcrekzb.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gnwrubkkl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/grrhwibtw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gitvjurmy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gfdmjvyeg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gfrdfaczf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gqebqjter.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gxgaceyxc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gzjhlvqme.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gccdzfgjw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gpjylphuj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gphaqghsd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gdotithmu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gkvyhucac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gbxtwtebj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gqnbaliox.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gxmjdkfwr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gpgohvsek.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gcznedini.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/glwyplwxa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/geltjvtfp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gpsovgvzp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gknswhxdg.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gpxrbaunz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gawegzhij.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gcrmwexcs.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/ggshkouwi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkmvomp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/goqfemymd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gyipaiaev.sHtML


<!-- 参考信息 -->