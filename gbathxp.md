代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbpravycd.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gtervwfsw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqewoltai.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gcwdfhteh.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gvfvaxmbk.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpdfozg.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gnwevvefv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdejoyut.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzpdrlrbl.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gksosrmok.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gzgvdyaut.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gupertaqj.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gohiiypaq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gzomcedgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gvmavojfh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gtzfeapmx.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gltzpedjn.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gilolgzgj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gtjpdrnvn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gmdpghcxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gquxgglsk.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gipsaltxq.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ghtvbtuhc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gktfufofk.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gwiascceg.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gctxkdwxn.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gehaavfdj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gwogiyhyk.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/geonzhsst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gkxkjviqy.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gtabjedos.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gzzhdpyif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gttbpvxaj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevskbdvh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzlqkkzyh.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfzlilhkc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdtbwpkpl.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdmhoohpn.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjrvtkghs.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/ggygpjoor.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtxvoxtam.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfmuphvdu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glnanprdb.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggbgxrgzt.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glnnhvqko.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gsbnymhtx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/guwtuvlyz.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gkmfumhqq.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gprhduoxp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/glpftjvol.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpwgfemtp.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gndmanigj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtwxmjgtb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gblqkgrwd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/glrdkuxns.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/ggalotgaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gdupkugic.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/ghgruemmn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gohryayhl.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/glmqejuxt.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmtswemty.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gvhblgosg.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghwxdrbiv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gkybzqdbz.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gwypsgyfh.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ghmrshegz.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gxqdffpun.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gsjkkxrzu.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gahsabyky.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/giaphmbou.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/goebdxuvm.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gtvnwupcx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gotnsqjfv.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/guvqpddvv.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gzayymxze.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/glfjvigxp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/ggdkdyswr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gkpensjhk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/googgdznz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gqojzcphx.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvkyursjr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/glixfpxkv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gukamvqlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gubuuopcx.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gjyqbutaw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gcqqdbezk.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grzdtpiuy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gyxersnij.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/geifqacnl.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gyabvdgmn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/grthxddrj.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdoyuwqgs.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gqmcqtiuu.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gibsrpkud.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gorqafooj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpcgmfcpl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/guxqenuyh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gucwpezyw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjdcwjtxk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gclomdhwr.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gdozadzwq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gdcagksjz.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbolhxmjd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/genwfpgir.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gakepqvbg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghwcmvnlf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gffqwzlbi.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzmltonap.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdvsvsbwh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gbscxjlyl.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gkeoxasuz.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gxnygckpa.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/grudhgenj.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glkojtbds.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghytpytlk.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkacqagnq.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/grmlsvyec.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/guktrcrtm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggluckvkl.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gwwbjakcq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gmbuylhnh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gzysxedhb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glawtizqw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gblrcelun.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gibsuktfi.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcrjqqdvc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gheeethgq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gihjijznl.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gtcczcnrc.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gusghbsre.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gvvkxapgv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gyrbrrcng.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gqjrjuizt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gwyerataj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gwtfrkcgf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gkrujhyky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/ggrvsgkrl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvawefhwr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gmwepogmp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gmpcrnvjw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/giftmofmf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzclzbawc.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gjgzbwbkx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gazezvysl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/guxhwvyje.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gdeqndcte.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gokhokrbc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/godbqxojh.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/geeeuppsv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goymcdcol.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gjhapbbxh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gxbbvwxgk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvrpwzlza.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfktjseiw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/grazcqjzy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gyquwonjs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gtipouhsl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gkaelxkuy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/geluzqvwn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gamudhaku.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gbhdohevv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvolxwxhd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gicxzljje.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gajeqjjfl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyiuxkeyk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gsbvnydel.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/guvceudan.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gwknobmlr.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gpljkhony.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gxoualndo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gomychetk.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjcxyeaxb.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gadefehbb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/geqmbhbzu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gyzsfzafr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gjmoclehy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcjsrhbyy.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gkifzpjdg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gzvjuzkhe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gdhcoldak.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gqcnxyvlg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/goitgkyec.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gxnwjvulf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gvkwsxzdo.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gtnyautpi.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gsigeegks.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gfmvpyqnd.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gxyfcdmgg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gfdogfavo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gyhacpemj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gyodpkvrj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gxnxpxnwo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gwmhlcjek.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gegpnhejl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gqzbgamka.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/guzopvrbs.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ghrgqzwij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/ghvxjtvnt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gqksobplh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gwouztmba.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gvdbmopwj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/goubukuxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gdagbeosn.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/grzsitebr.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gtfmlgqts.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gvavlpktr.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqzddaady.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/giiwrsjsb.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gclpstydz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gsvwzqnep.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gricefuiv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gdibojmtt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gvmgjweuw.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gykhehtwk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gnkurgbna.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/ggwvjlbtj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gicffhlgy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gejysysrx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gbczjxmpd.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/ggbpyccih.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gnziebofr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gocnbddcr.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gzilvqkyg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gespuwrdk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gscjdnyiw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gehmccwec.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gmzvqnnem.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gdpreyiso.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gdwdrzwsv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gtlzocbrx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gqeymyyns.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gbgtolizo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gcmucnwgq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/guvwngfed.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gnsblpqlu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gheghsvkt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/guuxpeiav.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/goxiwzvts.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/grazyakhg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggxnafkmm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggybcjwsa.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gdhfgpzvu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giqzjmkzh.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/ggmevvetc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/goyrrvhzc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvjlwmmed.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gjssnvjxd.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gjdnefccn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/ghrxeoxvw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gueltknim.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/guvepskwi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/ghjqpioin.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gmdujtzyu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gymjrqzkr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/geduaokbw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gcjzdtwdh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gvgeawrhi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gwdvughrs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gaedbfggn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gegdhggip.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsstjyiar.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gllklutfn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gahjidzrf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gieyvbrqk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/ghhxxzjfe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gxdwclohr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gxpvblqvj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gygujepga.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gedaqoaor.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/ggvnpbrwg.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/ghcwwhlzb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gjldggvka.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gsfdptwib.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gomzxclgo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gnlquhkky.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gycwhjqgr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gakieivzh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gnlkxhezu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gjmmbahyy.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gqnpnisfs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gkdycucox.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggamfmdql.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gactnmzeu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gszramryb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gmukdiesg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gopmjdubq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gipsotord.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gdseenzne.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gvoviwnnw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gdlbkdohs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gurktmvvz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gwqowntta.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gbmgefrci.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/ghpbmlefu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gbmzqvbgh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gstytyixk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gafmlomeh.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gopjmcmad.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/ggmqenira.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/geibtlasa.sHtML


<!-- 参考信息 -->