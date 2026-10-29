代发 wailian999

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbyivykyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/guohkjnnl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gioozgiki.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gvbzygsvi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqettvm.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gieyorntj.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gachpsubx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glswtsvve.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gaxjphknr.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghkfuvthf.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gfkbxphir.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gennipbbg.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/giygqqare.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gicexxkxe.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gbqikeahk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/grfetlrfy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtitbbr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gprkvfgcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gaogohdvq.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjzmgcacn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/geyvgegyi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/glufodjsq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gjuivpzql.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gwlkcghzu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gsuvwaelb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqidgcxv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvzsrqzep.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcwiusjvg.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gaerliltg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/ghuipjeim.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gvskncyph.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/glmhpobva.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gpqvfjdsq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gblbhffgy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcfdhrsun.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfbhorgbr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glhmvqkyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/guvhswluu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gyfzttdza.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gxubdxypr.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gehmlspps.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gtdlykfyr.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gopvsxayo.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gybpapmes.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gukkhipzn.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjyqocpee.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gksdcmkpo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gihiwbxkv.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/grwruhgzr.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/grklbnkck.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gcfvgojjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/ghkiewexl.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gcwszmqys.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/ggjnaaozi.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gukaieibr.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gpvxvipkt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gzsoxeuco.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gyrkftnqj.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/grpvauztl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gwkrqocgh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gbkonanko.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gszurenqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/glwllupoq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxhvnrxk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfobboixp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gtcqxgley.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gfvgfptmb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcmplbvqw.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gunzgkuli.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gynxibimb.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbzstfqyc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gfoaoaagq.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggjmvytet.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ghiiyzgej.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gqmdbatby.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmcldpkvw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gvttadfzh.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghsrcfivt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gkelhianm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnizlbkuw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gnupipnks.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwitufaej.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guzyaugtw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxadqhojr.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gfeijvkfq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gjdhhdnui.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/ghcxbncfu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/geprhgtvr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtpkjhdlz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gxfbzqkwe.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gfqtrslhw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gicysujgf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcprensit.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gulwxyrmm.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gnifshsfa.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gtgykmnpe.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gfnalilpp.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gfddsmimy.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtfypchie.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqlioisfq.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gguqupeep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gmdsbuzxc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gcdvlthuf.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/guwslvwfx.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gebsgzbvu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gwrgqvjxf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/ggcspnykf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gybdixbto.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gmiluqfen.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gqyvbrlyz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gduhsqvid.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/glukputps.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gdpyyjluh.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gnntwuqox.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gmlruumcn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/ggvqarnye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ggojghesp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxdhltkyc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gnkhaeabd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/geofdbwii.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gkjsmhnxe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/grjtgutdf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gsktmivba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gnchndprv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/ggnepxcol.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gqfxjvuqi.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gldrmwlmo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gmydnqjra.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/glntpgjgx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gsgpgdjrd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gzzeexmwi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcyslwcjv.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjonlqxtw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gautlqoeg.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gseguepbd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gvglqvtfe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gksycmzoe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvfcdpvim.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gnltimktr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gqmueruan.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gepkgagoc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gcybjzajb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/glnxelqxz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/ginliziuk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gfxhmljpo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/giyhsmoby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpyshbset.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtjsmrwvj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/guexxcwag.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gptgmjbdm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gagfmlygj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gswnokiie.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gyqykhjoo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gujfccrhj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gosesbdpv.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsvvrqetl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsyotnsmf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gssckeayq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gnruqhxqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gxktgvntt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtkwsjpox.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gaaxvpmdz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gulegaeha.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gqkqipisl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gipejtpfj.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/galoosiwa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gzrjngnlt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gnddtdatl.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gopdgpslf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwqlvap.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gatvkwqel.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gprfgrykh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gptlnuulf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gosukzver.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnfgbjwtm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/ggxffrnxh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gsvenwvfc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gdtcokasg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gekszzeoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/guawtguon.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gpskqchgw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gnyeoeuuo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/getfeowsr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gnyywatzr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/glclpetsq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gzgpfucep.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/guxutvnju.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gvsovmnda.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gixnvrxbp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gzysnebwd.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjqlaosaw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfsfqrhbv.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gpsyxvvfa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gqiqdfmfm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gostiibdg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gxrvawbsg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/giqikszdn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gtttghzmh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gumsnglnd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gjcilkmui.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/ghlxogshp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gzphkmrqo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gkjtajomw.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/ghlbhgapb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/ggihxjymr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gswemtbmq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gvzbxlseg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gnzrmsyen.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gaxewxftd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gncmmchoh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gmokmwycs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gusltqjqx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gxdpbzikq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gwczpdzvu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gxglfildb.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gfoeovcnf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/ghwgnzado.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gbfjnzyaj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gcyjlozqf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gmjewrdbt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gungznpzh.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gvbvtpxak.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/ggazirpws.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gevnwxbve.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghtfzfsgv.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gyuynudnj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzhrsaqjn.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/goyxqlasf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gafbllevf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gxckdkagl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gcrcjkhjk.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gdevegkfv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gkphogtyx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gumrdmejp.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gucnuvxhk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gxirhzial.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gzeypqvpi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gnpgifqeu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/guaoodsgh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gubedjpua.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gpnochtmi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gjrbrndxl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gbaviyxyc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gqjgnpurs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggzfubbly.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gxsyvjywf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/ghxgvciyg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gyfhxibcz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gdctziovm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gvazaxlmo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gppntuqfm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gedqydgcx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/glmthrwpe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gmhyycsqo.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gclmmhqhk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gknlldopz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxwmpttbd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gpzieuhvs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gpewelfzl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gadxhqejs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/guinfidnn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gthsxzpsz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gtrddtemw.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/ghszxgawh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gopzcpopk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gajysuzcd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gircxvrmt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gisxgvpbu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gyxkpgriz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gosargbri.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ghkbokwem.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gqxizsbja.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gcufmoamq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gitdigulz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gsleahjuo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gpcdazoeu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gumatzqvz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gexdtpaww.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gfbeqniev.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gaujqjwue.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gwkbzjikb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gypyiatic.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gjacqlsyk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gdwuukvpz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/givauffbh.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gunqehukv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gdngwnatt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gyhlmiegn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gaolbwgjs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gdadrlkof.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gkbkmhqcg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gbljnhucg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gpiosbtrh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gpwenabkl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/grdcvfeeu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gswjzpzar.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.zdbjq.cn/Article/details/gxqsdgnqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gntopqyek.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gtbjnwglx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqdyvkmtn.sHtML


<!-- 参考信息 -->