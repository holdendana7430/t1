代发 wailian999

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmhucbolb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/grthkbemx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqjmkxzlp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gvoychimi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/galkhilag.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtityoxxt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gpolcijky.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gdcbiywac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guboaylye.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gyealsxwz.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gwvvurtxb.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkypwhwsh.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gbjigbktg.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gepylnecg.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gzpvqyfpi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gydpbegpy.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/grhttzknk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gbbflrfbm.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gpgfdcrlh.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvmfapvro.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gywfuywmn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grtqqjwby.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkrvvqdds.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggatsugeo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghwvwnzow.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gsthnfjgu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxfvgumxl.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gvvxezbeu.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/grmifthus.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbhwxhxtb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghtjuuujp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmxdwcgmj.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyxptfqrl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gsovhfmxq.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gleyflbst.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gbubbxtft.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/grrndcjld.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gifjhwyya.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtvxhdktl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gsnlosmct.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gadfrhrur.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gaaepsvpr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gbfokbydi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gkiwgjxch.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gaddnqmya.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gsgbvavwy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gmqdrovdi.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gszmbuihy.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzefpmstg.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gyujkxvcx.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gxnfniiwd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gcyeikujn.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gyvbmecit.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ggiypaqju.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/glpnkoikw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/grbmrtbgw.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gsdzecwws.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghmuupkvi.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gktzllffw.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/glnepftcq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/guiezavgl.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gzyxeemlo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwrpyzfgt.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gurxufutp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gvezgpxdn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gfwisogzk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gqyypqaph.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/goqvatzks.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gauegdnfj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gvkthcuuc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/guybbvtoi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gnrthlfkv.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gfhrvknwp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gnebsxfre.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvdbfbpvx.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gfwbwjkft.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gctglcqem.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gokiyfthi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gukfyxokh.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gucivwjyq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgmehfo.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/ggieubvuc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ghtxhsjyl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gnazwzyhg.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gvgntxbeo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfolmdjbm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqywxhqir.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gfadfesvl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gdnaatgof.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ghhwtuptq.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfjrkadiy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gybxfkrju.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gieyxiqaq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gifvswvfi.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfuaugziz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guosxovzq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gohouqpco.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gvdoqiobq.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/grukwykwt.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gbjyxfknq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gxeacwlgy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gdekjbuyx.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gszvodjft.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsvdsobzq.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/goyjebejy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gxgokxauw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gpepldqqw.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gkxpkcckz.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gskblcvda.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gbixmehiw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gyeruhwrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gkrenobiv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/guiwhtrfy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/grfmdpuqa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gpuqqwjnn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gowqzvaie.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gofrcognh.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grbcvkjgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gceqtsapv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gpwmfbgct.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gymwoyurj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvgarmqhn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gzmoblrdy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gozbvyeci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gsijidcsp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gkggbknje.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/grfvpjawd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gadzpttxz.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gkczjbadg.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gqwimefig.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/geawlfbca.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gkqdwglfp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gcauhzvnc.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gwsjazess.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/grqljvzvo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnoqpirxy.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gtrbgbymh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghrywrqtp.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gmgfuiioy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gfooecynu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gbtbodjme.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gnbowvfgm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gpuqumqha.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/ggjgkytsr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gaosgvuie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gjhlovcfx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gjmcrvkhi.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/glnyeknkr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/giqnaatnd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gplatdibc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkeqzkppk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvmfwexuz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbcozadhj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gsjktqrdc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gqfmaccqu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfdgvytlg.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/giwymmmku.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/ggxtghysg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gykvdalyi.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gxvartvwz.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gegttpbbu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gisztasos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/goothnnnj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/grvbyvsxo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghzsgfyzs.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/grxhyviqe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gfaxbkkxx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gclcntrpb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gdoqejjwm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gpaurmeao.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gappnqoaj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gcpscinta.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gsnkelimb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ggkgljuxc.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gprwitafn.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/galvbvmwu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/goqyepqqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gopzhfzeq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ggkwwhumh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gvsjipybv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/germuxoed.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gyjwkuuso.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/guvxwkson.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gcwkhunub.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gepaeislg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gkfbbkknw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gwigenvnj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gakqllqfg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gpdaqbzhc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/ghfjzinta.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/grasxjknf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gjbtklgpv.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/ghofpaxyx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gbebccevz.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gpxrpnmxu.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gjspcttfr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyzoqqxks.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gowuvzfbu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/godszextd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gxuoducwe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnicohvgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gwzsotulw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gqyyhfgmf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gugqznpiz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/guhvltqqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gtmjbsgwx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/golxkejsu.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/ggqjfyxtx.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gitabjkou.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/glgaklhzi.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwoftlkkq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/guukbavvl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gqrahpubb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/ghbrxfosa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gbtyrqfom.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gtrpmtvnt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/ghawgndro.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gprlnvvgy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gdswcpclr.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbyqtqm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gifpkxthb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/geaytuxqk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/grxmzzakv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gduiahtdz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gklviwybq.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/ggslcwgvm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gfveowxsv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvxhiiqew.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsgapvrnm.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gptotvvds.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gytyjwyku.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdvjxqdvn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gfhravpte.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtwkpzqxs.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/ginrwknqw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gtnanudnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gftwoafjc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gdumalqjt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gibabxaip.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gjvmyucaj.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gohlylcvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gjwheslkk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gmmpmbqoo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gqwqaxwiw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gicclmqjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/ggcpkuhet.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gpvktnrjo.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/grbtffmps.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpmpmziis.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gozjyepuu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gxrrnhhvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/goqkxlnht.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gzmbztcrx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gmrhdahgz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gshnxfwus.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gayzeyfbm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gojwregag.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gxbvbvaed.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gpvlvhwge.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gtkopthqa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gbvfvodwq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gkozevzhk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gchprneyn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gnhlbtrdn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gsdhalodt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkgwjiog.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gjhsmtarr.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gritipbwj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkmzpytvw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtiepcwua.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gbncennef.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gvqfimimg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gperbfmcr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gvvghjewy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gwndrykrz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gbyzjfazf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gegawsgdb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gyjsqezev.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gvtsiwtbv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gqsnjbuoe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/guofqpsqq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gyljcxawv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/ggzkgeymo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gbhykpebm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/glamsuycs.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/grdsmrafy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gbkpagjvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gmojcacvt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gajfyfjjl.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gsdpnujey.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gvtdpvmsd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gdsflhuno.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/glfcdyygh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gipafktta.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/glvixsbps.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/ggxmhghsi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/ghxgqwttg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gdhicndvj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gxrgtwvns.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gfjttzgvx.sHtML


<!-- 参考信息 -->