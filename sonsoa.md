代发 wailian999

Java: class User {}
来源：http://hz.0kj1m.cn/gtzcogaiky.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtpykhqgar.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtxwsxrznj.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtrsrqkxrw.html

[G02] 构造函数
来源：http://hz.haohaochexian.top/gtadgvgocy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gthfkniome.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtwbrbkcaq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gthuzliyyn.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtnmsvyoxw.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtgxpakqmv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtkoualswy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtdxxkxnth.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gttmyebiop.html

[G03] 实例属性
来源：http://hz.yanxiufei.cn/gtcvyayswn.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtxzfgmocl.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtnadgjswi.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtddlctxcz.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtkjjxaure.html

Java: private String name;
来源：http://hz.ppjwa.cn/gtmngdudbm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtchtrhefm.html

Ruby: @name = "x"
来源：http://hz.pengpengdd.cyou/gtwxfralvp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtoanuopdr.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtfxhggslc.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtydaqocuj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtstawxtqg.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtzhcvtqru.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gteqdgdfzy.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtdnnpryee.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gttvmslmtp.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gttcdapqch.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtinylleok.html

[G05] 继承
来源：http://hz.cashguo.top/gtaohtjixf.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtbxgfjhro.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtmbozmmka.html

JS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtgftuajmj.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtjwindrqj.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtgkgetllr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtjkddqwut.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtthkpiklo.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtddkanrxl.html

[G06] 重写方法
来源：http://hz.pycfn.com/gtvzvsnihb.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtgjjpvaqt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtzzxvljkb.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtcdymktgb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtdrueyazq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtxguwobdj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtiqzzvmiv.html

Ruby: def greet; "admin"; end
来源：http://hz.andypj.xyz/gtzrndzcgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtzubfyoqc.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtxajiawpu.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gtcyviugzh.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtoypnmwio.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtppqvoqxd.html

TS:   super.greet();
来源：http://hz.c1oappe.top/gtbxdhjdtv.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtausxnsuf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtqeihtzzp.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gtlwmcmejh.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtnpdlziip.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtmbhmtwyn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gteclngisq.html

PHP:  public static function f() {}
来源：http://hz.wangdashe.top/gtcnkpacsy.html

JS:   static f() {}
来源：http://hz.sweek.top/gtbkbzewet.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtqmwifbde.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtiscngewg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenzaomai.com/gtcdnpbzoc.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gticrqulol.html

C#:   public static void F() {}
来源：http://hz.yvedp.cn/gtbhllthdn.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtpyzzukbu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.quarkkingdee.top/gtdvftucjw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtcknxdcod.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtnmpeqnlc.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtwchwfbdd.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtrhfkoseb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gthjfrzmnq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtkpnsvfrt.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtlfkirmdz.html

[G10] 访问控制
来源：http://hz.feifeiyinyue.top/gtmteyvpkh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtjlyhfwsn.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gthyhpgnrz.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtgkjzinbp.html

TS:   public / protected / private
来源：http://hz.9152youxi.cn/gthaavdwhd.html

Java: public / protected / private / 默认包级
来源：http://hz.hammf.cn/gtnbanpkor.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtasrqishy.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gteebssxne.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gthblmffjn.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtedcqfvik.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtwgqgtcws.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gttjblfaag.html

JS:   get name() { return this._name; }
来源：http://hz.havefunace.top/gtlvjrsspy.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtikelsqvu.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gttynpling.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gthfooaoeo.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtmutcdseq.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gthaqugyko.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtaoejyfjr.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtcznroeuf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtvrlsvkgp.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtgqswjxbi.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtkdtdqaub.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtsytcolqq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtejdbsvsh.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtjkitwgqd.html

C#:   public override string ToString() => Name;
来源：http://hz.cucudq.cn/gtfwyozywo.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtwufcwhry.html

Py:   isinstance(u, User)
来源：http://hz.chenlongwang.top/gtsagfopwm.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtsndmjdfd.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtkidnvcxq.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gtnyqaygmm.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtgejumedo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtwdvpgnrk.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtebdpqpdx.html

C#:   u is User
来源：http://hz.tian-w.cn/gtzxxhqmdv.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtabospjbk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtzwrnzgnu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gthkffncrl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtsebvjjsd.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtovtjnfhm.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gttmixzwlo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pycfn.com/gtfqgzjqnr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nwbrower.top/gtfpgszjmn.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtiendfbti.html

[G15] 枚举
来源：http://hz.nanxuanxn.top/gtwhjcrxmi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gteodzdzrf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangdashe.top/gtmofcshnf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gtxoxgjpnn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtjtxkphxg.html

Java: enum Color { RED, GREEN }
来源：http://hz.vqdsnc.cn/gtndcxnbry.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtkggbdeqc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gttuvfwhvl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtwbkvxdll.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtnmiylcon.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtpgnocafs.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtzbhrpsvw.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtbcqtnpac.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtynaucwez.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtgzfcfhhj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtbffvjfrj.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gttmlnkvvj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtfuwxqryc.html

================================================================================
来源：http://hz.yj20258.top/gtmweyarhd.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtwghikxub.html

================================================================================
来源：http://hz.shuidangran.top/gtwmambrur.html

[H01] try / catch 基础
来源：http://hz.zhengqikj.top/gtctcjkzaj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtrxmuwbai.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtmlucgwnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gthvvwceoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtudrbrhns.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xinyue.icu/gtouagemac.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gtbokllept.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtjkqnyuyr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtgvhpvtqa.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtzmblgdac.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258888.top/gtuncbtucf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtlediysgf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtikbqiemv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtrqxbwlfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtsvruokez.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guowangkeji.top/gtscufrftu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtdhchusad.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gthdmfwwpy.html

[H03] 主动抛出异常
来源：http://hz.fengsongda.top/gtyjjaiprb.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gthbtkqnvy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtdwrtzkba.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtqdodqfra.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtsujhgjqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtnutklhuh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gthweptwtp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gthsirnrdy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtkmkcnpul.html

[H04] 自定义异常类型
来源：http://hz.9152youxi.cn/gtuprznhvy.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gteijhpbnd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtnmkhkukg.html

JS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtnfwuwuwm.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtmladmpmw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtuzmjvrod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtdcxdejbb.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtkuzcoknp.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtqijrijwd.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtiovxwbqk.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gttdpgvbda.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.iojbl.cn/gtoqyyaaxc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtwkpzhhom.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtoqrlijwz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtmrktnhii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.0kj1m.cn/gtxylgihem.html

Ruby: rescue ArgumentError => e
来源：http://hz.shangyingyoupin.top/gtskecebga.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtbtqjjfek.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtytcsyxhv.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtmtyiddaf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtmxwjzzsg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gttbsbyire.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtiwprrtci.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gttfbxlyqo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtdsncvfip.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtzarvzxda.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtsyesgwra.html

[H07] 断言
来源：http://hz.gaohongyu789.top/gthytypyau.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtzecmhopw.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtsbmpejvp.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtbbcvtpmw.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtnejbjtdr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtxubjtqjb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hywenlv.cn/gtdvmpzvtf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtxsqsidbi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gtpdrpjfbl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtdgzudnuq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtphrhdnkm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.havefunace.top/gtfvecqmpc.html

JS:   e.message;  e.stack
来源：http://hz.cucudq.cn/gtwdoguoqf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtwhiizgug.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gtjtekdeyr.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtivirumwy.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtfjxoejrs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtdnvqbqip.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtprhtrhaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtzxvomimu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtiyenhhvq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gthrflsqya.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtiolzxxlk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtlqomfxnb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gttmcflngi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtyqgivena.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtkretryiy.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtjqrwlneo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtwsxasnry.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtzmeioosb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtauvalnyn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtffthwzgl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gtmtwqtmqp.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtinwvmszz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtdgoewkqn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtlanjonsk.html

================================================================================
来源：http://hz.yangfankeji.com/gtjaxhpdpq.html

I. 正则表达式
来源：http://hz.316326.xyz/gtyieiwzwn.html

================================================================================
来源：http://hz.guowangkeji.top/gtqadkcfeo.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtyymtlurj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtwpjdgerc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtofdrlbol.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtapidynpr.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtfqaxmhwr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gtmstvboum.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtfvipepjo.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtjgtrfwyo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtoukghxcx.html

[I02] 提取所有匹配
来源：http://hz.sweek.top/gtrcqzajan.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtihdfbpdu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtsgchtrdc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gtgijtstpn.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtdbhtwogb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtlwklfuav.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydjk.org.cn/gtiejevisd.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtuvgrjtfi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtctqsatdg.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtflhukgew.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtboudhrqx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtyedjlslq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtosmpbllr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtdlpfspus.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtjrhkgeyy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gaohongyu789.top/gterullfwx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtnhctbtmy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtzdwrfekt.html

[I04] 正则替换
来源：http://hz.svipenyu.cn/gtaorfhsat.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtzwgwzxfq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtkqxtiftg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtnesktfjr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtusfsimaj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtjyubynzc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtuvqrtutc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gthdmsrwsa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtrospcwdi.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtzjgkbpwz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtkedczmav.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtpnbvwdlt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtihtlswcb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtxtauidhn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtiviuaokm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtkwzczvwi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtrcvtxdhd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtgbbhqubt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtbaztlkky.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtbnweiwgm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gthijplilw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtnawiuxyp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtcofeyxyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtsechhcch.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtzpgfkkii.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtvosxdqcm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtbbuhrovk.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtwrixkkxm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtuudrjvns.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gtvenqfqsu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtzliwtvyc.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtetnewndy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gtdgyejjmr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtkrtoidvt.html

Ruby: s.scan(/error/i)
来源：http://hz.yongpay.top/gtuxfjbrra.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gteidteozh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtqwjcoilz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gtxhljhwjz.html


<!-- 参考信息 -->