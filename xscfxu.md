代发 wailian999

================================================================================
来源：http://hz.ydzc1.top/gtqgvsffat.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtkiwfckfe.html

================================================================================
来源：http://hz.tanke756.top/gtnghcljan.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gtqlbdowpi.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtolzdoarb.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtrsyboobj.html

JS:   class User {}
来源：http://hz.meibo888.top/gtyuvdqffo.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtziyhbhbx.html

Java: class User {}
来源：http://hz.daxiang520.top/gtszhantvs.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtwkwyczts.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtxubxkfen.html

C#:   class User {}
来源：http://hz.wangshuangyany.cn/gtebiishgz.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtjrrazduk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgufenzy.top/gtnszbffga.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xingfuxueyuan.xyz/gtptqtfuwu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtyvghynfd.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtslasusav.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtjitbwocg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtulbbmzqr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtmubvbido.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtsgqianth.html

[G03] 实例属性
来源：http://hz.ivvv.top/gttwecscsv.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtnmofrsje.html

PHP:  public string $name = "x";
来源：http://hz.andypj.xyz/gtthlhasnr.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtmdlbhmhb.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtmzqzbwmw.html

Java: private String name;
来源：http://hz.gogol.net.cn/gtlwiosbeb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtanuusbwr.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtuavwfstt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtifoqhuio.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtylvzqbzm.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtzwzavyxw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtruahvcue.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtfwweikpa.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtksktrgrm.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtmmnwnxnz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtbkisyxoi.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtumpkubhj.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtggnyswjd.html

[G05] 继承
来源：http://hz.fengsongda.top/gtvdhrywns.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtnuyatbdf.html

PHP:  class Admin extends User {}
来源：http://hz.chenlongwang.top/gtqyjnktaq.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtnjzhyvlj.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtgjenixwn.html

Java: class Admin extends User {}
来源：http://hz.yongpay.top/gtgnheoxdz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtmwqnogxo.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gthllfkqql.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtnrruapat.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtyvdeyits.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gtjqwvzrjb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtocehsvnu.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtqrxqbpwd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtfqdpgotw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtvvkkxwnx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtywnkfxxj.html

Ruby: def greet; "admin"; end
来源：http://hz.xylfe.cn/gtmrcahege.html

C#:   public override string Greet() => "admin";
来源：http://hz.kuanghao11.cn/gtfdklojue.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtiudrrqyr.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtoclxcvel.html

PHP:  parent::greet();
来源：http://hz.zdqjudy.top/gtljpikgwy.html

JS:   super.greet();
来源：http://hz.dashuyun.cn/gtweqrzeyu.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtwyecizrx.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtjlpeerud.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yongpay.top/gtzbtzwhsi.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtnbkvtpua.html

C#:   base.Greet();
来源：http://hz.zhijiandao.cn/gtddxsylgy.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtwapzgivs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258.top/gtnxxyrpbw.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gtrcgcklft.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtchlgjeuw.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtgqqyogdc.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtmneulwuh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuanzx.com/gtjafmrvfn.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtaypwqjhw.html

C#:   public static void F() {}
来源：http://hz.ehwqpu.com/gtsgbtkjzk.html

[G09] 接口 / 抽象类
来源：http://hz.sxryk.cn/gtuhshnlex.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtmagzwjky.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gthrdktcak.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtlkdezhfo.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtdiacgfwk.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gttpbbkebr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtfoiepaxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangkeji.top/gtztdfwmnf.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gtlpqrbzby.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtcabiwyei.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtjtmylffh.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtmxtdsxbm.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtdjgyhhok.html

TS:   public / protected / private
来源：http://hz.aibaodan.cn/gtzvcjcwfg.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtxepauzba.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuanzhike.top/gtrqxcftza.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtqdghtgeu.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtrpcxtinz.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtshasmyuz.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtukhngtzg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtmfrjzctm.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtulfmtxjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtwdfzhnal.html

Java: public String getName() { return name; }
来源：http://hz.zhixingplan.top/gtqrauhuie.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gttgvaghmc.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gtrwdvnnfw.html

C#:   public string Name { get; set; }
来源：http://hz.nwbrower.top/gtqjueqbrl.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtzetnwequ.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtpzmizcew.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtdpnmrjsl.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gtwccttodz.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtjdyuqjsc.html

Java: @Override public String toString() { return name; }
来源：http://hz.smart0.xyz/gtethgzxks.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gttdgmxtoe.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtvpkmzkdd.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gtjcsgiech.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtcpjyhckc.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtyvlfubeh.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gttwoterqx.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtqiosqpki.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtunygzyvh.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtztehgcxp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.andypj.xyz/gtyspuippa.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigfzy.top/gtbuesazuh.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtweqneyoe.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtrafpapuf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtzxrppgqj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtxprncfjw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.iojbl.cn/gtxmghfmst.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtrrbgrrid.html

Java: record User(String name, int age) {}
来源：http://hz.zhoulong.xyz/gtbnkmikvq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtlvtoovcn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtzxkfzhah.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gtwuqvwiey.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtldfnkemd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtwdgflhdd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtnhtwjpch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtqmniagsy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtddzxeyyj.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtaovvsdie.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtnnwmmmgc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtisbgltcg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtkpgtvfwx.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtdnfndcef.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtckxpyhmq.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtquhjlvej.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtdmqifvnv.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtrpqsuznu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtsdnkccgn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtjbpkxiym.html

Ruby: obj.instance_variables
来源：http://hz.hnxiangtu.top/gtigqdayvc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtudistnwk.html

================================================================================
来源：http://hz.birdmap.top/gtdcbpstzm.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtfymeyxld.html

================================================================================
来源：http://hz.birdmap.top/gtqcgumfnq.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtffwgeccp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtbeznvrsb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtsnkglome.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtolzcxzop.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtgmnrpuvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtwcxziiul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtruzvavfo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gtyfpqmanp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtwkydqacr.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtezbwxldl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gtgrusivkl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtzecrafig.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtblbkwhbo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtyswpnxmh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtejzwfmsg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtxtzotyox.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gtbgodxadn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.52xcode.cn/gtcobvtrvz.html

[H03] 主动抛出异常
来源：http://hz.dashuyun.cn/gtkzhmzsck.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtktvsontq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtjohpuhec.html

JS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtaqgxssxl.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtlpnjfipd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtmurmhrcy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtaynjosng.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtimzgject.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtupsiohfw.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtxmtcydps.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtengbgdls.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtbkzxyxpn.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gteuoergwi.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtmjepyzey.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtolbbtijy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtlngpnwpp.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtrvbblxld.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtbzngbrad.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtwgbbhlly.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtireusscb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtrmghvzqz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtjnrkpdfm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtxwgcasxx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gteesreifs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtcnxzybij.html

Ruby: rescue ArgumentError => e
来源：http://hz.cqqwz.cn/gtujjyvuge.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtjzythbsf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtsvfqalbm.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtesptjmru.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtowdcusbt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtrmlxhaku.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtqnpfviqj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtjwxohyjd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gtqbxxacdb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.vqdsnc.cn/gtpsjohrup.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtrbffznry.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtkausravw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gtraakhzgf.html

PHP:  assert($x > 0);
来源：http://hz.wangshuangyany.cn/gtghanylqi.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gteothoftl.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtphospzqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtuifzcgje.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtrybwfxei.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtdhwgcosr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtvwwukaqv.html

[H08] 获取错误信息与堆栈
来源：http://hz.sufxvd.cn/gtigyjeike.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtvililezx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtkqpimstc.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtabodgfnu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtkpenghru.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtkupltkif.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtiyznecyr.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhijiandao.cn/gtswbucbtd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gaohongyu789.top/gtjusauewy.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtjqrxpshq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtrpgsdoar.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtpsvnoedm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtzvakxsav.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtlymvqtav.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtkqdughir.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zycfv.cn/gtjcwbndxq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtgntteidw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtirurdfls.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gthfnyhxel.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtmqkqkcuu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.iojbl.cn/gtpcfyhzqf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtikbltxdh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtvvctdyqb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtfyefoffe.html

Go:   defer f.Close()
来源：http://hz.nwbrower.top/gtaaofzboh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtonnehzjv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtybtfszva.html

================================================================================
来源：http://hz.hfpthk.cn/gthnaoulun.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtmlwitslm.html

================================================================================
来源：http://hz.wangdashe.top/gtzsckyigb.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtpgchgvvf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gttljyxjxh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.redwolf501.top/gtxxsrdhqb.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gthdzbdgic.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtvhfjgjrc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtkkgqneiv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtgqphqbju.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtrrijjoey.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gthvtxlbej.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtildrdilb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtgrnjftxu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtvpgvkbpu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fzhhl.top/gtuymsvcet.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gttoptelxo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtdlpapynt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gthfxwrxym.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtsnffrefl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtlvzlbjmi.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtodfgrdwo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gtbsvmcwni.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtqqkygjvv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtiwjcluhh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtqacfqlvl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gtwtrjexpa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gtwsedryic.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yanxiufei.cn/gtprrzrwfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtznemytgt.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtjafvhxul.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtwsaoeqlp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtoqmlemga.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gttwvnjfzo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtgefvljsx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtcpsekrbu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtmftnmihe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtwzvcfbhk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtbepesnzj.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtosihaesu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtaewjebke.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtdfuytumi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtcjnsqiue.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtsyqnwaqd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtjqhqfmvk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gttogpiykm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtkzxkdxis.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gotoacloud.top/gtidyzroos.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtivalwyte.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gtoxiucrdc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtoueqqxeh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtvgcwjxfu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtjtnlcqnf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258888.top/gtquuryyah.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtwlnlgkuc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gttudcnubr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtwpmsnsvw.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtjwdoowdz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gthbiqvghx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtbxkwlyjv.html


<!-- 参考信息 -->