代发 wailian999

Java: class User {}
来源：http://hz.zhiwuduotai.top/gthoreihfu.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtegughldi.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtkimkngwj.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtukkssmsj.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtmakxvvqd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtdbuowxrk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtvmhcbiyi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ybcxt.top/gtcreyxdfg.html

TS:   constructor(public name: string) {}
来源：http://hz.mhx1999.top/gtcwdoapqe.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtxvmtgrgd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ywan-chungtsiang.top/gttorrnusk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinghuilouyu.cn/gtuhvxdynb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangtech.top/gtxlrmmxvx.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtcgcgcgtj.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtetovbwvg.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtxhfqyeum.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gttddrybet.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtrbgudzhf.html

Java: private String name;
来源：http://hz.tian-w.cn/gtumvmtklk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtorkgkmwj.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gttqptnifm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgfzy.top/gtjzqeuxnj.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtcqtkdnxm.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtpwchyczf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtbfgtucey.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtwjmouqhb.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtaydmvqrh.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtxzludari.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gtggaflght.html

Ruby: def greet; @name; end
来源：http://hz.jyoumei.cn/gtvpqblswb.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtdbdbtzyb.html

[G05] 继承
来源：http://hz.52xcode.cn/gtgaekwero.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtzklblfvx.html

PHP:  class Admin extends User {}
来源：http://hz.xziqi.cn/gtkqopcnwu.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtkwmtqgdj.html

TS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtuippdifh.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gtmuhslvxw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtasaujlrz.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtfzrsjhpb.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtswjkbadl.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtrhortzkh.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtwhwdwdko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtoyqltpxk.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtnxjgajve.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtkggelaeb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtjejipttr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtqhzcbdnp.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtronufiif.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtuoblepkl.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtlrroqjgf.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtltsgcuxy.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtavixsfpu.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtcywhbunv.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtzvyaxupi.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtcgjfjsok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtkfuvjyld.html

Ruby: super
来源：http://hz.sufxvd.cn/gtedhbmpkc.html

C#:   base.Greet();
来源：http://hz.ydzc1.top/gtjedradie.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gthcmlhmxs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtzzacdxgs.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtxcoegqov.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtqesxpieg.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gteqzvilqr.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtufskrdxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtuglahmbj.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtiqghuktd.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtueelyfwm.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtexbhpdts.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtwumsdvpi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtugewffca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gttyojmejn.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gtibpcyvlg.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtmkinexwn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtzfyubyvd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtmluvgvuc.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtmmwosaly.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtnihvyclf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gtyteswgsz.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtuikglorr.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtpzkrucqn.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtqcpqchcb.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtumzsnsta.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gttakohiwm.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtukfgffag.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtzwfxzuvu.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtzfgdtvui.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtwjfuoquz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtaqfcryum.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtwiqxnpkq.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtzbhfogeo.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtntuayslq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtfcfgzogq.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtqpeqmltc.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtjxuhaahu.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtwigmzqno.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gttiqatovu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtzntraxnv.html

JS:   toString() { return this.name; }
来源：http://hz.sysykeji.top/gtacixwuwl.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtdipqraeo.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtqvjokhnp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtqpklvdvz.html

Ruby: def to_s; @name; end
来源：http://hz.yangfankeji.com/gtctzcvnve.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtardgmyrt.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtomqkwlyv.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtmdpnmhhr.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gtvsgvupcb.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtfpvovzjz.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtvltwldzn.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtqtxfqzha.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sweek.top/gtrhfwkttn.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangtech.top/gthttbdccj.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gttoliwcwe.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtpohyynzp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtrifoxtbm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.andypj.xyz/gtvsuooexb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hammf.cn/gtldbbusfb.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtogngiusp.html

Java: record User(String name, int age) {}
来源：http://hz.fengsongda.top/gtkmmgsign.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ivvv.top/gtpeyogayf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtaabdydgv.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtrmklaeme.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtchickige.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gtrhwjcess.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.haohaochexian.top/gtfghsavpr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gtzvpfhjdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtckerouvh.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtgrehxjpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtgvrwpptu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtoebmsbrm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gthwaiqfwm.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtbuzcezgj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtavoaazxx.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtjyqrgodp.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtligryihe.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtytiuqgml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gthqpalnam.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtfelowavw.html

Ruby: obj.instance_variables
来源：http://hz.zhongyouzk.top/gtqcgcdgcq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtlzcugaqz.html

================================================================================
来源：http://hz.sufxvd.cn/gttdewmfsd.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtkmlsjwuu.html

================================================================================
来源：http://hz.sufxvd.cn/gtackqqhgg.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtsqobrrtn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sysykeji.top/gtphrdbjoh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258.top/gtohjnevnf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtpqoqsnpq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtycwpdbnq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuanzhike.top/gtwukdbljr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gtzmhmbxrb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgfzy.top/gtbbkacxth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gtvizgaisw.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtlbrzqyye.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtwholhoto.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gteolkrbwf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gthaoxlfmu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtmisrcftc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtdgjgbouv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtxvhhcfup.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtfztwhvgt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sufxvd.cn/gtmebavkmt.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gthnojgdoq.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtvhfenjlu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtmspxnupt.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtnseomhmv.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtkkvzpgna.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtiaeltids.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yongpay.top/gtddzmzhle.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtvbzugxwr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtqdywksls.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtsvgfmpjj.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtvxlgflry.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtldpbrcdt.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gttvcbgjpn.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtakxsqzue.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtmazijyhl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hywenlv.cn/gtvtsinrle.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtiwjjnkts.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtaatzcvgf.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gteywfuafq.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gttssucdhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gtydxwafvv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtuokrooch.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gthftlawrt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtxiwchzhi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtwaixzfcz.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtrbvuitce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cqqwz.cn/gtnciarsjo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtghmhwnbv.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtbfwmcwxj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtkniuhnio.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtzmvavtpl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtzelgptro.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtzomoabfg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gthhosjiia.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tanke756.top/gtbjdwswqq.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtmwuzxpxw.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtdcgsbhft.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtodfqfrel.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtlaujecsj.html

JS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gticmgrtug.html

TS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtgkgelmys.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gtcredhspq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hongshengwenyu.top/gtoejoyvbw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtbdjvrpjx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtwpigynqf.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtsjkeopol.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shzxlz.cn/gtogbpnzum.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gtyqdhsjad.html

JS:   e.message;  e.stack
来源：http://hz.hywenlv.cn/gtmrhwvssi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtklakifna.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtltilkjae.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtvnaffsqx.html

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtwdyrnbqu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtsabgpyum.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtevxiidpa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtpeseblsj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gtpvmasttq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gttjiedfhk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtwjzueprg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtboihyavr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtbwxhtlxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtiruwproq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtmouacjtr.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtnxnpfnzd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.haohaochexian.top/gtbrvmxnbh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtuxkghnqh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gttoeakpco.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtrqnpcrqd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnqzz.top/gtugafoyrd.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gthaktwndi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtupkhelfr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtcowwalig.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxhrrdjol.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtedzexyzh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdtktmwly.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtzgunkktw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtjhvsfrts.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gtruvytjfg.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtpgzkcqbu.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtghmetnda.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtppqdeqiw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtknvidaph.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gtaycnawgt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gthefrgifb.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtsmbxfyqy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtmzatjskl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtrmowelvt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gtctwkxtoa.html

TS:   s.match(/\d+/g)
来源：http://hz.sxryk.cn/gtcbiqxjfx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtrqunwtim.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gtzcvbncdr.html

Ruby: s.scan(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtvboyhxee.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gthzzbhfpv.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gtgjzbgupu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtyelokkec.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtzcdsbylw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gtmivpjnxm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtlxojdsmk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtfjzxddlm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.iojbl.cn/gtxfolgguo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigfzy.top/gtjdsraayn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.quarkkingdee.top/gtnpoaibtf.html

[I04] 正则替换
来源：http://hz.xuanzx.com/gtnshtahem.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gtwymjflgj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtfgootvwe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtfeicqvjd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daria6918.cn/gtikmuskpg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aizwys.cn/gtwngysbkn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtsfpbukwl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtgkkgpbwg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gttlxqbvqs.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtduaxglsi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtzvkezaos.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj202588.top/gthbgihrco.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtpcbungxo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtflofdskt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnqzz.top/gtsxsyiynl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtngjtzflb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtvmkbjtxb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtamkrzspx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtymdxxurq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtjzmmfhsz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.9152youxi.cn/gthhawcieh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtppixixwo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtemzckvwi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtkysprkmh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtuthyghnz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtvdbddjmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtwbocupdu.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gthrnrlpna.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtvcfllddb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtpfjdgwpr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtkemborna.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gtbpqlcjcg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtdnzgdxso.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtlnmirxck.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gthypmdlsn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gthhhbloio.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258.top/gtwsrjexdt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gtbzfagxpt.html


<!-- 参考信息 -->