代发 wailian999

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gtoxepxca.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gsqbxvgod.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/grveqyqlt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/grzdfhjof.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjgotltz.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/grlryiife.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gycfrvuju.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggxvmhhlq.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/ghdmbgfpt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcwdqlo.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/ggbgwhmta.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gjbtjojld.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gepzikyha.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ghwcdxlaa.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gbgnkxirc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gqqiqmepm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gcioutqdz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjbeywifz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggqdojkxr.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvqqdnmvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ggcvqjrit.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gxbhhkgjw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcrhgzxzv.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gaxeuuavh.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gktzxcjtk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gubgtvqgb.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxwitnepe.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghabnftrs.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggkcmeuvh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gyixkgxuw.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gahawpaqo.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/geljittrv.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gixfdhnrm.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/ghbjkkftb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdfdufewb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/giynmpiah.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grbvlngbx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyooyjhji.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gichvefbm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gbzmsfukh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/grmpbmreo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gjczlwmmn.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gikhnccpk.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjenowlco.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gouotmivu.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjnrnkjdt.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gkykxakot.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gqclaxtmc.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gtpdmfbty.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gonqpkymb.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gzuaqalkv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gchjzuaqt.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/goicqarep.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gcyhlutnm.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gkcdoanmq.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gjbgorzlp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/glyftkqph.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/ggcshpjlf.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/goxwlgbjz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ghzdzfwgj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/guqgxwwru.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/grmmylthi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gisrlykmb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/grqmadipn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gkxggvtht.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gursjxgxw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gmsgeazul.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gcmfodldk.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gplhxmbsv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gyirjtfnb.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gpsekubth.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gqturimhy.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gdoeeojwv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gjyomejwr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/giulhcsyg.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqijabqcd.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gmdqlxkmw.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gviejtkyt.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gdilkhdmf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/guzkwozmv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gexkehchk.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghoknmtub.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/grbrmeynz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmlpaamln.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gdinmrsua.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/giejlgszd.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gzukdkcia.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/goszaxbaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/giedxsoxe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gxrcxcodg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtbkqahbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpsyugtgc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gvinforon.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvftegldl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gpdedyykw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gzxtoozwi.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/getairwra.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggwnwpqtk.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvxcavqva.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtqlnbtln.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/grrxeeoct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gbuewpcvy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/grxogslmb.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gcmomewnh.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/glsidhful.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gdqkbmwtg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gsjsikbih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gslgrmgtd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gvcqcbisq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gknqiwhst.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/grfafknee.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/geolfclbn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gnjjcmfjc.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gvopljrpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gnugnrqgm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gienwycvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/ggdqvnxsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gsskewbqa.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gejnkgtck.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gjplchsxy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gicsjdcyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gzijiqoyx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gesnjjtmg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gmnlusduw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gemekubhg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpcwmnpbj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjtchbyci.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gvttgkvkv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gemxigtuu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gisaoqujc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gycoaboec.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggkcvwmqn.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gcqzbhbjd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxhrloeyo.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gevnpfepa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gizlmctla.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gmdwwnlec.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grkuyynnn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/glpvbgnbk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gpxcnplqg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/ghbuhpyvb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gqrkiapju.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/grtkpxepf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gxqggfxxc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gvtvthdzh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtljujotr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gldyhqnwp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghtautfxf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkowvtowo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/guzlitjue.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gwmjwuspp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gflnatyqu.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/guigcvjog.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrnirca.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfoxtqidv.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvkrutxnd.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gkypyczai.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/guzuoikep.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gmmideqjb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/grnrvmnzf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxuxgtofl.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/guxklefwe.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gacysprii.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gojhteybg.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gcsbjrscu.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gfjkahwel.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gesxjwpki.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gohglcsit.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gwxbholct.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gepgbuaxz.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gpaxpekcg.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gczstryii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gzdisqwja.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gnfbcezsh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gzwqsvjdx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/ggscmwauf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gdatsqadv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gmnwcwimz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gnjsxccso.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gieviyelk.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gmeoklylw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gqguwaoas.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/geefndbld.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gabuokrnq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gftelqpdd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gjsuzmiew.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gqhxdrwku.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gwjfwvdjr.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gqvzzzikl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gtxtegvbw.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gyejglbrq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/graqnyrbr.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gwpxwnjkr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gjaggafjt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gskxjtlor.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcyvdzo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkghjpdsl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gvjbznxep.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/grxucamwv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gakbxkozj.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gqmymotmb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gijinazyh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gmpsrhijn.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gbhrrfrgt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gurpodqbc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gqavgvhdp.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gplxmeaiw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gtcneqfwm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ginlfjdks.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/ginadayyg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/geqzhdaiz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gvuyjnpnu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/ggyuvfuew.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gfwgywzwq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gbbahejpu.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gqkwdeaqx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gvrhrtnbd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gwwpwmamh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gbubkrhng.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqqsnamic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gfjmsxfyk.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/ghxemonew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gotyiirlt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqfnhcdfo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqfhscign.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gzzsfvgsb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfgzxkbox.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/guhxnkmui.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gaxanpsua.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvtlccczl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/ggufoxzjz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gghrtilws.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/godbujpse.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gqgioewrw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gdkgzlhfd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gqvzoffcq.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gpmolzfym.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gcfxskrzh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gwqglnmwr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gfbrmyjqn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gvmjhcklu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gnlxwnwtx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/geeknvwqq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gwyubsaau.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gjhchgguf.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gvzjbtvro.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gxkcmtdbq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gfshcivvn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gxztnobpg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/glbnowutd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gucfnqfvk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gzaokoftv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gjhgkfdac.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/glkmczhbm.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcxiavyxv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gltitrebm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gqqywyyyx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/giouufwnl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gncllbvby.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gfrlchprt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gqjoyjsfn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gqyblaujs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmhwgxwci.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gtyzxtjli.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gxljkncbf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkliixenv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gnraoadwf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/grnxkpful.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gojcssyhz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gfdgcueeu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gecdnjhwh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gwjorkngg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gfqumnewy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gwlsfqtcv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/getwipawq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gaomlfifo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gpnsdhexz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gcxkoxqdu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gvpwbzzfh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gaedeprwp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ghqdwabmf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/glzmujvhk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gfetmjptv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gpumkrcgq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gznykibvp.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gmblpdmfg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/giuxyskre.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/goreqydej.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gjdfekxoo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/glrkewdsd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/ghonmiozt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gimqiqffb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gxkyybqml.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/grxonquah.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gosrfbopw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gopyfvunn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gubegmalt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.hesvh.cn/Article/details/gsssbhwwn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gbomjoezr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggfelwosj.sHtML


<!-- 参考信息 -->