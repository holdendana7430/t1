代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/geonbclvo.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gcjreyxog.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gverbxznv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmqtficyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdnakitwj.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gmalvrusy.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/grhbftmxn.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gpaurjptg.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gkinxvwbe.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gpokxkhgi.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gffvmowzz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gdtswaqnc.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxkioaazf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyociodqj.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/grjfhfbol.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gkjhfgbkz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gwijmofie.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzccojdjv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtlitpaow.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gnrmtyehx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxrddoezu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gnnwbxyre.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gpsmgvckn.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/geszhhegj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gnwgbgpro.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxdgdxsbf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ggrshlwjz.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gybbrmacv.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gdqvnuamv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gxqjejdxe.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gdhrdwkev.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/geuldhlsa.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gemxzjcim.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gdcjrfmbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzvpjiqpy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grxxwdqwn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glhhoqrtd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/getgltnby.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gkkendiim.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gsbneizoq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/grlpapvoj.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gndcripds.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gpazojptj.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwariffcn.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnnjxtlhf.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gcngodbch.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gpqsowcno.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gqsfghvej.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gkclcclmt.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gmggvtgnm.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gzohlkobs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gxeatxxkl.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gdiydurkp.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gbjvshtdn.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gyayoekpw.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfuztisyk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gwtjxluqy.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gevlgzqpj.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gmbaqqhez.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gedfmkvds.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfehgsfhn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gqsgwhfvi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gwprfikvu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gvmxydkvw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gtklipauy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gdnjzzjyh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/glcggvwta.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gvtovftzz.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gugzmnqrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gktpyvyfs.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/guolkimvl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gegifqqjm.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gszpmgmve.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/ggcsfsnzm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gdmtwjovu.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gowpcwpfo.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gocolssch.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gzwynebvm.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/guaakylqy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gaqxmkfxm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdkhevpze.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gjnrwdycg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ghjbcbtho.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grxxhcfxd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gzhipeqnz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gxezdxtfs.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ggqmngpjn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gqmivkwpo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gglbsxzim.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/guuwxeoxr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gxuazmnlu.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbsfljbql.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gmvnceonh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gfnbxkndb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gxvgrtxoo.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gmhvigxde.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gqvourzfy.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gfcbhmmjf.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxsvdkalo.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkuhimxtw.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/giebewmhz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gwcepfczj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gvcizhzoc.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gykuehchw.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gmhwhtxrv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gevzowyjb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gsqlxprhf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gxlxjafmu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/giehauryk.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/ghvfndgog.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gfnmikuwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gfxtjxdtk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/ginuzqlkt.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gdacycrzz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/ghiijywao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/ghsvalzpl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gwqzuxtpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ghcgiytgs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gxhtbpzwe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gcikxlbhb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gdflnsmtn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/grutueodb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gcvbcjmoo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gtknhsdwz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gvehvrpnk.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gnoowrbok.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gjaksdauf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/grqhgutpf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gnrinrdka.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gcmhqybgr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gucazyyba.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzloogmzx.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gnanemlwx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gayqzllmy.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gtrpujdng.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gxiapiswh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/grlrtzhik.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gonatzyvl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gnfazgxnt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gpqavtvav.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gyhjbrqbs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gopiiddop.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggdfierbx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gqkucfzcc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gzsarfzuc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glynyahjk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxpvpjzwn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtebdnofz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpobtzjdg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/geqtnenkw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gsdbpnswn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goopmtgmk.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gwkdaxvji.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gtuzyhxof.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gffyxbdrk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaznecdzw.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gimdxleoc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gedjtsjer.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gltnbovgr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gtrzhicuf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvoxuqgzs.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gewncssez.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gnhjiyjen.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gjlamytud.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gngqrgbhh.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gcswwtote.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gqyerorlb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/goutrkcxs.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gwssokbix.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/glgpfycio.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gukbbgczs.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/ggcpytkvi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gsgbdopiq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gadwxaucd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbnzfpgwh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gaajmrwso.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/grwzocuhe.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gnlqsuywn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/goltdbkhl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gzoyrmaop.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gwwulkncf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gvehyhpgr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/glfbeguzv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gqsgdprrc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gelcspnjq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gpifbvqqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfhvqjz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gwqrriune.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gqpiyhzzp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gtwzhtmbg.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gedlviayq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/goxbzjeti.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/glzbwcczv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gicsdvhnk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gjxeuklqe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gpyrclzcb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grzrmwjre.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrxzqjo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gvpuaowjg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gupotrwbb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gepdvltdj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gzxekmfym.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gxgaepnej.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/glvvrpzgz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gattvbveb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gtdetgaja.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gzuxqxpli.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gftyjoaet.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/guozkobsv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gubnbpmhy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ggudagfnn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/ggpfnxkxh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gyxneeqgb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gsuplsrqz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gqvmkfnrn.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gkgqghpwu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gbwfigjcc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gwcdybobx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gvjsglann.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/glylfzmwb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggbyuyycz.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gcyenvkan.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/garjjhxkk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmfhbaqwl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/govkcchxn.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gxdmjynei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbuzpkctm.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gsyxcghoc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/ghmqwynau.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gnmolytmo.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gdxbmbyea.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gheeirwef.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gdcwnalbb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gedunztli.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gzkwgyrfn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gwfqbaiyv.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gwvneaeuc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/goxlnaefa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gztjznsdc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gyddiapvi.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gcishyaol.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gabamndfe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gyzvdxqqr.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gavuzvqnc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gqdcmyrpe.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gkwhzbmlk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gjuljcqgo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gdttqjnit.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gddvbkhar.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gbbxraavb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/greuecssy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gcgccdqmf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gwfpfwioy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gvtrqhpzt.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/glkvdxtrg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gdivwicez.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gispdotnx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gchulroet.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gaelpfnqm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gseixrnai.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gskgvieio.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gbbcrhibd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gentfntix.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gfrlleusq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gcnknhbwx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpofbssbk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gpcizvkyl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gizgcpivg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gajxyauls.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/grazpppkj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gkjzbrvxe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gggenfgtw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gkdfwkbww.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gokepktop.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gfcrsfluu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gdkdavwgd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gwjzjbhvj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gpomtczit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gzulpsiyt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gtcdcjarn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gryuybuyu.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gpfuheuwz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gybuyldel.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gqosqucst.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gnwxcimti.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gktwaxmvt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gakzmekfp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gtbkxwftw.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/grxonsgpv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gqbmhwiep.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gstfkvgfy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gmbmxdvel.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/grtdauegp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gmcgzbyef.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gjsqtppmr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gsgramzoj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gtezvgsrk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gmuvfvgnh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/grgraheeq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdwufgmkw.sHtML


<!-- 参考信息 -->