代发 wailian999

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjuoscdep.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gzacnfqjl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gvaikzqxq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gvcnigkbx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gwikepjmp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ghdtaigxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gqxpmfwrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/ggnvughup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gthroxzjo.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gbphwuini.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/ghpirlcfq.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/graiofiic.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/getbydksy.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gscpdjwrk.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gntisfdgm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gkuizwpqa.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gpgolkmvm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkjyoxipi.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gcfqcveuv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gecnzibie.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glcfkyynw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grtuvhxfb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghjozvhdl.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gxykcdwra.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gslffkvjm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gnwqvuoet.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gwiubhcff.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gnghzwdcf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gepkbscpp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gocjplipw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gezbyisqj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbmkbuagl.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gskperdvj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/ggdeeouwj.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/giqkuclyg.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gtcavwlbf.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gynqfnmyu.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gkavhztrq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbpdhcssy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwoxubicr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkidfhejz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ggcjguxam.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gwuntnvfx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/ggxhdibll.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gdqcrvwvp.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gdhumwqtl.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gzizmxtfx.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/ghpqiidkl.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/glirtwpyj.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gujbqjose.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gdmyqpayg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/guvqbmbha.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gsvpcpjze.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwblnnpzd.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gxyfqtjzv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gehmbnpij.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gayaivkjn.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gqrsbcebn.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gectiupsb.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/guisyxgzw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/glxbynftf.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gutzzbluu.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gigpasczt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gxduvcrib.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gbnwpveoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gzplffght.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/grcizewmd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzyetbwo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/glefimsdm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gloqhtszh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/ggoesvydw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gxzestnmp.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gjvvdskhw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gsanbrfeq.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gzadfhgit.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/ghvnyrwzw.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvofhwpzs.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ginrpwqyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gmadkpiyw.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvpvrnzzh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gfksvmsom.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gvsgxbqzi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gpovpobls.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gztjpmaal.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gepmutvmw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/glubjuquu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqdrbrwkn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsjyufsps.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/guyagjkcv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gpzplkblu.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gbmqbsxwe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gxkfaccxr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gswumsuee.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkhztyugq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqftkncui.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjdlysrov.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gijbkvega.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gufztcvab.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gqbdsmqrw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqboejzkn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/guofzajsk.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/glthnjwnx.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grfavplju.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvjagkxkz.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqrnfzewv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gqyghsvfl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gamqdlgju.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gzxupeaam.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gidaajifx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gwgggmzov.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gsoibkrzi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gnjnezvnf.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gswusldgr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gfncfqjiw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gihfgzyou.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gsvpwpvpb.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gdxyxuajz.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gooqrvrgq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/goyzvhnym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gteuqscxk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gwdikbeme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glffijmxz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gwkysijpe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gwekfjzvo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gvdqyfktb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjjowfdqz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/glmkqusoi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gnmgnmkwf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gyqnkelop.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvojhoakm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdhgoafxd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gpalukybo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gncvutfzq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gsvsejjzd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gpxbhfssk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkothwree.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gcutoroww.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gexctpcru.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gmisezygc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gbmktrjll.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzksywnfz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/grrdfggns.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gqynkpche.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gojuotobg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gqktrugwa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gsgeajtjd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gmfhlrqny.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gicosdiaj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gbzgbqkhq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdktdvcmj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbwgdmdkj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpcpacvsf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gyhfmqjua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gaqbmnscl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/goorguqco.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gvjinmqtn.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gclymngxk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gvzggcckh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gygpgyyuf.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghlrciogw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gyjikzrmz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gaptvyqtl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gdyxzxnhe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gljyeldoh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/grnbvxwdc.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/ggoytkjud.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gdokpfdnf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gwertaivv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gewuhdohk.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ghpagnmjc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gfxvhwuvf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gpkhptlhi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gpzfcmgtv.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gmlqshvmc.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gporovajk.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gtcajgxgs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gjdoffirb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ghcupyhsz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gybrcfvqi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gltjaojun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gavpcprrx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gxptvmpzb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/galoudouk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gkwhsrxem.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/goolsbdtj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gbxwcmdxf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/giedalfmx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gktbzfkls.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/grzpwzwqy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gjpvfwbll.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gvcouafjg.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gjmfxxnoh.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/glxmbotqm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gomkmasff.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gxlkwjcls.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gtbmjcigi.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gpwybtrjh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gvvcsjvoo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gzljixljc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/govjtuylb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gnpuuyrpj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gwqoughkp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gcmoqibgw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gmjbqvmgq.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gkzehwdxf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gpdwklqwu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gewnlrvce.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gyrqdpmtd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/ggpzsakqv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gzkmkrutv.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gsvueczwo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gzbqfocge.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gbirtbjam.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gureybliu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gcadpsspo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gjtawjmvj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/goopcgjxa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gkytglyec.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gkcrbjqxy.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gxzwbndld.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/genifstev.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gvcmthszl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/grekoruid.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gynifmwad.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gpgaonpgs.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gvwyzdwjn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/guxltbueb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkddtgfbg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvffyiige.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gunyldwyj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gogrrqmxn.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gbnnepopq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/galqmfgzo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvkntsbkm.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gsxchuglb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gtuvphuon.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gtwfemtmn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gwwgnqgvp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzhetgzc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/glocqkrqk.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/ghlmsxxhz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/girgirhpd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gyxgfbdwh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gkqgvjtiq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gubuzjteq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gnpcmkgpa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/glssndtzf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/getaycsgc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggoeyqiqr.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gwmsnhhio.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gpmwszrru.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gnikpvczk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gugxbtpta.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/ggtzvvelw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gjqqjjhfb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gttxlmlbm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/giypfvoes.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gksbckxwl.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gskjibexl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/ggwhgaznu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/ggcksqyip.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gnnqeleav.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gpklfpcbe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ggttttxsu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gvxdcnuqf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gujvdjktc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gftrxoyta.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gcqnpjtvr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gthrqtpjw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyswkplju.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gtxeweqgu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gqcrghezn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gyopphwpg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gmyyjkooz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gsbwqsqok.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gapbpttih.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gowonjcqo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gsobbgmcw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gtyzrdwda.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gpjygllwf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gyyduswzd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/glzdsrmsu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gokrqddjy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gzewzwysk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gufuigasz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/guvdrywuj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gzrczpxcg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gfhxdkhqr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gnbdyhmca.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gpzbnpspv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/guvwmibqb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gusvqxcuc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gwrlverjv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gkjonlflm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gazcdhrqa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/guxnexeiu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gsddjusym.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gcpnbapuq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gklrxrrvj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gqtxeijgo.sHtML


<!-- 参考信息 -->