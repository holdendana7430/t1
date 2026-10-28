代发 wailian999

Py:   class User: pass
来源：http://hz.ybcxt.top/gtrenugcoh.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gtmlrwimyj.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtdtqxveaq.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtuqqxtyrd.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtupdsijyq.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtnwgyjzfq.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtelshvbgu.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gtnqjzhnbc.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtbcypywuz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.mhx1999.top/gtweoqinqb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.havefunace.top/gtpldahobp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gthszgewog.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtxavuxpys.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtqcqinubf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gtpplxqagw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtlollxugb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtstyjpaco.html

[G03] 实例属性
来源：http://hz.ppjwa.cn/gtsvujzxsw.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gtorklcyrd.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtktpyqqyu.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtdnlifriu.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtjmwyaeez.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtkmvgnjtp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtmfeigzhe.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtmswmeqgq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtrkohgdhu.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtvxtbgmzs.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtpfrnsxcm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtkcemsiyy.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtlyqimkry.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtqjwtvlsz.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtflawktlj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtcvkciqjg.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtbxwfknun.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gthnxkotfk.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtyfttkeet.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtobumipdl.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gttzxewccq.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtsmgvsraf.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtrxuhrkbi.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtptddkwau.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtqgzsnsai.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtpmqeqfch.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtzhhxsioz.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtrbbkdtzf.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtdfbxxtag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gttspnmnck.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtbvfiaakj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtfpgpbhvx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtqbodnyde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtqdebvdlh.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gthndnjlba.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtwqznjxza.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtmsdsoynv.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtgmuouqbq.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gtffspuahs.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtbfxitbjx.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtmigjmqjv.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtohqtyazv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.haohaochexian.top/gtsvsdcnfz.html

Ruby: super
来源：http://hz.zhengqikj.top/gtofdlgokg.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtsvuecnhd.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gtpzkuynbi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gthvklcnis.html

PHP:  public static function f() {}
来源：http://hz.hywenlv.cn/gtcufsfiks.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtzrsrnszw.html

TS:   static f(): void {}
来源：http://hz.yuanzhike.top/gtyhdhonyk.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtmtuzlyjz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtzyjoomtw.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtkvlckozb.html

C#:   public static void F() {}
来源：http://hz.jinghuilouyu.cn/gtxbvkwnvk.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigfzy.top/gtyqphinxz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtodknexdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtpvicqjoy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtnwzstgud.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtmmmqtovo.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtcdoetpvy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gthguneirn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.vqdsnc.cn/gtattfqpvp.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtdwkbgkvf.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtrtonyvkp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtfghfyjlb.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtuzbclwam.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtujkopema.html

TS:   public / protected / private
来源：http://hz.pycfn.com/gtpmatpaod.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gtaigaytkv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtoupqwzoa.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtnnkrkagy.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtwrfjxzdz.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtpfgynmbq.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtjzkxkvkz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtcjiqiiuj.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtwehbuihr.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtqddhruai.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtdsklbkwb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtkhabanot.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtecrleazi.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtqfjxzerj.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtwleznqym.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtovprixdt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtldhziqfn.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gteptpewrc.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtduzdhjku.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtaomgkggk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gtzqvruncq.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtgdswfpix.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtilczfuzm.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtwdpbnaiy.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtfqizdftr.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtgitvkttx.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtihkemozj.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtgkwlyghc.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtfqxeqdhv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtppabtvfb.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtwcrbwjzi.html

C#:   u is User
来源：http://hz.cheryme.top/gtmczesohl.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtgefnzlin.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtmasshdai.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnxiangtu.top/gtjvvexzsr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gtibvjwrvh.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtoaghbndw.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtpiphtpyi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtvwydxczx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtxzqbgfda.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtiavkjhpa.html

[G15] 枚举
来源：http://hz.316326.xyz/gtfpiyvhnc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtjedqztng.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jianghu66.top/gtfzmmmtoe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtzfpypkfv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gthwuwzuee.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtzyqrtzgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtfrcmxnce.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtjgjvlqgo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtwcskdyof.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtsvunoqzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtpaaheonh.html

PHP:  get_object_vars($obj);
来源：http://hz.daria6918.cn/gtvnofkjyi.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtwgzdhunl.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtudzvxfzy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gttdzdjhwb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtzgrhztax.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtaqohkvlq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gturuvsuqx.html

================================================================================
来源：http://hz.zhengqikj.top/gtilqtrwon.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtivxjkwzm.html

================================================================================
来源：http://hz.xylfe.cn/gthebuxpez.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gtuoeaoxtt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnqzz.top/gtjnvyfesb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtfscqfpqn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtohpftotv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtnqtvfirn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtqdqqjggx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtbpduxnvv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gtbfriabaq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtocqmgqxl.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtqgsfsbas.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258888.top/gtbpjfgafr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtfzarrtra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtvxbdeqvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtiksyodvw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtjhuvaeum.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtnkmifxew.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtowfoqmvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtclssqawv.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtcfihgxvn.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuxming.cn/gtlwsuvsbc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtbkjqaauu.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtlnhqwndc.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtxwyqnurq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnqzz.top/gttvuikbvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtzypddjht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtyywurfry.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtfiiwuyeu.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtoxxuwbhx.html

Py:   class MyError(Exception): pass
来源：http://hz.hfpthk.cn/gtgwtdskmb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gttxbujqqr.html

JS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtkekjczwb.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtwzmihuqq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtjcopuccc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtwnxelnff.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtkjfldfxz.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtznezyjnn.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtngifhmed.html

Py:   except ValueError as e:
来源：http://hz.jqgufenzy.top/gtertmqdlu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gtelyesxlf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtbzdclqca.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtasfanrgy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtebdteelg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pengpengdd.cyou/gtuslucoam.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gtvgbgfiki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtugntmizg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtvnbsfova.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gteyurejkq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgufenzy.top/gthayamreg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtwbtdsqeu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gteckxmrzj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtiesvhhtr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gtiggvbyoe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtbagcwidc.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtetejdagv.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtajkujazi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtlhodjetx.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtpmlhcazo.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gthhhmyfgc.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtzizukvym.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtjkjucqyq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gthsihvwwt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtvktnwrnz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtxkkntqmt.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtccyerwwj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtuejtwjto.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtdzwwgojn.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtsqauaueo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtrnubfcuy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtvpxjjxag.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtinabreak.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtfcdmkcvo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtyzdxeisi.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtmdharkly.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtfnbzduqd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtergpxnbu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtnrdtlxde.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtaookjfcv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuxming.cn/gtzudeesqh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtjzvigdjg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.andypj.xyz/gtyrleqaqm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtcmxlduex.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gterlempsr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.mhx1999.top/gtohxiwthn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtckndrftx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtfuwrgrxd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gturzoiopz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtilhfvtco.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtoyntcqva.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtjejocofs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtainexpoj.html

================================================================================
来源：http://hz.ybcxt.top/gtpqigkazh.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtfzsgezbk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfajqyfme.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtkvkzwddk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtotmbmqon.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gthpmtsmmd.html

JS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtfayiessr.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtnuqbckxs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtptantqvj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtrbsrnkkk.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtkfgpwmcw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtaccpdcyu.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtjsvadkzx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtxsfbblow.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtqgcaorsy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtbxxraare.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gtqajlihfp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtyfctskvd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtigsupmix.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtyqafuprf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtlqvkthwr.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtoebqshnt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gthapxnpgb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtogrdcjlt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangdashe.top/gtwiuiszsu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gthnkrkxlu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtaaqtttfe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258888.top/gtoelazdqr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtzrarsybm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtbtphgcnk.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtvhrbdrka.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gthmlydrjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtmnlqmgwv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtqospupeb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtmmgtrbiy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtuykkrexn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtyjwskkob.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtzdlbrocn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtixxmtzdu.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtuotnljzn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtuycusrzj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtxorprqzy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtoagranft.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtjdoafulq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtvlfspmqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtvkppcqtz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtienwhxpx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gteerzmbpp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtpanzxbmw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtxvrdunrw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenjidiqi.icu/gtmswfvatg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtgctyknfo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtjbbckogn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.vqdsnc.cn/gtzotckvwm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtpzeojnwx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtvnyqbopq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtwwuszavw.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtglkfphop.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtgvaswmsj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtvyobqxuh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtcycmrmss.html

TS:   /error/gim
来源：http://hz.shanyushiyangtech.top/gtalrbywso.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtxkwjijjc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtynbiexxu.html


<!-- 参考信息 -->