代发 wailian999

Java: class User {}
来源：http://hz.zhengqikj.top/gtkluutlml.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtgfejfurk.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtjquevxnc.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtyavrsrjs.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtvmyysadu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cashguo.top/gtlvynmihu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gteojuazkr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtxogyezhp.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gttfwmugsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtcisdvtiv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuanzx.com/gtkgmhydin.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuetiantiany.cn/gtcfbdybla.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtirabxjhn.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtnzzuwezq.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gthxvyrsrm.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtnuktajea.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gthgzaunlc.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtkjumldef.html

Java: private String name;
来源：http://hz.cheryme.top/gtsjxjiarj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtjlksrgvv.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gtevdteylu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gthbwguexc.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtmumdxpih.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gtwcshllwk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtzecmsmod.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtwclhfppe.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtlhvfbqjn.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gtbkytzgjt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gttetaudea.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtcjkhrzki.html

C#:   public string Greet() => Name;
来源：http://hz.yuanzhike.top/gtkoeacnbt.html

[G05] 继承
来源：http://hz.jqgufenzy.top/gtdhelqsau.html

Py:   class Admin(User): pass
来源：http://hz.jqgufenzy.top/gtclrnvfqa.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtwvzzjeqg.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtiicljjhd.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtcmadsezw.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtkschqprr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtiqlquaev.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtnezqkmkk.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtbvuxggdl.html

[G06] 重写方法
来源：http://hz.nanxuanxn.top/gtnfoepjea.html

Py:   def greet(self): return "admin"
来源：http://hz.yj202588.top/gtqwsdgams.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtuoegxhrt.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gtfrnivkrp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtorekqojc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtfpiicgxp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.birdmap.top/gtwkqmahjz.html

Ruby: def greet; "admin"; end
来源：http://hz.hysaishi.cn/gtscymhgfw.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtjfzbyvza.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtathvszvr.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtroytmklt.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtzhnkisjj.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtjvijgxzv.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtmkyorutv.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtezitmyyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shangyingyoupin.top/gtauoolarc.html

Ruby: super
来源：http://hz.yanxiufei.cn/gtaurcabhy.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtirjettel.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtcrloqzhn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtyrvwttlr.html

PHP:  public static function f() {}
来源：http://hz.ywan-chungtsiang.top/gtzaicckbd.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gthqqhfpso.html

TS:   static f(): void {}
来源：http://hz.52xcode.cn/gtsketndrz.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtekylmukt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtgecqfubj.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtswtjogup.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtdzlmnhiu.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtjdeavaiu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtxxgnewsk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtqeafgdne.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuetiantiany.cn/gtwfizvxtl.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtnbkhqbpg.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtswzajzcg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtqmhiowny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gttybpnldt.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtivjgbaiv.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gtnwffpnnp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtifbbbrjh.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gteozgsuip.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtbfjrrzfs.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtowcpdhlb.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtpssmzfgn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gthaorphod.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gteqvaehmz.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtavjuaasx.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtgfxalijd.html

Py:   @property 与 @x.setter
来源：http://hz.zhijiandao.cn/gtiagjfwph.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hammf.cn/gtnxcvfjrq.html

JS:   get name() { return this._name; }
来源：http://hz.jqgfzy.top/gtcyaokver.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhixingplan.top/gtfpvkwnjd.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtauolzcda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtfzauphcd.html

Ruby: attr_accessor :name
来源：http://hz.tianlin.xyz/gtalzldawh.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gthvcbxxpn.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtxkhgtidw.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtxmkqrjvw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtusjwtszf.html

JS:   toString() { return this.name; }
来源：http://hz.yanxiufei.cn/gtixpukcyx.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtpjesxkgf.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtqmchkuja.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtoqbawuyk.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtnhkgnoso.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtfvjmbhpt.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gtjdnpgfhr.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtycpypxmp.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtvpjaabvw.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gthktcdybs.html

TS:   u instanceof User
来源：http://hz.xinyue.icu/gtymisctcm.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtydeyxwcy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gttvuymxwt.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gttwghdvoh.html

C#:   u is User
来源：http://hz.guowangkeji.top/gthzjdahox.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtxgbadssg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jianghu66.top/gtkazmgtyz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtctdmqtbj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtobgqmfnj.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtgsskcnto.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtzywwrtef.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtglhutuuz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtlajmftdz.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtiqtltzuz.html

[G15] 枚举
来源：http://hz.yueranfly.top/gtincqmpec.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtkqcscgmn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtjqrudqpg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.0kj1m.cn/gtzyjzuhmz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtiomzsfye.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtimdqhroy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtkxsjrpwb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtzhpprnog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtfdkpkwvo.html

[G16] 对象转数组 / 字典
来源：http://hz.zhijiandao.cn/gtbjefwfoe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.snrcjt.cn/gtrnmvoqwt.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtsjxukouw.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtgabpozsq.html

TS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtuacmldki.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtwjqhafpn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgfzy.top/gtehubmaws.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtfdgsmhsy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtbnrplsqw.html

================================================================================
来源：http://hz.xylfe.cn/gterbhvwsb.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtdhqvzhmj.html

================================================================================
来源：http://hz.yuxming.cn/gtgmryohvg.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtdjczfhrl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtujuzjpol.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtzmwmhkky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtevdjjrxo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtpdxigksx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtogqlegty.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gthzjkludy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtkcyztywa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtbqwokqob.html

[H02] finally / ensure 收尾
来源：http://hz.zhongyouzk.top/gtxexujhtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtldnjuxcr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtdiflzflq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtgqulefsk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gthvswiyvq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtdtgmwban.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtjhchpbuh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtuthvclsr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtkhacwswz.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtjtcbvnns.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtstuhvqwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtueajvyrz.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtjymxnbnh.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtawcmzgfw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtthxxkrtg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gthgfxxatu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pycfn.com/gtxwhyzced.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.meibo888.top/gtglaajwsw.html

[H04] 自定义异常类型
来源：http://hz.zhijiandao.cn/gtaofzeksi.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtxsbrbugm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtymfxflvq.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtzqoqxtfx.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtnppimjhh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sweek.top/gtzksfnoug.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtklflckxu.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtprwdrdhy.html

C#:   class MyException : Exception {}
来源：http://hz.vqdsnc.cn/gtsrtvshdj.html

[H05] 捕获特定类型
来源：http://hz.xziqi.cn/gtcudxozpr.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtrcleukgc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gtykqebbjf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtjicmxudc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtefzmqgre.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gthlibbrix.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtfbjqgcfg.html

Ruby: rescue ArgumentError => e
来源：http://hz.quarkkingdee.top/gtzbwyclwl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtxbirujog.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtvrozdwoc.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gthjpfqsbe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtmklbfcrw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtzetenbji.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtaxkqszij.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtpylnnkky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtywlozilu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dianchejie.cn/gtnqzygoec.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtybfqnpwr.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gttzvxhhly.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuetiantiany.cn/gtncwjbzvb.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtgkbtshte.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtvyrlviqd.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtctpsmswh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtusdrqrxh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhengqikj.top/gtykwycdvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtskhzautb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gtxkxzvssy.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtlzxesisg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtcvqcovxt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gtsdvtakbl.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtpcnfhmev.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtissgwupt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gtmdefpbrx.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtfqxyukav.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258.top/gtxuudaxyk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gtrvdcnnll.html

[H09] 带错误码的异常
来源：http://hz.zdqjudy.top/gtfjjiizvv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtbwqhgchg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtddegsbmy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtyhmteovk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtyhbkonkt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtygylyatv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydzc1.top/gtelirnhtq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtxcrhobka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtwunikixm.html

[H10] 资源自动释放
来源：http://hz.jqgufenzy.top/gtquqieguc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtwlgdolnx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtqqeyfwje.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtspqdotki.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtehhgpqvo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtldishfap.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtzcuzwafp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gticogzkge.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtzappzkak.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuumzhftd.html

I. 正则表达式
来源：http://hz.yuanzhike.top/gtkmyqemjx.html

================================================================================
来源：http://hz.quarkkingdee.top/gtiwdwfxvw.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtzngiqcro.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gtyfuzgppn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtankegonl.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtazliuapa.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtaczbqrut.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtyacfzhig.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtmalhqcnu.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtzgvcxnjl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gtferyizss.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtqpccfxfh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtyngkidhs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtyaotthzw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtzilifvci.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtbpjcquvn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtfcedcoff.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gttkmhnzwk.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtxzpslcja.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shangyingyoupin.top/gteplvhhsx.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtpvunbghr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtoypxbuuk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtjajzonqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gtavwehisw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtzpcvoijz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtjokqwnsh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtayiihaep.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yanxiufei.cn/gtredhlmqj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gthapptuvn.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtccomuojy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtochxuhwk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtfxegclra.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gttpcyhrtq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtjipdhcxt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtznczixmu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gtgtynvqkz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gtnmkkudlf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtrvomqoqe.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtytfdstvg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtuqqxcirz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.mhx1999.top/gtvxtkurbu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gttxcegklv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtzpeaeiur.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtsdqialim.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtydkxcvyw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtfyyqrrxr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shuidangran.top/gtmznaqhif.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gthdvcldaz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtssevikqr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtlakaojpz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtplkjeoog.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtmwwnonxi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtjkalfqsv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gtrmbgzpcn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtaskszktq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gttzmziihl.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtbxepfrmn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtfmnvoyqy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtofgvucuf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtzdkginti.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtpfyywqjb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtqvkyxxsg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtaptogrmr.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtadugbort.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtcelvprku.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.birdmap.top/gtutxbkwcq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hfpthk.cn/gtdreajpub.html


<!-- 参考信息 -->