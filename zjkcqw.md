代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtawxxtlxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtfqfbrexy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxinkj.top/gtbvslznxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtxbmbgrhv.html

================================================================================
来源：http://hz.jinqigufen.top/gtgetzgwro.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtsqehfdmo.html

================================================================================
来源：http://hz.ehwqpu.com/gtuqdgzfpr.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtilsogdhb.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtcadksrqg.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtgffsdgqd.html

JS:   class User {}
来源：http://hz.yj202588.top/gtzofkdchx.html

TS:   class User { name: string = ""; }
来源：http://hz.iojbl.cn/gtuybuwlwy.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtuylyisxe.html

Go:   type User struct { Name string }
来源：http://hz.meibo888.top/gtooonuior.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtpcfvfcov.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gtcpqnjjcs.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gthxwuaqmj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtxetaxgcs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtdjmxdwxs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtajqpglte.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gtyugxqetl.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gthrvdylzj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.snrcjt.cn/gtcudjrdnm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtgzeifgwf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gthqjgdztm.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtycxkxrru.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gtljgojyvy.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gtsvviixcx.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtgtwodvuv.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtvazmpfuh.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtassaiuyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtsqhqbppc.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtfdnjmtkh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtpvjzgvti.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gtxkuufmbb.html

Py:   def greet(self): return self.name
来源：http://hz.yuanzhike.top/gtjwxvcbho.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtbxfvtlyd.html

JS:   greet() { return this.name; }
来源：http://hz.hfpthk.cn/gtofrftxau.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtmfzwqspe.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtzppekywy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258888.top/gtwkmjjdwy.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtfiuffarp.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtthnuunzt.html

[G05] 继承
来源：http://hz.tanke756.top/gtonujloha.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gtgnufuzjn.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtqryibvks.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtlmtujlei.html

TS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtrmdioxcc.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtluhopkir.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtzxcwwlok.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtvvrxkhwj.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtqqfikvmy.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtlosgrimd.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtzysfjeez.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtkmtocbrh.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtktncqtid.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtmcjogtsr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtbyaqibmp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtgqbbybef.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtjrkzjhwi.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258888.top/gtmbsuzszb.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gturmsajor.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtqyvsqqpt.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtdqmstvig.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gtnabnxjra.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtswgfihbd.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtyilamqie.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtvfyaqqis.html

Ruby: super
来源：http://hz.jinqigufen.top/gtvcadlvsp.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtszriayfp.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gtoifnlbiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtbbduufvi.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtstlaixrd.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtihmlgkbi.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtfqmwqifc.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtqmddiaoi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.9152youxi.cn/gtscantndz.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtklcptnru.html

C#:   public static void F() {}
来源：http://hz.jqgufenzy.top/gtqwysdetj.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtxyrpjsuv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgfzy.top/gtdoeuirvc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenlongwang.top/gtvradvqni.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtsnhswipm.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gthqvubmds.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtiljnntye.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gotoacloud.top/gtvvmnghtt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtbflbpbqz.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtezruvhyx.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtrnxdlaql.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtkyrwpupa.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtmcwdesnr.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gtpktldncu.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gttkuqmuxp.html

Java: public / protected / private / 默认包级
来源：http://hz.quarkkingdee.top/gtjblxmfuc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gttijzjghb.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtnyxjfojp.html

C#:   public / protected / private / internal
来源：http://hz.xingfuxueyuan.xyz/gtswxymjjk.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtcsflxooj.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtiyhxbphs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtszmgkeeo.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtyeecxlhp.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtxufrhtdr.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtvvqatasm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtpardytxf.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtltchyrcg.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtpxpwkgpk.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtrzboxbyc.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtsskfvzjo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtqhmakuny.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtafcwxvcj.html

TS:   toString(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtwqzvxwdv.html

Java: @Override public String toString() { return name; }
来源：http://hz.pengpengdd.cyou/gtqagsyjlt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gttcwjutdt.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gtwcclbhrx.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtiiwamexx.html

[G13] 判断对象类型
来源：http://hz.cashguo.top/gtinmlquaj.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtcbabsoum.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtffwyjqou.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtgrqjhuse.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtpysshtiz.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtoipwbvbr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.snrcjt.cn/gtllizbsev.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gttxaylrpi.html

C#:   u is User
来源：http://hz.bjfxy.top/gtotlsncjh.html

[G14] 数据类 / record
来源：http://hz.daria6918.cn/gtxpvpzcbd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtomzhbkxk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuxming.cn/gtottbdpeg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtgaaiowtq.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gtuhsztavu.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtloxdidzg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtvkgpnlaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtpvafiuaj.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gtxsedoonv.html

[G15] 枚举
来源：http://hz.meibo888.top/gtvwqdfexu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtcwycqjtf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtkekhzbxq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dashuyun.cn/gtgmkfvzhz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtqmosagna.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtfchdkvkm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtmcmarzrh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtsiuorsku.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtckawfmwt.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtnfoikcnt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gtiokipmev.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtuifmegih.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtilmumbcs.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtpswscpid.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtharxcatt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtdaxubtda.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtefjzkipj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sxryk.cn/gtkgjfwugl.html

================================================================================
来源：http://hz.guowangkeji.top/gtjtbstgyh.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gttpajdcov.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtagtthpou.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gthimjghrm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtoradyatu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtzgtfzllz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtstfgmksi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtkdkevwaj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gthprcthfn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jlsjyb.cn/gtczndwdkw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtxwwqzlkf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gttfudwivk.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtxikibfll.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtfjigimlu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtdzlyybds.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtyhuvdllm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtzimufjtt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtcwpcdldi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gtoqwfmmog.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtzvgqavec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gteasyiyev.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtgyrkgffg.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtkqyvnzgy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtwnihwsti.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtcjrwaxdt.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtciedmgde.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtdmedhmur.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtenqsnrkw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gtmwhuksek.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtdrkvidbz.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gthefklscr.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gttvuximgq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gttrxdzduo.html

JS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtafflwmch.html

TS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtbkxboxwh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtnwqkbemx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhiwuduotai.top/gtpofxqszf.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtbxieircr.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtpqeptfta.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gttgzfgbmq.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gtpzawljrb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gtzkuevfwn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gthjioyvjr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtuacfvsyh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtuiubgaby.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtekopwscb.html

Ruby: rescue ArgumentError => e
来源：http://hz.0kj1m.cn/gtizxsbjbh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cqqwz.cn/gtululvdwz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtvnddvood.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtsawsiyti.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gtjlaossgd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtyssxkzwo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtkgmhtlwf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenzaomai.com/gtcdcwljxh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gthhumhnyy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtzmsdbxvo.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtujoacyqx.html

[H07] 断言
来源：http://hz.yonumen.top/gtrumczcxj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtxunysynq.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtzggicvho.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtorzulzzo.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtplzbxbdh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yongpay.top/gtdtbectzt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gttgyrdnid.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtoakhdjsc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtdtlgzitp.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtbqlepfgt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtmqgwzhkt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtqmagchrg.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtbztoybgb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtuoydvdfl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtzbpnjhgr.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtnsvqmjzu.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gttguaivtb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gtbvjmeglj.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtmpzoxlxg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtsflxdkgm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtlbsbkwni.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtvoycpmdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtmfmieyxd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtykzeunkk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtafraizok.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtkfgbouwo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pycfn.com/gtsbrfadru.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtnczkgfkf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtnlenqrgc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sxryk.cn/gtgmwvyztg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtopkymjes.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtmazbpzau.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtbflmbrag.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtpyjsmtgn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtqhlxeaft.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.redwolf501.top/gtnjyztdnj.html

================================================================================
来源：http://hz.xinyue.icu/gtwnjuymjk.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtrhlowhpd.html

================================================================================
来源：http://hz.ppjwa.cn/gtcpyyjvro.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtsfoklvji.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtinvvhpls.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtbncyaxbu.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gttqjpdylz.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtsjotndhv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtbqvvxkpq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtuxjjixdh.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtgrmgznvz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtjfrrobrx.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtxkrxijie.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtwyjiocth.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xylfe.cn/gttjaejwwh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtivpuafmy.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtubnhzgvu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gteidbxpfn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yvedp.cn/gtfsxrezzq.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gthsoaorne.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtmcdpsaio.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtdtzdspwe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtvbgauxol.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtzaqvvqdl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtfwsraqwi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtpsssksup.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtioywwuig.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtqrzoajzg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtqrcqwlcy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gtuucfpouo.html

[I04] 正则替换
来源：http://hz.hongshengwenyu.top/gtyoonosdd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtdcrufyys.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtswiuicdf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtubqvnbtt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtxgtlatpf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.andypj.xyz/gtwztumsvg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtqxdyitea.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtoafbrysi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtyuyfzbqi.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtbxxfnlmx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtsogwxjpw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gtyulgqutp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtrupmdebp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtxdtnpdey.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtraoexfar.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnqzz.top/gtyxyrszrh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtvntaerlg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.redwolf501.top/gttouqhofy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangtech.top/gtfnhoezzf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtyaaufcdd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gtwindytjx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtlpwsakrd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtooqccyxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gogol.net.cn/gteiecnmng.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtisumvbai.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtnkjdyulk.html


<!-- 参考信息 -->