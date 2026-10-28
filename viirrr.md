代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gtlyphdsst.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuanzx.com/gtmwytssjm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtcketpiwv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtqskmmeiv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aibaodan.cn/gtfcbpkmii.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gttrvsucib.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtdvragspg.html

PHP:  public string $name = "x";
来源：http://hz.ehwqpu.com/gtgutgnsjr.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gthtwqfvvk.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtbxpzfxak.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtjqvdapdq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gthqupovdt.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtkutytfyh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtjbhipsdn.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtbagwnhyx.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigufen.top/gtfsglxovh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtranoleep.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtjvrodkrq.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtbgnexvok.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtvuhfcopq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuanzhike.top/gtihewheky.html

Ruby: def greet; @name; end
来源：http://hz.hnqzz.top/gtuvhutpvk.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtwqsohofz.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtmqlnaqfn.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtplbyddqj.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gttclkfzqb.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtlhpmecrf.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtivgdrdbz.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtqjriflxq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtlwbggfjv.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gtfgmgnrms.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtnvmtvxyl.html

[G06] 重写方法
来源：http://hz.kuanghao11.cn/gtkglxdihf.html

Py:   def greet(self): return "admin"
来源：http://hz.ydjk.org.cn/gtukkgcerg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtwtygigne.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtljkzmkct.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtjxbcjuoa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtadokjfco.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtwnpkexya.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtpnmlbavh.html

C#:   public override string Greet() => "admin";
来源：http://hz.yanxiufei.cn/gtmxfwuuew.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtcqhjekta.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtebhqiwsj.html

PHP:  parent::greet();
来源：http://hz.52xcode.cn/gtusdndccx.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gtgviedzwr.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gthimmubcx.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtsgbkmzoc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gtxdcitkew.html

Ruby: super
来源：http://hz.tanke756.top/gthpkloqqf.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtchjzgcya.html

[G08] 静态方法与属性
来源：http://hz.guannengcc.top/gtaqcdnzeb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtjbzdihsq.html

PHP:  public static function f() {}
来源：http://hz.ywan-chungtsiang.top/gtaovvaxjl.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtnzxvgzyn.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtpxfgujts.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtxezpuknr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gthqgwkxjr.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtkgkafspu.html

C#:   public static void F() {}
来源：http://hz.zhoulong.xyz/gtpxwrnfbl.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigufen.top/gtaeksyktv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtvozbeypx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gtolgmheub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtovazekiy.html

TS:   interface Shape { area(): number; }
来源：http://hz.mhx1999.top/gtnmixcbit.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtthehjuns.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gthiskjepn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtzeayarlc.html

C#:   interface IShape { double Area(); }
来源：http://hz.gogol.net.cn/gtneelsjfz.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtmflmpajw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtmwjrydmd.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtqyarwfud.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtkdgbfwha.html

TS:   public / protected / private
来源：http://hz.redwolf501.top/gtedxnerxn.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtinhdaikv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dianchejie.cn/gtduqvsyac.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtfzfmuiko.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtzhrdkpfz.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtrpanjuvw.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtixqlfhsd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtaicamyjw.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtdyqfxlpy.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtpimvwqct.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtqxtjelrt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtfqdojbyf.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtwtdivicy.html

C#:   public string Name { get; set; }
来源：http://hz.ydjk.org.cn/gtlvtbgqdk.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtwxsaxefm.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gthuphwvhh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtxqgxuguw.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtyweoaety.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtukjfllll.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtrkkxvaqn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtbafjnbfk.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtyxoohxgo.html

C#:   public override string ToString() => Name;
来源：http://hz.jiagoushi.top/gtzyyfhfxb.html

[G13] 判断对象类型
来源：http://hz.xuanzx.com/gtrwvivcjj.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtsamzgdps.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtxtjppopv.html

JS:   u instanceof User
来源：http://hz.aibaodan.cn/gtxcpkrcuo.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gtuivtykpi.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtlbikteyk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtsobfxdcb.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtbjosirlm.html

C#:   u is User
来源：http://hz.yuxming.cn/gtmleuavvr.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtjoedrlyv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gteqnznhzb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtnsdrveln.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gteroopame.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtsbdjxtjk.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtyyvxrweb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gtrgwkvdvb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gteizxoeww.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gttydbtkjk.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtqyxqziqa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtkqwbstjf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtuoqsnimx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigfzy.top/gtajjozzhe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtspwpogpl.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtuucqtvgr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtccwapvis.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gzhubu.top/gtuqifeeij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtdwosifuz.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtprvwgybp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pengpengdd.cyou/gttemxuvfu.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtmaqlaoja.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtdcckxgyf.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtsisgzxuz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtlmegwhjn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtpewnjpkw.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtoiwaoleo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gtegufxobo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtahptsvih.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtxdwyfwnc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxlbfbkjo.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gtobtwfwwv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtmsukfept.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtsgekrrue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtrbwzzxtu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtidwltafs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtdbtzkprg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtanmbqktq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtavseqzkx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtcnszdvkt.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtjjfqmhxp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gotoacloud.top/gtrxszxeaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtmkbjzqhg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtvwbaxpyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtwksembwz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtqdwooysj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtjldvkdxh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yongpay.top/gtdvyinmjx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtnqnkkvhm.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtnygwsuhl.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gtkqummxyc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtclwqydyd.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtkoxpkujx.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtjdgiybal.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtbmfjiujr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtggkboqgl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtibkgbzia.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtsottrodr.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtkensxyzt.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtciuiugpo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtcnotnjeu.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtjopuyrgb.html

TS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtpcevbvos.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daxiang520.top/gtofgcqbli.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yangfankeji.com/gtdtpqlrbq.html

Ruby: class MyError < StandardError; end
来源：http://hz.redwolf501.top/gtglarrxjr.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtsmhfqkwo.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtbxwtxbjb.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtlxbwxrkv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtqopoqkcx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gturyykwnm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtntjyjttv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtfhgbabtr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtoosfduhk.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtywvagwdl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtrztekrzv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gtxzpygcwm.html

Py:   value = d.get("k") or default
来源：http://hz.snrcjt.cn/gthcgrbnnw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtbslofbzp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtayfoyqqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtmfikwqkq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtgsnlxnxm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtdtwniyja.html

Ruby: d&.dig(:a, :b)
来源：http://hz.haohaochexian.top/gtpwngdjhw.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhaomingkeji.xyz/gtgmvhhplb.html

[H07] 断言
来源：http://hz.smart0.xyz/gtotldnlcm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtmzbfvspz.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gtdummndmr.html

JS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtyxzndcux.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtlhlqytor.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtynyyxemo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtxeuunytx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtzyhblqel.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtbkselvmg.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtvlggpooy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtlsfrqflx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhongyouzk.top/gtpppsccob.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gttlzyuono.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtuzmmamyb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gteofcqjzv.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtejseyhpb.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtxnznltoo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtdyrysbko.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtvdyhxjrc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtqpoxoaqo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xylfe.cn/gtbhxgvqua.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtoryhikea.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtmwpzppfy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtugbkmtkf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtxbszuesy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtwrrxetpu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtadhpvdnr.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtnvyvmhyf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtcnaoeagk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hfpthk.cn/gtahguzbtg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gttwinadyl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtftdzhyyo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gtghtvogry.html

Go:   defer f.Close()
来源：http://hz.0kj1m.cn/gtmtjijldc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtwatwnewx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtzyeibzxf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmldtdmvm.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtxainisiq.html

================================================================================
来源：http://hz.hywenlv.cn/gteqpbwlab.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtqlozzuoa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtgopbrvqn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gtrjrvohrs.html

JS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtynvadieu.html

TS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtokxhwvnr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gzhubu.top/gtawvntonc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtzfqsttkn.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtvvguyhvn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gotoacloud.top/gtmwyehxyn.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtthpwnutu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtbycfianh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtwuxcullj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtygqbrrdp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtngyuguzx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gteijxxasr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtmgwqvqqo.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtdkidjabb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtjeohsyaz.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtgkiegkdi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtskathbec.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jiagoushi.top/gttfvvwzlg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtlujxuugd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtznzeiwsc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.svipenyu.cn/gtygboqjmk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtflcixigh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gtaeknsklr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jianghu66.top/gtxhboqucg.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtjtbteikh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtnxbamwjy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtvyaglwnu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtubozpbvq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gthiixqidm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtolcygwqa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jlsjyb.cn/gtbdntaovz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dashuyun.cn/gtwxvmoeqn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtaenjptbm.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtlyfeqivp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gtljpuuloz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.snrcjt.cn/gtetpfylui.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtffulodcu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtpgwfweya.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtzvnbtseu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtmfdjasrf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtfdwparqf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtkqdumvcj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtmwszchtj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtmqkibhyb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtvpacrzzy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtdtgqdtrs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtlxjkmbzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtaxhfguom.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtklptmgal.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sweek.top/gtglvmkbth.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtjrqngimg.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtqnxalryd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gtqtrcknmi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtaqicvnbc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtqfxyqyrx.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtxdhucldw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gttjdzivir.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtolctdisa.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtxqblsnnj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtxkdjesel.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtpoklgpjg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtlhfyafnr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtbzqqccjp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gticrovtmu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtclvbjvoc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtmnyeohro.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtypeenuzg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtqzmjuznf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtjfdduyxe.html

================================================================================
来源：http://hz.jianghu66.top/gtumcumkek.html


<!-- 参考信息 -->