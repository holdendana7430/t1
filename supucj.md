代发 wailian999

================================================================================
来源：http://hz.yuanzhike.top/gtpkpunwsr.html

G. 面向对象
来源：http://hz.316326.xyz/gtbofgljpa.html

================================================================================
来源：http://hz.haohaochexian.top/gtzhwqshji.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtndxclihv.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtbaobjrfz.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtqybiycte.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtuemuriyq.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtcamydpit.html

Java: class User {}
来源：http://hz.yongpay.top/gtdhggaweq.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtrrcgnlth.html

Ruby: class User; end
来源：http://hz.zhengqikj.top/gtybiykqjr.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtsyekruyi.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtjjrrptwn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtgudaifos.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gtsgxmmrrn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cheryme.top/gtsuvbaalr.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtplxubyid.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtydlvbzuh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtazjhlsth.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtqqoqovnp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gttyvuipjt.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtvnczenux.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtxaufktfb.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtmsabopyb.html

JS:   this.name = "x";
来源：http://hz.jinqigfzy.top/gtxtzgyoco.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtwffthjcd.html

Java: private String name;
来源：http://hz.zycfv.cn/gtoxcvkwbx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtxmcpfgfs.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtlftbtgkj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gtxeakpmun.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtgttyxync.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtrwhrxqcx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtgpbwecny.html

JS:   greet() { return this.name; }
来源：http://hz.cdnleiting.top/gtbmzdrpyl.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gteawrltgp.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gthgtrxhro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtcbvlyzlk.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtbtuxvbxm.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtptlushmh.html

[G05] 继承
来源：http://hz.sxryk.cn/gtywvkukpj.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtwukzhcmu.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gtoowylzki.html

JS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtxkbnfwjr.html

TS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtzcysfgrq.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtywbtkcxh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtneracazf.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtozyhgvul.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtbwglqsxq.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtvxaknbwt.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtflbgvsto.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gtzzllnjob.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtuoybmjle.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtztkoqmyz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtknnhkyqd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guowangkeji.top/gtqhbvkqhx.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtxxddntxv.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtynlikvxy.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtxybwnnpf.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gthtgpoabr.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtqvsdtimg.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtdxihiogk.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtawmenqvc.html

Java: super.greet();
来源：http://hz.shzxlz.cn/gtxodetpku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtiqexrfqh.html

Ruby: super
来源：http://hz.tian-w.cn/gtywqlitbn.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtqtiytvbr.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtehxqpoej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtyikdjjmu.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtzkusntln.html

JS:   static f() {}
来源：http://hz.cdnleiting.top/gtxwqltrom.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtfnhuellq.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtvesxzltn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtppkzxnic.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtslcjsyxh.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtmpmydehe.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtvjxvocmb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gttzailwqj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dashuyun.cn/gtsriixhkv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtrpznveew.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtcpoyvuwb.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtshtlsoeh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxuanxn.top/gtwecyxspm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtcqkpanpf.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtxsxcgmkt.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtnrpvxguy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtleoeibtg.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gttwgclgon.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtrqtvhqbw.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtrgpfauom.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gteqasutaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtijwpopsa.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtsjmyakfa.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtlstumkmt.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtibinagan.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gtntuxzwei.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hammf.cn/gtfghbmqoj.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtjaaxcrys.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtfxfcrwii.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtpzkwcilk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtbdkhpqka.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gttlqvobjf.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtaidxfzpb.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtfkuipwia.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtmyvczjnl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtlriqqiiq.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtluixegfh.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtjglioqbt.html

Java: @Override public String toString() { return name; }
来源：http://hz.havefunace.top/gtcvxhhprl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtizszbjcg.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtiadnrxof.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtooupefzy.html

[G13] 判断对象类型
来源：http://hz.ppjwa.cn/gthmpxoryd.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtgrqscsar.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtqywkjzxs.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtxzdmfavy.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtqvivemvn.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gtzmzrmblf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gzhubu.top/gttzjyxbzm.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtuwdsghhj.html

C#:   u is User
来源：http://hz.ivvv.top/gtnyzdudhg.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtoohzhwiy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtkrdblhcd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gtbjuuikpe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gttlblyhyb.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gtlzuxtxgc.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtyhhjybft.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yonumen.top/gtragexorm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtezwahvyv.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtjvgcpeac.html

[G15] 枚举
来源：http://hz.pycfn.com/gtdzakfwmy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtgcyvittc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtikgdvjdi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtwjtundnr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtzxdxqrbk.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gteatcwejb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtqhkrsjuz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtdyjokneo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtzpvzykpr.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtixunjhxp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtrqwlwcrt.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtktvzmndl.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtcapsevun.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtghplpvxk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtvwilqvop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtprfbjwaf.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtmainqxwm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gthautniue.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdbnbevpb.html

H. 异常与错误处理
来源：http://hz.cdnleiting.top/gtvqoahlsw.html

================================================================================
来源：http://hz.tianlin.xyz/gtmwcckqlg.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtztdmvzxh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtkesqcgqu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sweek.top/gtvzkgcljs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gthjtceqpw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtvgxgsljg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtdkfepvys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtfkfjumur.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hammf.cn/gtjyxouewl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtoqovzpbf.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtzjpqnfyw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tianlin.xyz/gtoqaynyna.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtmnehhmjq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtnnbmvsqh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gteyewetgi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtoukorxdm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtkfvrexct.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gthcpmrobw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cashguo.top/gtqthxnaoe.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gteltciodx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtqxxmntbz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258.top/gtrokfigvv.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtszjbivrt.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtebaqjsam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gttcqtugxr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtltczvdiy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtamyzzbre.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gttnduphvc.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtnxuvvdfv.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtjxikxlpv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtrqihxhcq.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtplphpsmw.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtcgflznua.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtmyygixnp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtdelyeypm.html

Ruby: class MyError < StandardError; end
来源：http://hz.gotoacloud.top/gtcgbjjksf.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtbbineisz.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gtwprrvvbt.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtyknmjcdd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtwmhcqysf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtmufvybxn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtfmjjocqu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtjnlljfju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtckzpybur.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gtyqpgwezx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtbysxnnzu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ehwqpu.com/gtmcxxnvlv.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gtswdlhmqj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtnnpagxmn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtkxczzoje.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtnhvltgrl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtioqfdeze.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtyrgdcavk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gtjmjbijma.html

C#:   obj?.A?.B ?? default
来源：http://hz.yonumen.top/gtfadludiw.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtpchkkmwi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtqmjgrhep.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gtjybzlzuo.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtlimimcru.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtogfmdibp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtdiryzbge.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gtsmacxkcn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtgkxxehig.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ivvv.top/gtpktufkqm.html

[H08] 获取错误信息与堆栈
来源：http://hz.aibaodan.cn/gtdjbxjxlr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtnzawjpwh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtyavinyzj.html

JS:   e.message;  e.stack
来源：http://hz.ivvv.top/gticbenmfw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtjvqleazb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtpbvzloyc.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gtsliddjys.html

Ruby: e.message;  e.backtrace
来源：http://hz.meibo888.top/gtphyehqdl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtsfvonofz.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gtggzdatan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtfudgfoya.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtmpxyvgsn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinghuilouyu.cn/gtzmbqcurc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtqeockdqy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtftctxsvi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aizwys.cn/gtmjbfjpdd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtyrpzrrvs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtkpcjkffq.html

[H10] 资源自动释放
来源：http://hz.zhijiandao.cn/gtvggzoelh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtxtjwalrt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtzixbdjxa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtriihlxye.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtamkrtitr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtaavuhebl.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtupewzjgs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.havefunace.top/gthgkwahvi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtwwbcfrzo.html

================================================================================
来源：http://hz.andypj.xyz/gtjuizdopl.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtucwsnrli.html

================================================================================
来源：http://hz.xziqi.cn/gtmwnwbpbr.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtswnbfqcw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtqvzooarn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtleaxpntl.html

JS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gttbwpadwb.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtlepuyuhw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtkndvpyhe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tian-w.cn/gtxmtwfhum.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258888.top/gtrqzwvptk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jlsjyb.cn/gtppkznkao.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gteewlxyaa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtalrxmrpn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtauwpyyjf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtbswjqjcu.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtakmqrqya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtjltmhfnm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gtshpykbcs.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gthgcvobdt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtopuejfuw.html

[I03] 提取捕获分组
来源：http://hz.ywan-chungtsiang.top/gtcaptpwfg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtmuiwvuus.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtmuzozwkb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtfwciavxa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtmovejzvr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtbnghgpjl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aizwys.cn/gttdgwxgns.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtbqdrxeqw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtocpggyrg.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtvxizdpdo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtdfhwxagg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtcwudmlml.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtjtfthjql.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtoznzixeg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtrqjuxrky.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtepucxymf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtfwkmfcit.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gtjmiffvnl.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtyntgzjei.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtvqqwsymr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gteubawnrj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtkduadqhg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtcupfcgfs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtakxsdlls.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gthjwzbxpg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtfvsecgct.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtszhpojni.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gtrvackadx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtopjpxyxi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtomspeuok.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtvssimfuw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gthechmgzg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtkpvbtxlh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cdnleiting.top/gtlgfcwjwc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtzfjqzofl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtkpbtmukx.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtqaxpqizm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtlpdtgfhn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtmkgrkwzs.html


<!-- 参考信息 -->