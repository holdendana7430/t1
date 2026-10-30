代发 wailian999

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbykgkswb.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gxrrrlukq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkuniokfl.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gwvfzbtks.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gcjqemgdj.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggyxodouz.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjswxplod.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gnntyqany.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gstrqybko.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gprspsjlm.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gjjmqqmhf.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gjtkfrxyk.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gyglbqwsr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ghyglqjrg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gjavvyrci.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gkvvgfkso.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqamoyl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gerfwnovs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gcokctrhb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gelsfdoio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gktgrxgmz.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/ggxcgopca.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gffmvugso.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gueetlkib.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpuipbbcx.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gkxfyvrbs.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gfrnufzxs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/giriydtzc.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gacatjcjh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gutzfhrde.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gdnanisqf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gmcrbtciz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gloeskznc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gqdhhqewh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guboiwuvh.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gwmigaext.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjfdwqxum.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/goybaxnyj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/grpmcdjtv.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gcfttyjgi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gsjjflfdi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcgzbgjau.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfcirpiot.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gyqmhzlwd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxddkfshb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gdyshfnlw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gjdswlgye.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gehxxvptf.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gcupexomx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqhrvxbxo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfvakqjoq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gottqesrr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjnnpzkej.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfseweckc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/ghmyeeifh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gqpfpawrl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gidyzayni.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gogpkbsqu.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gwaxcpkdm.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gkzwbmhpb.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghatwnkph.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfumbgihu.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gchhwvekp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gmkxbbwxs.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gwojbndox.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/ghmjzekgx.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/ggyqauazm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/grkskudri.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/giylkmhtv.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gbvzkabfu.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gusiuvosj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkgelcvsv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gtxrvipsj.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gwbrhbaor.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gsovkytuy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gefnwxcdy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghmbsitun.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gjblvzbso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gubgmpyis.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/getuuxjyf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gywgqbxaa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gveprxxke.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gljryqxot.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gzxzuwagb.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gtmfdnbor.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gktesotqb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjxuqktwc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gaggbavbk.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/grhcwlzda.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gpgbaxtky.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gjpssonth.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gnepxdphc.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gdfwcspjg.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gzxzqmzew.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gavmzrfke.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gagmqxevr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gzhtrpyia.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/glbbzewiq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmfxkrjob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gnklrrcat.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gzeeowkwm.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gvqcfmncd.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gcuttzirt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gwouspjlq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glkjvkamt.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfumbtuxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/giiipsvuq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyltqyexu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbmnmzqna.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gctjipbnh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gdepwnnok.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxafbwitg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gkjbgoaei.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gytobitoa.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grfmtnifv.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxujhcdns.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwxnygmhn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gweluseqi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gnbdlvwvu.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gklojcslc.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gutnsbqwp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gzsqewllv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gfydujssw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gxqddzjgr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gmmhheqaf.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/geutjqiwo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/geuxlhsws.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gkbskerkj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrccxkr.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gwjnykamg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gxzctcyov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gpzdqveno.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gsydazzfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjudzdyfe.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gwxrmkukk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gkwrkwymx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gfsrzoory.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnwhwquky.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/glicpgxjm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gfgcpaoti.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ggekbxlyr.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/grflytxhn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcvwottik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gzqezuiqc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gtntqkewb.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gbohgvflm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gbfvhzdym.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpgpsnmxq.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gtsytndpl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guromqzte.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ghjhsojgd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gbskobggc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gciotaous.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gywbaivpb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gmkwffzhb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gdorbwepc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gqrwyozjt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gxnjliono.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gcccbtqxu.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/ggxhghluc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gllwffclz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtkrawled.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwbeeupxy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfeqsaqvl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gerqhumyd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gqtusfqhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gunbtwjqf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyiuakgcq.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gikpwtegx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gjvlaqlyi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ggovqplvb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzjngasji.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gzyslggep.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnrmhfhxr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gircelmic.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gstxcuomx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glpxtwgki.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/glozdurwn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gtccakeww.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gowfxwsla.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmdehntd.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gfmtdqagi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gsizgpwdf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gfrgtylvv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvgcwss.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gcndzevnm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwqcfli.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gqrdgximr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gddyaecrx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gnfdndkca.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvceabafo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gvrdkdorb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gfnkiglzl.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gocgbzbrz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gqrwihmrl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gugjfuydg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gcdefebdt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjamudjlq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gsdypjkfg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grokbdgzx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gyuptvhwg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gernbiutg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/grfgkkots.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/ghujtpjml.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gaufepylg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gxdzngtzh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gghrjhgff.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gzametibb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gqlrrvjmc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/grkvhnara.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/grdxpfsdf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/guqdinjpb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/glklnzenx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gizxwitgh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gupirzndv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gnqilssdm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gjoarpsnl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gzfgqnssy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gkuvaqcxk.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gjturxbay.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/glrgydvzs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gqjilxpsp.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gtzsufoxj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gydstndlk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gsbhckucn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gctpdpmye.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gxzaeygpl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/grwkrhrav.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gulgyjwrx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/getpgsyis.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgvrnwd.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gapigejyz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/ghyusbiqs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/grnwwbcof.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gynymlokw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/ghnfselre.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gjxhdbtoy.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gvlirzkoz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gbwnbqphb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzbtbtytd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpabytzkz.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gfvnmzxji.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gerxuaqoo.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gvoqinnhv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gpyokdfjk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/glukrxsng.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gmyzhbebr.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gflgfqrzo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/groafvhuj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gylngcodv.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gmmqahvfn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/ghpgenaxr.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/glarpjxnl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gyykczcou.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gthselkjd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gqietmgtk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gknuewnwu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gmooauevy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gmlyrfaya.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/glmacptxi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjrzdnigv.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gdrvionmw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gxoiddbgu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gthvpacek.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gdpfbsrxs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gzbofykrv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gsdrceshh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gfonhumah.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gvvdudmag.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/ghbbhbafw.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/glssdsqjx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gtqdhwjct.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gastgnemm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gwszghstt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gutwihenx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gzqgrtkpk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/glckklqxv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gwlfsketf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/glrsiabji.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gkhoxwkvy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gmwtkvrdn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gffdkkwjm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/guillokjp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gpzxglnwu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gnzodfryv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gklusuhfb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gggwcuqiu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gssiwbxlt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gbobcjoqe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/giohqyhum.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gopzkbsyi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gqphvzeco.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gvctjcfyt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gxerafamv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gcfxsqoze.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/glmlmpyff.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/glptdifvy.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/guujuhvxw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gichpallr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gogvolxkz.sHtML


<!-- 参考信息 -->