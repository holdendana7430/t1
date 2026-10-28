代发 wailian999

[G02] 构造函数
来源：http://hz.sysykeji.top/gtwlqyvpyd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtzdoibroi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangkeji.top/gtplnktvrk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtxyivjcwx.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtlgwmrfwo.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtzwobvniy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gtrzedrufa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gthxbbptfq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtbnfixvik.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtorwoqoac.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtqhcekefi.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtokfqriyq.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtsnjqntht.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtkvfyojsh.html

Java: private String name;
来源：http://hz.zycfv.cn/gtucpntrxy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gttajehcxw.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gtdvfbflna.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtfcgjgiwt.html

[G04] 定义方法
来源：http://hz.pengpengdd.cyou/gtclqogupr.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtqemgqkbw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtmsdhopmr.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtcclrzmne.html

TS:   greet(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtndoveoob.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtoogwesne.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tianlin.xyz/gtohrgazwk.html

Ruby: def greet; @name; end
来源：http://hz.ydzc1.top/gtgnwjvgrl.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtagcjujme.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtvgajcpie.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtztqiznhu.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gttosaxued.html

JS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gthexycgbb.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtimgilzce.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtlgkskxml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtvwlzrfvx.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtuufduges.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gteuzddiyd.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtizibcsuc.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gtnkhztykm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtyrxqynix.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtudazhnyh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtikatwtub.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtxutynvho.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xinyue.icu/gtkvvwyuhv.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtdjprjctz.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtocyezutp.html

[G07] 调用父类方法
来源：http://hz.ydzc1.top/gtzyirqcbn.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtqcquoydi.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtjctpglmm.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtgqdbwwbx.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtbxmkrmhp.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtlqdttkqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtwcqfjjag.html

Ruby: super
来源：http://hz.jlsjyb.cn/gtopiguwck.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtmzsnzhsx.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gteppvpxly.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtbejulflw.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtabeksspe.html

JS:   static f() {}
来源：http://hz.zhixingplan.top/gtwtyjoqlw.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtohqwovfu.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtibrxziuw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gtdnnrlyas.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtntggeswb.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtsijwvmmf.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtvkhbzamu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tian-w.cn/gtpogyqzyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtxlbbwewg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtxlrxvmqb.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtdikkxvrd.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtvqenabuy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhengqikj.top/gtlhemoigm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.iojbl.cn/gtjrhisiav.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtnubolywh.html

[G10] 访问控制
来源：http://hz.cashguo.top/gteswpjfem.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtlxkqzljr.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtijkkmzwb.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtendytzbk.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtrseklfzu.html

Java: public / protected / private / 默认包级
来源：http://hz.yuanzhike.top/gtuqnjiamr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtvnoqjhbr.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gthbiixxsc.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtpyshuseu.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtznogckwx.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtlgrfbzwr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtzsbuhycq.html

JS:   get name() { return this._name; }
来源：http://hz.ydjk.org.cn/gtduvyvner.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gtgfowfjtg.html

Java: public String getName() { return name; }
来源：http://hz.jyoumei.cn/gtilzfbcng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jiagoushi.top/gthurecvps.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gthowqjnbn.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtytwmrivw.html

[G12] 对象转字符串
来源：http://hz.guowangkeji.top/gtrjsaublf.html

Py:   def __str__(self): return self.name
来源：http://hz.jianghu66.top/gtkpexjoja.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtwtkppudl.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gthkbzbcif.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuanzhike.top/gteuatytik.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtlpwbfjdp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtolaauiks.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtqswcwtcn.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtmbzcgizg.html

[G13] 判断对象类型
来源：http://hz.ydjk.org.cn/gtthnrsofi.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gtvkgmycxz.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtusnillpj.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtgahscouh.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtckistuob.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtqrgwsadk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtbrcpmjcu.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtlzyrfgni.html

C#:   u is User
来源：http://hz.nanxinkj.top/gtmqcflnem.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtgotmijkq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtscblande.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtlwgmwmpc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtwlbpjifq.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtehylvsku.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtqrnhcdnw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258.top/gtjipeyvma.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gtzmuljegt.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gteetzjwlh.html

[G15] 枚举
来源：http://hz.52xcode.cn/gttrdzeqtz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtojdelzfm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtkoerltgf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtqijuhfyg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtfgmgkxtz.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtlpcdybbv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gttukiogtp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtmfjjmyzj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtkljsatem.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtqmvfzkoi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtywxhiqxk.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtdgaehvbd.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtpppsvwkn.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtzxwbsgdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtwokytaai.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtlytxidjn.html

Ruby: obj.instance_variables
来源：http://hz.feifeiyinyue.top/gtypssydxh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pengpengdd.cyou/gtaeyxedhg.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gteearrrje.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtzeiwijce.html

================================================================================
来源：http://hz.yuanzhike.top/gturayxazl.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtkbzeisad.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtidizuqih.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtxtgnjlrf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtgrtwixtn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gtowdyeuxe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtewsbspnv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtncdaxiwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtjzuqssss.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtrlhwxjcw.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtjsqmxfzf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtamjwvfcv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtmpzdxsia.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtyprbkuyv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gthgmdlxrj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtqkekqohe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtxyklssst.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtovhewywb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gthgkiwcuf.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtomgdyebd.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gtxzinuvfk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtjupvxczy.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtwtchbvst.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtzwyrpnfu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtitumiwnq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ehwqpu.com/gtenyjwrtb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtcwsjhobg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtzcnzknuk.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtsbfsildo.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtjgcmuhnh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtyyepgvoi.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtocfnczfw.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtwjggjwlg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gthjdbdxbf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtvmblrsfg.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtqngmtkym.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gttgpswdun.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtogwwoxqh.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtxrleuiii.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtiuuthcpb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtfmkcsamh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtvphgghry.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.snrcjt.cn/gtofxzzvso.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtnhznqqzr.html

Ruby: rescue ArgumentError => e
来源：http://hz.ywan-chungtsiang.top/gtrsooixmd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxuanxn.top/gtbviuztej.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nwbrower.top/gtttrhwbjo.html

Py:   value = d.get("k") or default
来源：http://hz.shangyingyoupin.top/gtotaejfpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtaoqtyzwn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtpgobxejm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gthbbwquyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtvqdaxwxt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtobryfjqq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gttmrairak.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gtjwwotzjk.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtclbzyexm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtpcjcijdj.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtubcysxke.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtjmstoght.html

TS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtujeybffl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtkcptknpl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtkpsiojuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cdnleiting.top/gtklrjogiv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtymikgrss.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gtkqowbbyt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtxsuzgzhd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gttponiygf.html

JS:   e.message;  e.stack
来源：http://hz.fengsongda.top/gtwrdtijjd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtxafwcogs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtflbymruz.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtwnppbdcx.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtmotqaijm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtyzfktdlx.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtokiaxlrd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtglcnvyyb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtxredsjuc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ybcxt.top/gttjdzvjht.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtukxlaloy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtictfnzyb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gtpgmzyagg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtibavvkrz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ivvv.top/gtsmcfenat.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtlvfsidsc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtndjhmoid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtjpwbefkb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtghaajnyd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtofhvegja.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gtvvlovbbg.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtztzrqumm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtmstrgkuj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtjhxmgkmu.html

================================================================================
来源：http://hz.sysykeji.top/gtwkfdhsdz.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtnserjgil.html

================================================================================
来源：http://hz.daria6918.cn/gtpliscgne.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtgyhrxgxs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtwixclqzz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtvxwxikzb.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtwlbfeqlp.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtyliccnbe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gthjuriqkf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtwylkhmlb.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtdwpxmvaf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtgphnycma.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtipehjkfj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtnfiahsqt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aizwys.cn/gtkzerkbpi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinghuilouyu.cn/gtgafgdenb.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gthgoiampq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nwbrower.top/gteupuqvru.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtemlcqmfn.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtgrtzmuyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtrbnoabyo.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtbupjynfr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtblidsdsd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xziqi.cn/gthmzvhius.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtodssqujp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gtgifxfmqm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtdnaemagt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtfeifaaru.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtxmnkgifw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtswbmftyf.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtasomehzl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtaaibhzhf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gtjsqitucz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtouhxzjst.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gthiereyxu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtgtrrfoum.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnxiangtu.top/gtxnvpxpas.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtkdyxdijf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtflznbeab.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtqnfklxtm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtnyesmecb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtkqvgpxat.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtyljfdamh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtvavzirmn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daria6918.cn/gtcurxxsez.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtcpoxsdvz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtmwozmplu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtbcbeyqcu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtnxgidjrl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtcmyuxrjj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydzc1.top/gtxdrjqxxq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtmnefnkmt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtlpjhnzlz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtpzjgedto.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtoagkkbey.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtmpawenwu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtofsvpyms.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtcaiboslb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtdhyjaicr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtvggbvjir.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj202588.top/gtkbabwbmo.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtlmrvhjvm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtmsjdynrs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtwtcforcs.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtwalzukfd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtmhekprzf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sufxvd.cn/gtyzbutjzw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtmjewsptf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.9152youxi.cn/gtfelwarbt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtbtedfxgk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtugxywbsv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtzactobnm.html


<!-- 参考信息 -->