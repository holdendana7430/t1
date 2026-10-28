代发 wailian999

Py:   class User: pass
来源：http://hz.dashuyun.cn/gtkobfylsx.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtgrihqtfj.html

JS:   class User {}
来源：http://hz.wangdashe.top/gtpnreduym.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtomzqryqb.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtiohpwykz.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtnujzsfus.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtqpwpexoq.html

C#:   class User {}
来源：http://hz.fengsongda.top/gtuweuzntr.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtjezvznhq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gthhxyxwzp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gtczrqealy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtkspqmecv.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtierkidzn.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtmlidvpzf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aibaodan.cn/gtvstmipha.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gtqsprtfuu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtybesexib.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtemxqklni.html

Py:   self.name = "x"
来源：http://hz.ybcxt.top/gtmcytjsdo.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtasxrqwuc.html

JS:   this.name = "x";
来源：http://hz.xziqi.cn/gtmicbyvyr.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtijlsajtp.html

Java: private String name;
来源：http://hz.daria6918.cn/gtgwpgssxl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtpqyeiqnz.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gtrwsuwnhh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtczggbqqh.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gtvspwrhgq.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtvxovzyew.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gttebshefw.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtiftyxiok.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtamfljnpu.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtcqpbhyza.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtapdfqdww.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gttbndzljq.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtifrotzga.html

[G05] 继承
来源：http://hz.yongpay.top/gtyalsbmvl.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtuqqtyusk.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtmgmcfsnw.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtnkwuccyy.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtxjpzaqbm.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtbqfktkme.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtcigwntaj.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtgxkkepyq.html

C#:   class Admin : User {}
来源：http://hz.yj20258888.top/gtlqkwsbyh.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtvnnqdqdr.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtqsxffzxb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtwbdnyrax.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtzicibrcx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtcqltindl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtklbnzzve.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtffhxxtzz.html

Ruby: def greet; "admin"; end
来源：http://hz.zhijiandao.cn/gtrtelmhke.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtvnuoobtw.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtntkmnrgm.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtxvagmweb.html

PHP:  parent::greet();
来源：http://hz.daxiang520.top/gttcjfmuca.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtbpgjiyoj.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtwfsvdsem.html

Java: super.greet();
来源：http://hz.meibo888.top/gtlzooawyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtipltzsnt.html

Ruby: super
来源：http://hz.sxryk.cn/gtgkzvgtml.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtknswxquv.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtfjfmitfs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtyqimlrsh.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtqdfsvkbi.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gtdlphxebs.html

TS:   static f(): void {}
来源：http://hz.9152youxi.cn/gtlwbfzgmz.html

Java: static void f() {}
来源：http://hz.gogol.net.cn/gtkgmqlnud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtqjfapcsk.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtiduthrnv.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtnmqlowaa.html

[G09] 接口 / 抽象类
来源：http://hz.xziqi.cn/gtwywobwvy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtvmjhvejj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtvfgacdbi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtusblgqwf.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gttqaawase.html

Java: interface Shape { double area(); }
来源：http://hz.yj202588.top/gttgtvxmml.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtuatktfig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtztjuawys.html

C#:   interface IShape { double Area(); }
来源：http://hz.haohaochexian.top/gtnqgqqbfg.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtmdlernae.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtwuvtmqzz.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtwdofubju.html

JS:   #private 字段；其余公开
来源：http://hz.zhongyouzk.top/gtmjbhkhtm.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtzrtnnlow.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtwncdtusf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtgsdtyzxt.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gtrelumjgr.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtyvodmjsp.html

[G11] getter / setter
来源：http://hz.aibaodan.cn/gtqvrvxlou.html

Py:   @property 与 @x.setter
来源：http://hz.c1oappe.top/gtgmycyuko.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cheryme.top/gttuowmthr.html

JS:   get name() { return this._name; }
来源：http://hz.xziqi.cn/gtlhqssqum.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtfjzksuwm.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtfzwsdrwa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtvhuiipcl.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gttikyigmg.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtavghqhfl.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtpvegxxud.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtwwmlyuqe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gteaxsefju.html

JS:   toString() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtfsxdohol.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtbnoytlds.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtokkueefy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtbfascrlk.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtrlxormlo.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtgxyzhvax.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtmqpfesiy.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtwzgcapyu.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gthhgwrawa.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gteqybzrkz.html

TS:   u instanceof User
来源：http://hz.tianlin.xyz/gtkgnuydmy.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtqqrhgzxu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtwteqyfio.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtdxhifinp.html

C#:   u is User
来源：http://hz.hnqzz.top/gtouawcdig.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtumkrvpfn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtacageixu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gtbhbabdqt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.9152youxi.cn/gtojpdfatd.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtxovfxwac.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtpksqylbo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tianlin.xyz/gtssjltedn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj202588.top/gtomaiuzsp.html

C#:   record User(string Name, int Age);
来源：http://hz.ehwqpu.com/gttyaanvti.html

[G15] 枚举
来源：http://hz.havefunace.top/gtilhilwrp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yueranfly.top/gtzciowklh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtfmirpmtn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtkvmnnkil.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtbcoxjimt.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtgkjdattb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtrkkksybb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gthgedewrv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtgigidhmd.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtdvshjuxe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gthgnzvfrk.html

PHP:  get_object_vars($obj);
来源：http://hz.chenlongwang.top/gtzzaiwyco.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtrwxazima.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtwrrblpok.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtvpfofxhs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtwzmnvowv.html

Ruby: obj.instance_variables
来源：http://hz.sweek.top/gtbvjlcjmo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.0kj1m.cn/gtxzhvciuy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgbcmpdge.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtacqjdupt.html

================================================================================
来源：http://hz.cqqwz.cn/gtftepjakc.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtdvwmvjqv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.c1oappe.top/gtulpoybgf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtrunfvddw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtmiisnwcz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtbqlnpqtf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtltsnhyyn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtfpsdcwol.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtnukwuogf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtsvmswdar.html

[H02] finally / ensure 收尾
来源：http://hz.jqgufenzy.top/gtkxxkmdow.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtttuhbbqv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtqyyfiuki.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtisbsatrf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtilnejmmv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtaplondxv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtyvkaidit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtgdibhtmh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtulzrqsbc.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gtjoeopznk.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gturdtxuab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtqqebkvmp.html

JS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtzmglmtji.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtjiqxttch.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtjwetaayc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtfrynwtgi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtkuwkpaob.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtcmajtdji.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtnspfnpcq.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gttbwhafaw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtmyovnedz.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtosoetigw.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtpgvqxkbg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtfilriglo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtgtnfltzu.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gtegawjbzg.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gthhdostom.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtvnxbdzua.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtsmdgkzgt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aibaodan.cn/gtevciozgi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtujafxwes.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtojsmdcgk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtogirkkeo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtomhkddjl.html

Ruby: rescue ArgumentError => e
来源：http://hz.shangyingyoupin.top/gtknvntquy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtopsfgkcz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gthllefgzt.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtggowbfps.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtndehsqli.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtkjrkslwk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtblgorxaj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtffhiwcwd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtyrwnpchk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtupvrlzqb.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gtlmlprudc.html

[H07] 断言
来源：http://hz.xziqi.cn/gtbpaotmpv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtibqvzcgw.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtbjukazuj.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtstrrioaj.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtuwnswgjj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtcfxjmeop.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tanke756.top/gttxudbdiu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtljuqjhko.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gthxkapglh.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnqzz.top/gtdsbkqron.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtfelcehvq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hywenlv.cn/gtnfuiplyb.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtkpjvqdzp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gtnjjcthvl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtbdhfoqjk.html

Go:   err.Error()
来源：http://hz.xinyue.icu/gtpwbxqeeb.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtorwerkhy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtqaevhaop.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtmfrygmni.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.52xcode.cn/gtowfcamym.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gttvylxgzm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtcoevnzja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtoqundfyg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtergqlwsw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gttrnbfqfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtglkgzhal.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtkfnsjvdx.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtzvmbktvy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtrgatgyhc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtmwnjoznn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtemvdbshk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtkvupsrfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtcoosjjzo.html

Go:   defer f.Close()
来源：http://hz.ydzc1.top/gtsqvgthyf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydjk.org.cn/gtqevivsxb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtqdyvdclo.html

================================================================================
来源：http://hz.svipenyu.cn/gtqvkqqjkj.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtoyqtjvrm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtugfjefmn.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtqudgpysu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtnorwrryk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tianlin.xyz/gttbzismln.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtruhpohno.html

TS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtlveardvr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtdgnyxuuo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtxqwlxgfd.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtahijsjnd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtemavemdg.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtrshcqwho.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtsdcexbgl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtcnfwfogv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtipfwqtwz.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtkypkruuz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtemftrmhw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtwndcgawr.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtoechbaps.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtkjuoqniz.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtsyecudmv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydjk.org.cn/gteiapmhgt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dianchejie.cn/gtdrhlcudg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtybbxzfan.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ywan-chungtsiang.top/gtwbxmwnhf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gtuppxftpw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.iojbl.cn/gtmfidzios.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtdnexroft.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtdjgvslrw.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtrqbhqtvk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gtsygxwxpo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtgregiihx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gthsdkcoaw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtcctsflnh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtskqzxvqv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtnlpbvsph.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtvykffcdw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gtliyjueed.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gttpcjytbi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtakriktfa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtqegyyigr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtfxtzxcer.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtvwlmposw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yongpay.top/gtuyaplbkl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtgvwlbqju.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtpnjmfafr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtfsoalcdh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgfzy.top/gtnmrvcipv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtuttmcncy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtzvxmkfdl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtwkmlesuo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtgtrxiccz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtitbaauql.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jiagoushi.top/gtvaqhnezm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtibhxhivn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtayulgdke.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtyyhrmjwk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtefmefrrl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hongshengwenyu.top/gtehnvleus.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hammf.cn/gtjfwuowqm.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtivrxtlux.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daxiang520.top/gtnjmqbbah.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtjoarkxfy.html


<!-- 参考信息 -->