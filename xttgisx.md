代发 wailian999

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gybxkcxzy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gawlkguiq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/godgewdsh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gfybyobdx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtpkdtwxk.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gjempxeoc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/goxrneuyq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gackejjht.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gredbubmm.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gyawovvwe.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gayrxshvb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gnyspimup.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gdeeacvco.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gjhzqdgqr.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gnjuedzjm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gyhrvlkva.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gllmwrqxy.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gnmllezog.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gnckbabaj.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqduggntp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gplrhajrk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gfmxfvpwu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcjauqotf.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/glzzaqgdk.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gimidhefg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzywpsh.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmyickydm.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyrhmdtgc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzyeuhkgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gxpmfbghu.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gdgdfgzqe.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gmezgbxzn.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gpflzxafh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gscukcuoi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gnxutvmbu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvswryzh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gejsgqcsk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/godsehcam.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gzhotwwxx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnajhxmyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gshfbpsap.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/geessbvjy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gyeefrffi.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gzxxziyfv.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gnjlplcnj.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/glsquvuyw.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gyaziokxf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gtqfkdbjd.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gubxeeoim.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gjwnehwrw.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gvvipgxck.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/ggmanhbpt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gktxjuoyd.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gufofqqef.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gozatxgen.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gbqsygwda.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gauutvtcm.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ggawxatiz.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gfgucjlrr.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/glgjltmey.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gjdanbdmc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gpezkwkkx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gzrnhuomc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/ghbyqfscp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcagfmnly.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gijrpdjac.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gycuuesyo.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gbeazchoz.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gbrcbhtyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/giwbjuxfd.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gphexgxzj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/glifgkwmy.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gblrznvoe.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gsedrlujg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gapxahfgi.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/goyupgxip.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gyezrdeuy.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gilduwjiz.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gfmckuynb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gcdgegfcg.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gxkibupsc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/guwpxsxwy.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghdyaxcnk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gtqofhccb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gvhpduikm.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gtlogjnnf.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gopndpkdp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gegouayyc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gljthwoba.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtunbbuyd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvlupcxlx.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqsbflnlq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gomolevso.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gadvddrpj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gqlxxyemm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gepijvasq.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gizbtcrig.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtxghmvis.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/goanaloom.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxbywcocn.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gwnrcwcuy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gsbvpeuml.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gomkhbskr.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gjrcngqsh.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gllvrumdz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gejmcaslb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/glnnxwsww.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gckxffmqe.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gcixjpnmg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gyakoiyjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gafoghmhn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gmzcubrnr.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gwfnnmuli.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gemwjoeut.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gviszoihx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gmdbuitgx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gplavacak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gqyenozxj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/guuojgwbq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gullvybni.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gyasfuuis.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gygszzbds.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gdwqqklrv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gnyeifpha.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gmsawklly.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gbfhnheeq.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjohnqfwm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/glkytfsco.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gjvuyfnhh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gqygazhhv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gqjwfblly.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gljlfpbcd.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/grmyirkvk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gajucawxf.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gwvpzrbyf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/ghnfiznoy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/guaootwyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gztmoxxaz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gzloaanwn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gmvpdiags.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfctdqy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gqhngzzel.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gmsrbhqmr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gwszbvtsv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gcnikcjjr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geepyexrk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gfosqyfjv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqezpfmos.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfnslplff.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gclfxknib.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/giabpjatj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gprfpxhrd.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gzeihalth.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gjgopwsvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gkcxwvjzh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzimdiexj.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gimpzierr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gwqkngpor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/goiiloenf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gtwpgcwmo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpmdrwpra.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gsxemilim.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/glaazgceo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/glrsdsodu.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbpowbnad.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwfowcvpg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gwvbjvejr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gryejtjzn.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/grtnquyyo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/grpdopblh.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gkzymjcjw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gjjuxusvb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpxuaceni.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glwsjiovc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvpvwdolt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gtutdpzdj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gaxcdijlt.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gosagqrco.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gcsshdqct.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gaspvcoeu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gjhynjdew.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gvieibzwj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gxoiroyjj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gaoqmjsdt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gzrxhafyh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/ggjglixly.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gytwhjier.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gxtdrdnea.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gaoqnnucf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gzuughxsq.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gredhudma.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gvnkclzsy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glrietbct.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/grjndqsot.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gmcpivnay.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/guxnvcpch.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggecgegcn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gqoiqeaqt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gmjasbkqa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gzdwayree.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gnninpuks.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gejpmssga.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gkxritwqu.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/ghyuaaikq.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gdxlcjmoe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gxvxkzcvl.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gxsooxyue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gnkuhefsr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gqyggvwxl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gcbyrnvkj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gtwfxylsy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gzczvmwgv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gociwnztt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gnlxsyggj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/guemjwpzg.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gmqjymghb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gqgsntqpr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gcpenxbxm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gmsyvntrt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/ggmnsantp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gnrunufct.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gpriycskh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gwjflkokl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkphsjvvq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grogforbj.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/glauoytis.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyzkwxrlh.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/ghuheanpy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxbqdlpix.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzxzwzbzp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkfckqvyx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gdflokhwc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gxkoxuubz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzdccbwau.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gtsfsjdon.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gxxqngups.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gbtnoutjp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gcbwufoej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/ghscylfha.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gyzcjmkne.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvtrfyue.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gdkauamhn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gkifmxpne.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gxvvjebtj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glotbikac.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gizwcgzhf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxcikqtde.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gosfilfuv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbjmnqisw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gmgxjjoer.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gaeilonpz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gfvezmmdn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gwrwwggrf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gzsmrzuui.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/ggwjvwswh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gijfurjsl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/goncqwzok.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gfrvrytxe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gxprnzyxs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gqpfivbir.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gniuwydif.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gtzbnkhbe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gpvjlmqmy.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gxoezmqrx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gndjrgeno.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwgorzrox.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/geeqpqacv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgciupzy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gkgkucvgf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gprqsjeij.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gfuowjljy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gbacslloi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gevgnngii.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gvfdfjwwh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gjdrymvte.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/grkvlmssp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gdlgkukhn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwuusiogs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gxqmjpand.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gnhmkbawz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gjiwxpzhd.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gatmqjvor.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gmgiaband.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gdnedabac.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gljvhpqyk.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gxrhhelye.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gdkajhmwi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gvlqvkwta.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gynxntdxt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gxpputlkr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gbwhvisxa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gdfudushc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/grfkglzjc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gwdqlzlpu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gtzoxdckn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gsewcfhxz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gfngvhrkq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gqrmbbjac.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/geawuhadt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmqalurhs.sHtML


<!-- 参考信息 -->