代发 wailian999

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtnltlacjd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dashuyun.cn/gteuhavjhc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gthhshvuxs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtnbdhylcg.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtjpkfwzel.html

Java: User(String name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gteosfkszy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.smart0.xyz/gtbbkxxerk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtbaxtwnzv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtszzjtamx.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtztbxtfgl.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtjfubfrek.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtrdfurodc.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gtuezexvdg.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtxyfemnyu.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtgkvviwhp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtyvryxrfa.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gtevteyvmq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtvzksyspo.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtjvfwvufc.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtnidqoxkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtrrfyqmhc.html

JS:   greet() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtbcwzgpda.html

TS:   greet(): string { return this.name; }
来源：http://hz.meibo888.top/gtqhsqpjat.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtfferxzdx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gtinmqrnvy.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtimwyunxg.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtyhbzvluh.html

[G05] 继承
来源：http://hz.sysykeji.top/gtswnblkto.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtauffqrpf.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtwzogvnqr.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtleqahucd.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtfntezkyu.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtihhidoxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenlongwang.top/gtfrxxzlur.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gthenwsqkt.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtjdsvmbhg.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtjoojcohn.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtjcflbmog.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtglijoywd.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtmytwiyeo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gttbgjkqsl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtriqwcnug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangshuangyany.cn/gtukjplpys.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtajclkiox.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtljkyjyvn.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gttxrzbzgd.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gtmbmlzelk.html

PHP:  parent::greet();
来源：http://hz.0kj1m.cn/gttpblnosr.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtplclbuwd.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtgydxkxci.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtttnyanxk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hysaishi.cn/gtbxpcemym.html

Ruby: super
来源：http://hz.ehwqpu.com/gtvcrshsto.html

C#:   base.Greet();
来源：http://hz.jqgufenzy.top/gthbofffqt.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtelrleuwp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtvbyuvjyx.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gttpxefxyi.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gthbavgbwe.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtjxemkfat.html

Java: static void f() {}
来源：http://hz.gzhubu.top/gttckhzsvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258888.top/gtojkvbjgh.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtpekqyimv.html

C#:   public static void F() {}
来源：http://hz.vqdsnc.cn/gthtnmscxc.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtfmnkeruy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtyyyiixpu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtgdqkymtm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtqgfnulsk.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtokjbszdp.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gttmrjdoje.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtdpozsuon.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sxryk.cn/gtbwjygieo.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtnlfdnqur.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtzdevftae.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtaqgdzpzo.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtkdxpeikk.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtuglstqwm.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtaqocyikk.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtppwuvzxm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangkeji.top/gtlgnclchc.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gttcanfkcg.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtrlzqesyg.html

[G11] getter / setter
来源：http://hz.feifeiyinyue.top/gtzcklkhcb.html

Py:   @property 与 @x.setter
来源：http://hz.xuanzx.com/gtyqwsijxl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.havefunace.top/gthenqrvsi.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtsltphqge.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gthtwdcvxu.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtyoacyopt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hywenlv.cn/gtezfngmfx.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtyrznjehb.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtvdhlndxk.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gtgqljymrz.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gthasomzzz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtsamipyop.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtxgxwmrte.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtjcrzibun.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtczwvvidq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.9152youxi.cn/gtyspiuwlx.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtirrauqne.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtyqfevpde.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtjzhwxwyj.html

Py:   isinstance(u, User)
来源：http://hz.zhaomingkeji.xyz/gttxhetknt.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtmhkmklhs.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtwsmplkic.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtlxplizdf.html

Java: u instanceof User
来源：http://hz.smart0.xyz/gtsxkheozc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtkaanfdyi.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtbdycfxsc.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtquabcous.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtccastdal.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtkecwosid.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtqpnvfzpu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gtchvkdqyv.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gttdyprsen.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtcunvturx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtittcwzjc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtutlgrujb.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtsjrdbtpv.html

[G15] 枚举
来源：http://hz.nwbrower.top/gttnijgwjh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtpnsuvirw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtlwdulxxw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gttzzbmdsh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtnesjymcx.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtspsdrjxj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtiheqspun.html

Ruby: Color = %i[red green].freeze
来源：http://hz.birdmap.top/gtnynovnwg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtbfwycrjx.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtzbmfgcbv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gtdcmfxnyz.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtjyivcnoa.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtjtufmyrj.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtaartpqfe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gttavocgto.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtvmizncob.html

Ruby: obj.instance_variables
来源：http://hz.yongpay.top/gtqwztxfbc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cheryme.top/gtkkeorucs.html

================================================================================
来源：http://hz.hysaishi.cn/gtewlwsdkp.html

H. 异常与错误处理
来源：http://hz.chenzaomai.com/gtjyleawlc.html

================================================================================
来源：http://hz.jyoumei.cn/gtbjjnqrgz.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtwxslmeps.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtsifzhupf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gtzkilbdfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtlalyvzht.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtcmaqvwlv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtikcxudhb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtpgygfipa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtgqvcvjun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gtckqcghci.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtdeqtcmjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.snrcjt.cn/gtsxovtpgj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtoouyyzgx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtuyayrtya.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gteymmehmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtagtjrqtv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtlmimyulb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtifmtnvbu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gtelklmkfs.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gthnrgzwdm.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtrnnnxquw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtpwwofjgp.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtghbeuafk.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtfgfryksa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtxzhrllsi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtajbhniej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtpcoamuhm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtxrrxncbp.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtghwopxdj.html

Py:   class MyError(Exception): pass
来源：http://hz.yuanzhike.top/gtcerhgaut.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtvsqewpja.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtrbxyfubs.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtpwhmxtfx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtwscvljsr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtrnelcdnu.html

Ruby: class MyError < StandardError; end
来源：http://hz.aizwys.cn/gteilddlag.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtvdytahtw.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtpwbpmpbo.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gtuzaxkkhc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtigdcmujw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtsubkzjbl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtfjzeoilj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtdsyxrkht.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtzdkoipxr.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtfgayepcf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gthacjerge.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtmujooqxh.html

Py:   value = d.get("k") or default
来源：http://hz.xingfuxueyuan.xyz/gtiljdicow.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtxsvghkgg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtgdjbppje.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtrlfdkrtj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtuzesfzhy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtaszohcab.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtvfrpxtiy.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtujcdgoiw.html

[H07] 断言
来源：http://hz.ivvv.top/gtsvoxyqaw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtbkpscbak.html

PHP:  assert($x > 0);
来源：http://hz.feifeiyinyue.top/gtrlabcths.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtzskklary.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtmyioybza.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtbtavlwop.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtzvexlrvm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtywbonzgd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtecrckqvg.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtnorffbou.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.andypj.xyz/gtimxyeppf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtonumknxt.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtblhhpsio.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtkqevjzeo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gtpaqftkym.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtlaybouxq.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gttmznijhb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gtinjgesag.html

[H09] 带错误码的异常
来源：http://hz.hywenlv.cn/gtncwpwfwc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gthcopzmye.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtxcmedmtk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.316326.xyz/gtmnjltgau.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gthrwxidoh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtcizmvadu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.9152youxi.cn/gttdskcawm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtsvelqgwg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gtrvdwrnwv.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtyaexlvjy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtpnoqknxz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zdqjudy.top/gtdkmgsyal.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtzekuhqsr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtibhvhbjp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtyxwadmdk.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gttyvqaffn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtwdvudjio.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtaxztmlas.html

================================================================================
来源：http://hz.ppjwa.cn/gttydscgja.html

I. 正则表达式
来源：http://hz.sxryk.cn/gtqouunzqi.html

================================================================================
来源：http://hz.yj20258888.top/gtsbrgnpqd.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtjwmdvalb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtieraytij.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtirlodqax.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtnpqvcbgp.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtlqmppbrc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtbleixwhi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtyzcewxlx.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtyvqthgxy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gtppbpihia.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtplecjkua.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtfnlkxmfq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenzaomai.com/gttsscbclw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtwwiaomei.html

TS:   s.match(/\d+/g)
来源：http://hz.aizwys.cn/gtptszqbjf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtahlmxdux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtadsjtasa.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtcgddebvt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtvfsldzzi.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtjqphpakm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtcynobqwx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydzc1.top/gtmlhuuiio.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtftbwzxck.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtwezbqdjr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gthfnjwpoz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gtkohayecm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jianghu66.top/gtwulctipq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtvpeupawm.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtqgsyqrbi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gttwtoqvxz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtmqupdmln.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtcxlpxqog.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtugvzfygf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtxajdkfpy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtveoibrsi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtqitwzspg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtfsuuwnzb.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtyckffazh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtyegdegzx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gthpmsyvvo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtlbiftdvp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtjcovwrtt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtafsbbmeh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtrslnlfuk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtgnurmlwo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtinfpuxvv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dianchejie.cn/gtnctoviwm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtovtbevkb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yangfankeji.com/gtldvyygfk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gteqopnmdj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtjmgmzghn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zycfv.cn/gthbzmizyp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aizwys.cn/gtdufkprwe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtbzprjsdq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtxjimofay.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtubfyrdca.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtdyaqhydd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtmzcidmpn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtzxqlzumh.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtgtvuvocm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtawuiycyr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtphcscgua.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtycrmltrx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtwljinevl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtpanytcwa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtrbruowhz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtjlhmpgnc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtwfchocvg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gttmkazoao.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtdavqqebb.html


<!-- 参考信息 -->