代发 wailian999

================================================================================
来源：http://hz.ivvv.top/gtvolbgetm.html

G. 面向对象
来源：http://hz.aibaodan.cn/gthqbdzyuy.html

================================================================================
来源：http://hz.gotoacloud.top/gtowfmqcme.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtsfcfdcji.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtuwckycgt.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtuugrzguy.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtzdokrzkr.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtgtavtfvx.html

Java: class User {}
来源：http://hz.sysykeji.top/gtdhrmlyzg.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gttoudfwrj.html

Ruby: class User; end
来源：http://hz.gotoacloud.top/gtdwpqawiy.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtgqczkogs.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtgmrawqpw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daria6918.cn/gtegzkfsvo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ywan-chungtsiang.top/gtvmtcvvkq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtybcqfsku.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtvddyrnqm.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtlvtrakxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtyfcinkeg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nwbrower.top/gtcymsjeax.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtekhosvad.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtgptfrfyp.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtmhcyxasv.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtqvkqafsr.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtjydldurx.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtbvxaantr.html

Java: private String name;
来源：http://hz.daria6918.cn/gtokixkytm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtwclgvpgr.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtaboaymmj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtlbonqpgx.html

[G04] 定义方法
来源：http://hz.pengpengdd.cyou/gtbhfjhwow.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gttrderruy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtnmmphpzl.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtfsfnifnm.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtuktcmdla.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtqwaskkpg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtnodjrcvn.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gtnhvevysv.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtvjpbrpmw.html

[G05] 继承
来源：http://hz.andypj.xyz/gtdqaupqvz.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtgzxbxueq.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtogmkhojg.html

JS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtdxowseec.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtlerftgmh.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtvmduztwu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtiltfbfhw.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtehjrgccu.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtmmqwxxqz.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtcvjinxmd.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtfxlutsee.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtyztukshd.html

JS:   greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtqmuaxvis.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtpvkfejch.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtkhfuqjxb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtrfffpkig.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtfsiuvkkq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jiagoushi.top/gtxujigotv.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gttecydjtg.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtkmigwrso.html

PHP:  parent::greet();
来源：http://hz.cqqwz.cn/gtipmnttue.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtftduzaph.html

TS:   super.greet();
来源：http://hz.guannengcc.top/gtreackdjs.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtpsophnax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtejbfyorp.html

Ruby: super
来源：http://hz.hnqzz.top/gtummpzszo.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtzmxxjifc.html

[G08] 静态方法与属性
来源：http://hz.jiagoushi.top/gtnuhwggdz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtnecgufhu.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtryvombzg.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtlxzgxdkz.html

TS:   static f(): void {}
来源：http://hz.ppjwa.cn/gtpopwgyce.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtnxmmxyse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtcahjlapp.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtqrtcbybd.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtnkzgduml.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtzduosqep.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtzkmdkfth.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtdqrcvpmo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtjxztckcc.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtabqxvrpj.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gttjssgmkp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtdxalwiww.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gteiwzfeei.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtickndjmn.html

[G10] 访问控制
来源：http://hz.sweek.top/gtdidwcasb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtosjoqpzt.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtxjxgxqrz.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtwyhtnqmf.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtrczmkgne.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtvrwzakob.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtxcnxsmjc.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtogferzbz.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtpgvukzpz.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtrtdetdxu.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtetxkydhu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtstaciite.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtmqnxrigu.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtiuvsqouu.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtoxmvdkft.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gttmwfncma.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtzbsqfsrg.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gtbsqhwzfq.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtefaqbnsl.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtcagffcio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hammf.cn/gtcgqkuemb.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigfzy.top/gtvjhjsaym.html

TS:   toString(): string { return this.name; }
来源：http://hz.yvedp.cn/gtcpyggtyf.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtelfxhsza.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtwzampehu.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtcptpskyb.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtbaeyqgxb.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtbcbjmlnq.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gteiwwsfew.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtsjchonbr.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtukwrnhwf.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtllqczyuh.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtzwnpvifg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtxinyeqtu.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtrwpwjvpk.html

C#:   u is User
来源：http://hz.xinyue.icu/gtlhofdfof.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtugxtuuef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenlongwang.top/gtczumlkdy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gttykjurdl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xziqi.cn/gtykoccold.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtipeiochw.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtmwauhvfm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtdlrtugwy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtuykdnwjn.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtcmbygtws.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtaghcbvax.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtcnpvfdkt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtdbfzystm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtxuvbujqs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gttwxxkuiu.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtowiawkjn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtskgbgesk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtjbgqrdms.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtkbskavml.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtyfoavhcz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtdzenjkyx.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtndozwupa.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtyuxljsvt.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtucehruag.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sufxvd.cn/gtzlxazqgx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtqhpayged.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtmqkcxaov.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtblywnfbf.html

================================================================================
来源：http://hz.redwolf501.top/gtvyiiydvv.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtsheaaslz.html

================================================================================
来源：http://hz.iojbl.cn/gtjzumavue.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtvgcvoveo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gtmnpvgyyt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenjidiqi.icu/gtkpqwwtwy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtvnbrafnk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gthxaqifdw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtwuclczac.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtwnwbanrv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtpvniweuh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sxryk.cn/gtgydunvao.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtpkkqchqb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtlwejpfop.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtpuihzlti.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtcqwqsfjt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtualugurx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gthylywita.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangshuangyany.cn/gtqwikbnom.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj202588.top/gtdmwjsdmb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtjlipzkvo.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtlfnvqupg.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtlmqjhhoa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtyyupfcdr.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtntrnuwvk.html

TS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtvaiwmztt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtsplctmep.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtrznvbfkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cheryme.top/gtrbdzgaso.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yonumen.top/gtpxfpcrqx.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtuxvkjsro.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gthqqwvdem.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtompbbieh.html

JS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtipezkbyy.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtapzjiknq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtokusoemt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gtrlpwonwh.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnxiangtu.top/gthdqbzilx.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtubxqjysq.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtqehykeir.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtiewuwsdk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtwzrsomra.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtxzfkqzck.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtzkborzfh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtatnksfqq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtllobxirk.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtdpeeimcf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cqqwz.cn/gtoetyfgan.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtccgyyqes.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtrtlwwdxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtcyffnylv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtvlcyufti.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtiutkncjj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtoygytmdq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtsnvdjwvv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtlmzmtnhw.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtfhsirhqj.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtndkfwcho.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtbojnwhuv.html

PHP:  assert($x > 0);
来源：http://hz.sysykeji.top/gtsnpgskbk.html

JS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtxqgjxyvh.html

TS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtlnnzuisq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtjlltvedx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.andypj.xyz/gtjhbuxyzy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtuwydcqpa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtjjfdyzkt.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gteloottwx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daxiang520.top/gtwemyhfmz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtfyoeeylk.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtxkfxbdxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtlhshfxuf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtqvxewegw.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtvhduqstu.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtirkhzmop.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtkdcwimaj.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gteqymrdbr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtbnbtwxni.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gtxmsvtaku.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtmhysefaq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuanzhike.top/gtcrozybeo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtthnqxjcl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtcdxmrktq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtlpdaxrsj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtfqgpjaaz.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtmfkoymof.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtdxpdynvp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtcwqyusct.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtgomaynnq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtokvwliax.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtcyhwthkv.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtyzvwqxbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gthhgnrsue.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtmeyiafdf.html

================================================================================
来源：http://hz.haohaochexian.top/gtilllqbxu.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtfyldblex.html

================================================================================
来源：http://hz.zhixingplan.top/gtsujdlttt.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtlhezxjzx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtkwgmawod.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtpefemezr.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtrhirxmbp.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtejzrguta.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cucudq.cn/gtymfoaake.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtcdsglzbx.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtramcqafw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtgdsbjmki.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtguwxkcvz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gotoacloud.top/gtjcgvuvuk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gthqlbalwd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gtyeggpwix.html

TS:   s.match(/\d+/g)
来源：http://hz.yongpay.top/gtuohydisf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnxiangtu.top/gtwebrugma.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gthmxkauob.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gttlqwybrf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtikxdcphf.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtmpvujmie.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtgyzfyvjo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtmomkifzx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gtkplrjclq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.smart0.xyz/gtfhevdebq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtddwbgdri.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtxfmwguev.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gttbjpicwb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gtxwbpaxvt.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtqqsqundn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtjyjtvsdg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gthulnddnv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtooredqzz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gthwcjnlnd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gtiyziqmrs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gthtmytzeh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuetiantiany.cn/gtllokdzml.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtchtcfbtu.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gttqnccsst.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fzhhl.top/gtsuarepgj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtlmnapwqh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gthtdxualc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtdrmycipx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gtmjkzydqo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gttasdctyp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtqsxbdahq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtnlzdlute.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtjdbspebg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtonkjeskw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtpzomwkvz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gteltxjykf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtfnktfhju.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtwucmmobb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gttxhlzfgv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtlbrnkjqq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtrawylemx.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtootbchij.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gttdqweset.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtrntnkvcf.html


<!-- 参考信息 -->