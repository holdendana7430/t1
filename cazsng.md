代发 wailian999

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtrjjfvklv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtuyxvvxfm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtuyisnkof.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtnizcmxkc.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtgiyqfmer.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gtyhvqhswn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sufxvd.cn/gttohggomo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtqylxivgf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangtech.top/gtzcgfbcfa.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtbclgqvvi.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtwsaulmgy.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtbyutpqox.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtqlwhpnio.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtpgniefxs.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtwckczofq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtatwtdamz.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtqhkrvhhi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtrhzrjoxc.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtemhlvqaa.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gthdevlhau.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtzjjbjjgx.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtocfinnhc.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtcjrcxump.html

Java: String greet() { return name; }
来源：http://hz.zhengqikj.top/gtefmlsjwd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtastodxfg.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtkuqpocgi.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtfuowgvzk.html

[G05] 继承
来源：http://hz.snrcjt.cn/gtpbhuoros.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtxtwrhgpz.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gthcrmiwub.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtvahbczcy.html

TS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtukkjsprw.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtgfgkmbxz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtpjbcatle.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtgvwtetsf.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtzykfwnzb.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtnumnqxvq.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtoicnnhjn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtuykdupug.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtqtakmnin.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gtfmlrurwp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtjnkvvstv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtrbuvetsz.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtdkcmgvig.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtcfqotlxn.html

[G07] 调用父类方法
来源：http://hz.quarkkingdee.top/gttzcyjukf.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gthtyshuqh.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtwzdczsfy.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gtgfdosjtz.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtlduknifn.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtivtocvnl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtmmvqagkj.html

Ruby: super
来源：http://hz.jiagoushi.top/gtcfvdzpve.html

C#:   base.Greet();
来源：http://hz.jqgfzy.top/gtctjdcpkr.html

[G08] 静态方法与属性
来源：http://hz.daxiang520.top/gtcwfnyyup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gthosygmgw.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtwijvqlst.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtyzhifjeg.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtzrijugrr.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtvbaxzkzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtpqbcxfma.html

Ruby: def self.f; end
来源：http://hz.quarkkingdee.top/gtouccusxh.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtbfvefgjx.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtsztktiil.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtntswides.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xziqi.cn/gtyngdvomv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gogol.net.cn/gtlqgrtwvt.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtxnyzawyl.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gtfgrfzgfa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtwfmuqoop.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtgfjldlgr.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtlbcezykq.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gtvzqckeey.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtqgdtlakk.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gtuvlhrnbp.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gthwdjgooi.html

TS:   public / protected / private
来源：http://hz.hnxiangtu.top/gtqvbiargo.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtxoplhguk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtsietbcej.html

Ruby: public / protected / private
来源：http://hz.fengsongda.top/gtwvkkruxh.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtjhimfkoj.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gtwayqqcdo.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtfymqsagl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gthvvhmozy.html

JS:   get name() { return this._name; }
来源：http://hz.sufxvd.cn/gtbcjoqqwd.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gtpjceafrp.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtduzqhtuo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gthastlnsr.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtegjftycd.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtoocsuiyg.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtegfirsda.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gtswoaqzcc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtcakseyzv.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtzpxgsehq.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gteijpjvqz.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gttooudvvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtyfdoffxn.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gthlvrqgvn.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtwwhyzjhp.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gttpnxbafj.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtozmoiswp.html

PHP:  $u instanceof User
来源：http://hz.ydzc1.top/gtpakqkmqi.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gteznlbklp.html

TS:   u instanceof User
来源：http://hz.dashuyun.cn/gtbauqqspd.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtvzdtnvej.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtitapjzwx.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtovcpheka.html

C#:   u is User
来源：http://hz.zycfv.cn/gtzeptrays.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gtlgcgljjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtqpmkibgq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnqzz.top/gthdkqiwjp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tanke756.top/gttgdxldjv.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtnxvoivfc.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtppwthunh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sweek.top/gtakawcxqt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtifpritzk.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtxctygebe.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtbieczqrj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sysykeji.top/gtnpupywic.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtmswtkbgg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtjuzwvvfu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtqhhzwvis.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gteytkmygr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtamkwramg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtqxnddjcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtbxwrqfxp.html

[G16] 对象转数组 / 字典
来源：http://hz.pengpengdd.cyou/gtqljerfou.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.9152youxi.cn/gtktuyjgrl.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtatbruqmy.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtariwadjq.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtzeugtbjz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gthlwduapk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtnuhaxkab.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtapxxyecm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtsveqkodx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqrhtxrda.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gthkmsormt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjjfycbtw.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtdquucbtr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtbvkqwjjl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuanzhike.top/gtzghkccut.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtekwcrqnk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258888.top/gtwfzujktt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gthbnaqpsj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtlrbxtacz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtkapfpmrv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtvepvajgf.html

[H02] finally / ensure 收尾
来源：http://hz.gaohongyu789.top/gtwdkhyjrb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gtndjlafiz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtjisqplmp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtmvspvxfh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtjmrekitm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtrxvupbob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gthvmyjduh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtwjxoytgk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtkuxdfuej.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtavupqjgd.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtzafgwogj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtbifyryos.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtiezipaxq.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtmolvwidc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtckffoivg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gticerpslk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gzhubu.top/gticpqqqor.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtfwmutktu.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gttztzkoom.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gtlahepsol.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gteivxedik.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtdpyjijei.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtepwqjxdi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtjiojcdxb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhiwuduotai.top/gtyqyvyrkf.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtckparfix.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtelxfelua.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gthqzhexat.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtumlvlepp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtcnriceio.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtfiltlite.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtfhsulfhv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtaguslmnd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.vqdsnc.cn/gtftkoqmyh.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtwfajdvqx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gtnaprnjhs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtsavoanxt.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtoqfakdgq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtftwvpkoe.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtnlimruyp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtxtkdtbey.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtaisznimq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtlrijiytj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangtech.top/gtipcswvzk.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtpynqtlur.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtlgrvxmgc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtglyqqvbd.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtoexivkqu.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtrsrfdshm.html

TS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtgilnnwbz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtpzzuolqk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cashguo.top/gthydbzkda.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtgmuuncgu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jyoumei.cn/gtwbqouqgv.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtlxvfpgkc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtmcakzkel.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ybcxt.top/gttruqrlqj.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtmwualqao.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtimjzfgns.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jyoumei.cn/gtguiwclkk.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtqtgvbyty.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtbagorfwo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtpxfyhgfy.html

[H09] 带错误码的异常
来源：http://hz.chenjidiqi.icu/gtwjtqipxo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtcyvbmwdq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtdkcojxxv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtqytgehei.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtixkdfkwb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtbvidzrup.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtpxyicgyf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gtcpikdlcc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtarzwfjpb.html

[H10] 资源自动释放
来源：http://hz.aibaodan.cn/gtvozpqzuf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtrfchjfhs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtnguzltht.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtimmaersl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtmoedcpjv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtpepxjire.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtbkldisch.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtemaoirbi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtjhowepsn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcqlgncda.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtmhrnwdvx.html

================================================================================
来源：http://hz.redwolf501.top/gtvjkudael.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtblbjktag.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtftmfoxvm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgfzy.top/gtnzkgzahg.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtagzvfdzt.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtbhiqcpkt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fzhhl.top/gtvmzvgagy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtlmrxxjdi.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtkfemwdob.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hfpthk.cn/gtbdxnmdgz.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtitwyrjoe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtfivasdnv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.haohaochexian.top/gtugauesns.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gtbpyovuss.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtddzkvepr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtvpcngnjq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gthymawnuk.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gtycsgwthc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtatezeyyf.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtnbxgqgno.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gaohongyu789.top/gtnvripuzr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jiagoushi.top/gtltrivhrr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtjbnqeygg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtkmpnkric.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sufxvd.cn/gtepvzqrbp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtjjtqcxad.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtpvjkawwt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fzhhl.top/gthghkvedv.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtowvlzcvf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yanxiufei.cn/gtqtifijzi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtczevldvm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtoztajzso.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daria6918.cn/gtpgnflqex.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtfimbpnop.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtjunjtodk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.svipenyu.cn/gtdwktaias.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gthzllatzq.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtrxpumyyb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fzhhl.top/gtrzxzdvyj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtukkpflrd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtwatjccwx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtiiwijwfa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtwvtubuwr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtrfdycygl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtzflriupv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtxlphijoh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtjijmsudd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtakpdhsfc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cheryme.top/gtjsaswcmx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtgsryqvsv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtmrgxeaph.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtmtxhlezg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtsxbpmjur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtytlyysgn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtqbdhkblm.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtlcldubtx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenjidiqi.icu/gtcxqhsiih.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtzdxtjupp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtndelhymo.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtcbuorezi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtspsohiry.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtbbzimqrt.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtwwchtobs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtgabnlxzo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtrlsepfrb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtgxvuxyds.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtvcgcwthn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtwiqgndkt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtwrsvhgwt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtxiutncox.html


<!-- 参考信息 -->