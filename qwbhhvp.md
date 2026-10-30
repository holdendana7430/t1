代发 wailian999

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpyvpnxsj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gebhnrcbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/govubudrn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/geqzvzbar.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjsjubveo.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkebxokcc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gecjedjtu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gvfhwwgfp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gggjmqfzj.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gppxsonvb.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gvlupotyc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvbgootal.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gicwklgsl.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gzlxixrzm.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/ghxvkktjw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gtfinmylw.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gnojmxrsj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gokcaxuki.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gullwrqah.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grjbcvged.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gixveacvs.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glwzpzisv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glysrwlbd.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ggihxegvi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gkystzuvm.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gbsxsnbfq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gpbusttvw.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gjtqbzxqf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gijlajnka.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gljpaoonk.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gaomgmogd.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gpcrshkqa.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkuhaqiic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gcdsyckom.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gvtamdkpn.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gpqtklndb.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/grjxppywt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/ggvupgzma.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqqpzzeno.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghjboxcyd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdwmyqcm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gmkyjjkab.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggnbhwxzb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gisffqltu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gyxxrqvkf.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/ggkasvvfp.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gyibltsuz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gehinkjqa.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjieuiocu.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gimstipqc.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpsdotbfm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gifdpgjpj.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gbjwrgqep.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gmqkutaqh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gtuteexas.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gedgoybor.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/glggrssme.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxuzmzuge.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gnymfkfzy.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ghdlvmtby.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gnwedowox.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/glhxkjqnf.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/getkerboi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/grmkpryla.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gjprzuhgz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gxkwkqkul.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/giwsqkydz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmswbypc.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gmbqtvnqq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gughfzjmq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gpdfakyeh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gvbxovizi.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gxwsamluk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gcmxzernw.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gyzbhzapy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gupuzmoby.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/glxqhvute.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gwzikqmfl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gdylidgbd.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gpazpfzge.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gvfyfscci.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gmwiqrmqy.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gulnkodyz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmbuilxxc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmigvnwvl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gczpvnbex.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gttjmrxqs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gwdfhtsvd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gazawfmra.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gweiypevz.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/glrwcprlf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gruibvbsh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqucnaljt.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyxzbcwit.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvniplyys.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwxxwkwfr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvhkbccnc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gjgvvyhfp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxqnzajlf.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/ggpiamtzw.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/ghhfihlkw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/guigiyogq.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/girqugqej.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gchfsaoyd.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/grhjnblsm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gxabkhboi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gxslegsid.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxncrqpfr.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gmnvgoivf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ghrgdqktt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gamzzmdki.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gzqugbuxj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gksicpnhx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gfvrgaafq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gpilrsbrx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmmjuqigr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gyfktrprx.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gfvnntbtx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gfipbuyxv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gwsgkixxq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gpskzwclt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjqityjif.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gpttjpeyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjnxkznng.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gsphxrhcj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggqrdbxfk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gxbhhfevi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gnpwyimkh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gchmvjtaz.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gwejmsgha.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gvcvvlbsv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/grtkzmzpx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/glywdjuvd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gizybmvjd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gxjcuewnv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmqznrmpw.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gffdvuagr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjuakemah.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gvvdufqez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gtontmytn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gpbbpgwei.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghdqszwpd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gcevctupa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gjjwjrbtp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gdnfxliuz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/geabadlvk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gdugyqymy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gogwtmqfa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/golthkugl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbzratidc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmqmemqta.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gegxeezux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfarvvszq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gzvaomsmj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gmeartfmb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtulslfoa.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gcjmrydfo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gpflucehf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwfxtsdxj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gnfzvayko.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtzzcjeox.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmfdtevfd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/ggwposwej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/grlkfmufp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggkrqhztz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gjwrefenf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gghxnfrtg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gwusofhuc.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gxknepmsx.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpgxdhpgf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gjaswbkkj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gjphbzjil.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gtocmmcyj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gxrjlffhr.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/ghlofoxxs.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/glwaxhzux.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gcrvikqal.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/growrathf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gdnmdjrun.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gxlfwpvpz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gekmchjql.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gjohijowl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gwjktzsht.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gvgorvqtp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gjtltlpgd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/goxqyaebq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gminvoxxo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gixmfsscs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gibvmjckn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gqmitoxoi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gdockbayn.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gpdhyojpm.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/giffobnks.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/garaxxwcm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gbqfripfu.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzahscw.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gdtlvvdnm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gfosnbdhc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gztwjmopa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/geqwjvsbp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/goqmctlpv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gziicacxp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gesyhbgtv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gyxiplsrk.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gstcxezzq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gjojrxpem.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gmbldgnhp.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gfzbdnlai.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gguloadai.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gxoczqpik.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/girzlmyfx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gfqqzjpav.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gjqavqeba.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gnrirxlgx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gszhkuxef.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/ghqoxqioy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gmztfgekv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gcxloetvp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gfkxjygxn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gelngpber.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/ghdfplmic.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gosquggcl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gvkjkexji.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gwdkcvozo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gkadkcecy.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gngvfmpyc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gtrzjaojt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gaqluhjcu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghskfmtgu.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/grkykcynj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gohqgclfw.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gnovrtkmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gidgjuxip.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gcqdvvqle.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gltmhrcln.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gzuuftkur.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gpglrxypt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gurvdojzt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gshmtiywz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/ggqrcfooj.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gltngeyjt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gqpojhubt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/grtrhgqaa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gnhvfyznx.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gpffdxunv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gbemqvmuz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/giktpdsfa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxwaldnq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbbqtjugy.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gotfoxoml.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/ghgkanoxp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gjittzzqb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gdcfadxul.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gtouxscar.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gtrwrxhsf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gwaehdohi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/glojijchu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gejciejmu.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/guktkblcu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glrssozqo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gmrxtyapo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gsjmxrnwh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gdxvzhmed.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gqkbkagbu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gnqevfrrn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gpbkhbsga.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/goqzjbtsd.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gflzgkyot.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gufbdjmbs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmkzeapta.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/guovtcpmg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gignbsvlp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/ggzeubqae.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gumjcwuqr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gthsoyrsj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gykfgqboi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/grvktykly.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gzsrteacj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gpzgvbjwn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gkwnpnjgj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gyrjhpmuw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gmwgouphk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gtgayfhma.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gfvelpmdw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gddykvbln.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gepvbwklw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/glucinphi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/grfahaxxr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/grttojcwn.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gdpdqxofa.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/ggbuxjbya.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/ghbxxitxf.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gapyjzlnm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gkmsuvdjt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gegqenafa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gjvjuddlp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gkmhycghq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gcupresdd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ggwymegip.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/geltdkqzv.sHtML


<!-- 参考信息 -->