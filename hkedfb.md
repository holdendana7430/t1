代发 wailian999

Py:   class User: pass
来源：http://hz.jyoumei.cn/gthrdjgafo.html

PHP:  class User {}
来源：http://hz.zhiwuduotai.top/gtdvzpizgu.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtkixoelpr.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtqdsqcgke.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtfsvyttrt.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtgajcdsuq.html

Ruby: class User; end
来源：http://hz.svipenyu.cn/gtvyptcxak.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gthoxjfebw.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gthohesqqa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtcviyjosv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtipgqvaof.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtbgdpzqss.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtlimyjwte.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtaxtnpuos.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtpovtgsro.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtfvzbndji.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gthmbqarcv.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtgkmimbzx.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtnkxphpeu.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtbjxtrgzd.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtyijdyjdr.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtchypuvhl.html

Java: private String name;
来源：http://hz.hnqzz.top/gtcqpebiyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ehwqpu.com/gtabkgegpv.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtjdzsdybq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtltxtupkz.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtuerzzvfz.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gttmyafbgh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yonumen.top/gthiozjpuq.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtnogdgljv.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtkrpajsoj.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtgpuhoivr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xziqi.cn/gtghortcrh.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtqcxjcnui.html

C#:   public string Greet() => Name;
来源：http://hz.hywenlv.cn/gttygdnftn.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gthmepedlh.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gttyqbsvsx.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtjdljrica.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtvmsggvxj.html

TS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtrhakwnnp.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtiloeqyah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtcpukswfi.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gtpjgpuhqs.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtjmfusjdt.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtmjsumzcj.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtcawjokur.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtrfttkyyq.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtvsdtnnax.html

TS:   greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtbvldvcbl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gthuuarxnk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtkolcjpfm.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtmusmojxu.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtmwoxsyon.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gttgcvfgjs.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtsnmfhkuw.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gtlgopegqu.html

JS:   super.greet();
来源：http://hz.ybcxt.top/gtdkoctewo.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtkmwhkhrm.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gtsqndfxmp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtxbagjwjj.html

Ruby: super
来源：http://hz.9152youxi.cn/gteorullub.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtycexfjfg.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtaqxbjazv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtmtiocgjk.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gticlioayj.html

JS:   static f() {}
来源：http://hz.fzhhl.top/gtvzinioty.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtjrhjwmwy.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtiydrjbce.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtmvmjhfpw.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtkgubvlvv.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtizfwmgas.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtrkzefixk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtwdktwdtm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtoqeciwfj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gthmiidlsk.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtvdlgzuai.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtnudjzeha.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yvedp.cn/gtfynvurao.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigfzy.top/gtbtswlmtw.html

C#:   interface IShape { double Area(); }
来源：http://hz.gzhubu.top/gtyynfwdho.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtfvjtrvid.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtdkdyvtgv.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtwdywiuwn.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtutehbqmc.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtcvvorwvg.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtvzafiiho.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtfsehhoke.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtnhletdfi.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtenmlcssd.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtezcqvlyj.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtsoawwczp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtharsxgyj.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtezocisdo.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtcrdzoigc.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtoovukaek.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtjtukakxy.html

Ruby: attr_accessor :name
来源：http://hz.tianlin.xyz/gtfccvvbyp.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gtpxcclfwb.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtelvztoif.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gticxvwgcz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtjpgdjdgr.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtadbywaas.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtfqexdivs.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtoommkynq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gtupjtrfhi.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtaehotixe.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtupbpivms.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtevdzvgqs.html

Py:   isinstance(u, User)
来源：http://hz.shuidangran.top/gtpnwfoskx.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtlrzoencd.html

JS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtndqfrcaj.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtukkuwqjo.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtblniqtks.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtmgtfnfsz.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gthcpiqdej.html

C#:   u is User
来源：http://hz.tanke756.top/gtqhahffmp.html

[G14] 数据类 / record
来源：http://hz.redwolf501.top/gtlexjotaw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtmlirbkhs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gtbzqhjily.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtyoarmvbo.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gteallfrii.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtqrfkmjna.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtpedgjynb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtkrtquegb.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtdlvqkxsj.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtwrsdcomd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtjtowmtii.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtabcomrse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhaomingkeji.xyz/gtjkhsemwx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtzpahzwds.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtjrcpysbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtfupbrsym.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtwguwcadv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtlficvjww.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtwpuhlgtu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtlsjjcbdu.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtairiupau.html

JS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtjdfbcxmt.html

TS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtpcnmqvrr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.havefunace.top/gtzmslkboy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtykgdwglp.html

Ruby: obj.instance_variables
来源：http://hz.hfpthk.cn/gtvfypytod.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guannengcc.top/gtmogwbjsg.html

================================================================================
来源：http://hz.nanxinkj.top/gtoarogjcy.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gttmkhsimh.html

================================================================================
来源：http://hz.xziqi.cn/gtkznjnmga.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtknlrteod.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.bjfxy.top/gtrtqygsit.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtjfurcyww.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtyxpelcjg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.redwolf501.top/gtvwynchof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtzzccadtk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtgahzqhwx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtvqqhcyht.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtrcenituc.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gtbczkbxkw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtfsdqzway.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gteytjdobn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtzaccgbsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtnfcvxbwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtxtgqbfzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtopcmckmi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtxyuwxmaz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtbtsbblli.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gtenybsfic.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtebbggwoz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gtkszglwym.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtxqlfndyv.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtsqmjwbxk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtctoccxti.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtyldvqohf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtsnycdwcc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtanohawbt.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtsfrelzrg.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gttcopkyno.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtpupnopgt.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtdyzacgsi.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtezfiwvki.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtgweqwocq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtuotjfohb.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtfsrdgavk.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtnlupslrx.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gthnszwonn.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtqwgzuqzo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtjukpifan.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtrerjewmt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtmakvjkmn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtspoqrgmv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtyqpvawup.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtonsoognp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cheryme.top/gtuogarvjo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtfmmdonpy.html

Py:   value = d.get("k") or default
来源：http://hz.yonumen.top/gtqodhuign.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtlukslhfp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtbysxnkwz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtiwzphfin.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtuafzjojw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtsnmortzb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtjlwasxyu.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtmbbsdinx.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtyvdbywfv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtkndcwuno.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtmfazvneb.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtlmtgocij.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtlkaxuuar.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtcaiarajw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtipjiqxzs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtgpvkvgvj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtafvchbcn.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtvzddkfvm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtudkflbxn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtmbpgqmov.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gtjfypfhnw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.smart0.xyz/gtavupjbav.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtteecbxwi.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtdbooneim.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtupdeynes.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zycfv.cn/gtayxxcdiz.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gttthbchtq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtaafmhuwx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtdbvgbpvz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangkeji.top/gtryvunqna.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinghuilouyu.cn/gtqyledija.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtnspvxurf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gtbegjwkhv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtxrusxqxa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pycfn.com/gtgqgoomog.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtbqofuzwg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtxwxmqhrc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtuhxnavvf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtxpaddpdk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtpaohjmdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtuhfmeboo.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtvofkrmpt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtkxausywp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtwfmucsiy.html

================================================================================
来源：http://hz.redwolf501.top/gtltwtfcmj.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtltolosfw.html

================================================================================
来源：http://hz.xinyue.icu/gtzvaymdkf.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtxuqhedrx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cqqwz.cn/gtnkrqyxmb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gthufmbvve.html

JS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtyhncsxbd.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtafhhcnli.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtgbvetjpn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gtdbufsxzz.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtoxzsikko.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtrttdzcld.html

[I02] 提取所有匹配
来源：http://hz.hnxiangtu.top/gtsqpzzpty.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gtkcyywgqj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gttqrrfieu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtrqvfszpi.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtwwirlwng.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtcttsramb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtidpbgbkn.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gteqgifneu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtsmklxfyl.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtxhgwwqrl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hysaishi.cn/gtjjeadjpm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cqqwz.cn/gtdhjpkttl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtaeachovc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtlkjywssg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtfojyptbp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtqyxludgh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtrmfzhktg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtpywawsoz.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtnjizbdod.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtmlgvfsvj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtryptpmld.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gttvarkvgo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtmmqfkozg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.birdmap.top/gtvnxhpouq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtehcwwkvv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtrfinqulv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtaikqjysi.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtdkpzbmym.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.svipenyu.cn/gtjvtikblj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtsknbwgep.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtrnjabkbi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gteiwjjihm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtlukbvcta.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gttqlbwmhi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gthpcbckiu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtlmugdblq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtcoviauak.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtfjwgekiq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gtiibspipm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gttnugpaif.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtaewhvrrr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtjxjneaij.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtfptewjte.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gtrfusbsgr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtznyrcjth.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtaklytnis.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtmtdppcys.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gthhupkudf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtcncguhnw.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtklhvlohi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtmsfubyjf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtfuysoktd.html


<!-- 参考信息 -->