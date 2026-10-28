代发 wailian999

================================================================================
来源：http://hz.xuetiantiany.cn/gtluzrhvxi.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtrrtlzylm.html

================================================================================
来源：http://hz.pycfn.com/gtslvmapcu.html

[G01] 定义类
来源：http://hz.meibo888.top/gtwrkwpjen.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtomhvsabk.html

PHP:  class User {}
来源：http://hz.yonumen.top/gtbootzgey.html

JS:   class User {}
来源：http://hz.pycfn.com/gtyofuyrfd.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtdzmcgvqv.html

Java: class User {}
来源：http://hz.svipenyu.cn/gthblnkivl.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtwgwlvnyo.html

Ruby: class User; end
来源：http://hz.wangdashe.top/gtnyqfwsqv.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gthkyhqyxr.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gteuoksmma.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtizbhsmrx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtsuffyrfe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtbenakxnu.html

TS:   constructor(public name: string) {}
来源：http://hz.shangyingyoupin.top/gtbzhxqfyk.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtmkiwxpmv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydjk.org.cn/gtoigjsymo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtxzosxdzc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtzgytzimr.html

[G03] 实例属性
来源：http://hz.zhoulong.xyz/gtxnoffhmt.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtqwyxente.html

PHP:  public string $name = "x";
来源：http://hz.jyoumei.cn/gtgagwnklz.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtppaupwzu.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtegodvmzx.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtswovkmxg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sweek.top/gtermijvwp.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtdsrokfch.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtpdbynqew.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtnnawxqnt.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtnvuvwtic.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.meibo888.top/gtsxgpsudu.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtrkczhwxk.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtoipqyjqa.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtlmxnbczj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtexrgoluv.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtshlyrrom.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtxwmfglux.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtdzwwkvbt.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtvafylnvc.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtplnpirdk.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtowywcjgm.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtclwtgjzb.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gteppgorvt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtfpiqubhr.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtfvvwdkin.html

C#:   class Admin : User {}
来源：http://hz.pengpengdd.cyou/gtnckdbelw.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtzeeozwxl.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtzvnppzqs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtlqhqxrkz.html

JS:   greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gthdefejfs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtbvdgtmrz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtqsstslci.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtgvcfnpgc.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtdxdgqqgh.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtvxwaxsqy.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gthujjddhj.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtghzffeuc.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtxyubyfwa.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtwuuzgwqp.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtmuuvvmuy.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gtbmttxolt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gtnjhkdpxk.html

Ruby: super
来源：http://hz.jqgfzy.top/gtgtwhkhso.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtqwvguqxy.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtuvmlbcfb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtsbcasprx.html

PHP:  public static function f() {}
来源：http://hz.birdmap.top/gtehqshurl.html

JS:   static f() {}
来源：http://hz.wangshuangyany.cn/gtiuoynbpn.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtmcbqsfji.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtdodskczq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtwjlqwzkk.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gttxirqfxa.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gttkyiprrt.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtsrdlgpsf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sufxvd.cn/gtqwdbwfyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtjlsgamif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtkganmqkp.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtljqhoykn.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtewdejaoa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtlyssyvmu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gthapqxmrp.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtyptkcxhx.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtrinvfrgu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gthqhsaute.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtittihvdb.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtagmujbfk.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtzrihjqhc.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtfliellbr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.snrcjt.cn/gtftamzvjs.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtvwojqyqu.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtrctxtfci.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtyxrbrsua.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtchspwsor.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtnptaqoiq.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtrysradjo.html

TS:   get name(): string { return this._name; }
来源：http://hz.cashguo.top/gtmlpmqvfu.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtwfoibizn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtvelfnbmq.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtpoowvnrk.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtniyldbwc.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtcpqjltzh.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtytmtyopw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtxnbabyiu.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtyweykpcr.html

TS:   toString(): string { return this.name; }
来源：http://hz.nwbrower.top/gtvzywvgsp.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtyzbzpbpp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtocuwgcrz.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtfvfsnggk.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtmbrhaakl.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtthoqdipb.html

Py:   isinstance(u, User)
来源：http://hz.pycfn.com/gtlqeyjsic.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtqdpeixrn.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtwybimypv.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtuldfptbx.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtidttaggp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gtjrtrwjwl.html

Ruby: u.is_a?(User)
来源：http://hz.fzhhl.top/gttbjaamcn.html

C#:   u is User
来源：http://hz.yongpay.top/gtihzekwmj.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtveqeaqef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gttyknqwkc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtpppoxvsw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ppjwa.cn/gtckgdtotz.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtskszxico.html

Java: record User(String name, int age) {}
来源：http://hz.birdmap.top/gtekpeabfm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtdbruzuug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtmhoedcnl.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtrfcjlrjy.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtcwninkya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtoraeojbz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtggbrsysh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gttvhygoyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtctmbxgvx.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtuyavkfft.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shzxlz.cn/gtqqzpiuwt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtkrfbnvzc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtzagpfwmm.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtkivlvvir.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtldclldqn.html

PHP:  get_object_vars($obj);
来源：http://hz.xziqi.cn/gtecwypysl.html

JS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtqeblxcov.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtuovuozxu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtoejccdtd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtiqsziyoc.html

Ruby: obj.instance_variables
来源：http://hz.ydzc1.top/gtlzygucxs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtkqazeugd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuvfxbqnn.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtqitociuz.html

================================================================================
来源：http://hz.ppjwa.cn/gtwhfpeggd.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtepnrmvvu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtsjvphjam.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtqqryfwep.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cheryme.top/gtoltkshpd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtebjxgayk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gogol.net.cn/gtivxautmy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gtvoxexfjt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtvqhohhag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtziycxdvk.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtryyomfrf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtorbolfni.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtqunjhnnt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtqjskqzhb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtasuemovz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtibenpbdh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jianghu66.top/gtvtkneyya.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtgslebfem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ppjwa.cn/gtzdydtgws.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtghtwgulq.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtxyrsifoh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtogofowts.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtyewvxfzg.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtdawfjjni.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtpxahdfoz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtrmbugcql.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gthkudydpm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtlandohtu.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtlutdlevq.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtcawavwei.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gthoklwaxf.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtcafkhofa.html

TS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtcxnzodgw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtqwbhnavs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtzrwpljep.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gthbhvyekj.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtbfxwxbdn.html

[H05] 捕获特定类型
来源：http://hz.nanxinkj.top/gtmqbsihra.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtqpsxnnzq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtnztixgdu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtqojpzyhr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtnbydfsvi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtoeteitlu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gtsofcwswr.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtizwwbpdq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtobyaqaft.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtnsngrbud.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtnyigxjmy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtlvkjvfas.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtphfmqvyw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtsxewyoxp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtcuzoyfkk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtdytdxqha.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtnixrzctp.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtiqiniteu.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtjbvufcfe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtcwykvrqd.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtmufnkivr.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtdyjihors.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtbbgwryhq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtpezfopxi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtryfjabow.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtsalkensc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtodcbewax.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtksdvdxwt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtaqvsgcum.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtigsdcinl.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtxowwmfgw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtfznbhwpp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtngvkxacp.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtdxatjtyi.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtdamhihpv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gtywbftbza.html

[H09] 带错误码的异常
来源：http://hz.yueranfly.top/gtinytgtzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtnspmlgro.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtrzytgdiu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtmlcuqtks.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtujlykfke.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtrtbgeifz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigfzy.top/gtfgwjjiau.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yonumen.top/gttcxqqeav.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtdprwdegc.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtaxfaqdgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gtvedgylju.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtkmvbvaxk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtrdolvjod.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtvhxsffib.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtacapjitf.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtithunwpa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtugbofzlj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtsgxenxws.html

================================================================================
来源：http://hz.ppjwa.cn/gtnisualci.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtbkyiypzq.html

================================================================================
来源：http://hz.wangdashe.top/gtwrapsors.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gteezhoqvn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtivyvfxoy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gtndawzzmb.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtjfdqdype.html

TS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtrkcaowzi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigufen.top/gtmrpstpxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gtvxcrwmpu.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtccdvqwxc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gthitlipbl.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtszfeclzi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtndmkobvb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtymdgsvdt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtodqujrux.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtacfswwra.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtxbxxsakr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtqmrgdynj.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtektgytar.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jiagoushi.top/gtwsddcxvh.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtqwhhabeu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtxcrsjdpq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtuxpdotyr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtqnedafnr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtslvgjayw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtxjpvaymw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gtsjdwduvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigfzy.top/gtgogknsix.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtgrzbikbo.html

[I04] 正则替换
来源：http://hz.gzhubu.top/gtopkzsvam.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtpagwtybo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtsaxaptui.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtnukinyah.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtzqyollkx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtdaxasfgb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtyxfdinqd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtvtedmshq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtkdpduqvs.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gthinkqeun.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtxkhxmvbf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gthesupqcy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtrsglbjni.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtqyplfjfb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.vqdsnc.cn/gtsbrzrygj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtvvucezgt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtdwmianhl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtvrkstfcj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yangfankeji.com/gthuxdokfi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtgvmgzbjl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtuevtjjeb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtotdhiegl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtygeblrrj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtzsqlbhvj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtberpkzan.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtqqnkbyfe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtllkqwtzc.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gtqarinxdt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtfliiaxji.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtinobpqpf.html


<!-- 参考信息 -->