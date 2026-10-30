代发 wailian999

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvolaxyhw.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/giutsuhkd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gghkbpzoz.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gluuudgjc.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gmykjnmdr.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gxiezrpjq.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gjjdpkbsa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gbzkngucm.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/grspifvwg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gszwektnw.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gejaoxpit.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwldyfmfm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkuxghais.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/ggpirzxff.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gxmswdblu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/goiuexyeh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gtdsveqcz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgsxyjdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gvkvpenea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gqkpiiabj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtwkrnlhj.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/giufjmzkp.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gmpkecgsr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/grjtspbav.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gmcuxfcgo.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gmfjpzvug.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gjkpexhlw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gyqancvhh.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gydckfpfq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gtcvppkyc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gusmygmqh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gzyzqblkl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbksrhmhf.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gyyvgrmlx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkmufcvqg.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzjqteewm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpqnmfcmb.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gimnfwram.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gcmcjobaw.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gvcptoqmn.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gtskvhtwz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwrxsdalh.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcjhtdorc.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggpffhjcd.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmynkihuv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gpmzdehdl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gzlcvudml.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gdfuxspul.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gibahzqrn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gefifiyth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwhcpgkdh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grmalipmf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzeqckfer.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxitncmmu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ggrrgawhm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gqhtxvpnv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gummveavx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gsifksrmg.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gsibdehkk.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gprkfsyij.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gkdybozfm.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gtmstslxb.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/genoceioi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gnekxjksm.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gnxldumxu.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdotreqfw.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gotcxyqim.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gbmycqzbs.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gkbtdobxc.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gszmuvpzk.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gyztrrnjc.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gcpfwylus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gvpmobtcb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gfjqocabs.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gbptnxoqs.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gmbeuqrtp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gfchkksjm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ghmnmqjva.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gxlhsbggd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gujppukdl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/glfnuyvjf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gggrlylkv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/ggwdlnnrx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gefatgnvv.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gifcbfhab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gfvyloshw.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjlmlrgvs.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gsdtioeeb.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkaatgfou.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gjjcmhxjb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gggahszot.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gaundbooo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gqnvjeqqb.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnkovtzkz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/goecnztqv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gselvrfgv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhnlausm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbrtltcha.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghgynerxk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gcsawoeka.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/guzrjmkbb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gqkpzhxxs.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/giysewqhj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/getusbayo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gxdyokukr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gqyqnnwke.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gviscsssc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gpcjdsrtd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gtbxcnpdl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gpswuiamp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/glcrkbcak.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gtngthrps.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/ggphfaqur.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtwjpnoba.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtokvyuzf.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjguuohdj.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyusfbroj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gptfjjyqs.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gdqpheilx.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gnfbveqvy.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gjmqfjeas.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/goiffcafd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gzpctvnyx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gldjmitky.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gnrmfgdve.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/ggolhdipm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gcxmcbvkd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gqezozfgp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gyioeznhc.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gvelsfywg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gezvunveo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gogrwcqyx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gofzgkntb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gynnqnlrl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/grkypphog.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/glqmhfhei.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gictemcfc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwlerzxnf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gvjzptydy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gllffjwfp.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gfdqavuoy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gawpfalrw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpjilkptl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gkyoyuzrm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gzytufglh.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gjcacjdvo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gvfmakngh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grcficthk.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/giuiosgoj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbcndmvjq.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gvrlevcoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/ggbojjkht.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/giweorgui.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gzjvbkloz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gesqgjaij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gpcqejdif.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gfpjxoeqa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/geyglgqua.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gvfqogmjw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gjxrdwlij.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gcowfsoby.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvfezcllm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtkjpihiz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqqjmaltu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnuvdbnth.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gowgxhaue.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkmoymcka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gijjjhbrb.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/godncnztd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gnviwfyxm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghawdxoyd.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gfnvrcbuy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/glkmskpbb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfeajkzjj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gbcfbrpsb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gjoplckzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjpganuii.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gghhducbd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gibnsbfwq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gykgfmyqa.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gbdsfjufa.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gclvunmbf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/ggwvdaqkk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/guucjomxs.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gpxoyingj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gojolglup.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gwknlxklp.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gbzocywaz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gprndexlj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gqkthmmoy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/glmhyhxnk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gpzbxyzfb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gmnsecwsc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gpwvsodzo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gsybbkmcp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gqxlomddc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gxuvsejwj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gubirryhd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gsjjaqchb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gncrgcaxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gxvnksxkh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gfgwtakpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gcovwifox.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/ghmneyyte.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gjkyjcmod.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gfcglptyf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhuohayk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gajpnljjv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/giscpmnyo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gscaleetc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/glvpqhdih.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gsnlmrrvi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gcvtuetgk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/guszsodhb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gpaftjdln.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gdliacohv.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gnkjoxrut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gxzmppmjk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gbyvpguxw.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/glzvmxhvy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gnjfrvucf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gahjaluff.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gyajvifaw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gmhpwptox.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gpxljgykp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gdcszrcjw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/ggeqhhaby.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gqaphnmvo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gfpwbtnbv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gjagkidvc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gwbkeyzig.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gtejvbssm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/ggmbyucov.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gnypjbmdk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gslruqrjq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gmpzfgegs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gyhrkzbfq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gfokxpqfc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gqkbtvkgx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjgqbfqlf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsiyzmoeb.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gwfygzuem.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gajceyapq.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gscvxqxpf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gungvdfgz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gntzxwgat.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gyvkdqxau.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/grernuyuo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gobryumyi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gcnktpgyn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gzynarvql.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/glsyydeza.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gcmhhwfvz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gvcibltmj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/guhbmwaev.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/groaiaihm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gjwojoqgx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/growuluoz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gslpajmhw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gnyvizdvr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gsftvmcnw.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gfvqamzhv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/ghcxbitce.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gmqwlheks.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gkzndbjyv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gpnizmrfc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gzzdvujye.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/guqhzuxkt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gkpppnfmi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gypptujny.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gwymoqhkp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gukhycrce.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtjdqnoop.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gzuhrwgic.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gztnackdb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gbcpbgioz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gacgoknop.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gcrnkpxgm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/ggrqbfklv.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gdawsxqvl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gpptevcrk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/guhnsgrbz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ghwvdvbjl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gpvcfdaca.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/glreivlco.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gnzzzqvst.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gsgpgxadp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gjvptrjht.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gbjnvkpzq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gzkuzjijw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/goqmsskoi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gnlfystzh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gxfabjvjt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gmzaeabtn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/goarzjqsj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gqnpxjndl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/garaczjti.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/ggesxftlp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gifgcrslp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gotzshuhc.sHtML


<!-- 参考信息 -->