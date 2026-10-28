代发 wailian999

Py:   class User: pass
来源：http://hz.jiagoushi.top/gthmxonhfa.html

PHP:  class User {}
来源：http://hz.jinghuilouyu.cn/gtencdihom.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtmpyxvbrv.html

TS:   class User { name: string = ""; }
来源：http://hz.zhiwuduotai.top/gtwezmxgdm.html

Java: class User {}
来源：http://hz.jinqigfzy.top/gtgawgpjgb.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gthrdzhdmp.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gthevcxilw.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtamuyysxu.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtntbawglb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shangyingyoupin.top/gtqpxkcpvy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtmjowlnwd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtsuazgmqw.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtxlqcyjsf.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtnmrasqfk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj202588.top/gtrvnimqvf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtcbfbzzlc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtmyrruepx.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gttiwwscqq.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtwbzoqmoo.html

PHP:  public string $name = "x";
来源：http://hz.gzhubu.top/gtwtwlxxax.html

JS:   this.name = "x";
来源：http://hz.jinqigfzy.top/gtvbmmiyqc.html

TS:   name: string = "x";
来源：http://hz.dianchejie.cn/gtgumsubbl.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtgplpfiru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhongyouzk.top/gtydshbfkw.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gthgsgsnqv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtvfnhkkuj.html

[G04] 定义方法
来源：http://hz.xingfuxueyuan.xyz/gtbgkvqmoe.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtgcetvmrw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtcrqcibui.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtcjpymvqr.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtkfeihdax.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtvvylnkzq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtgqifjebp.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtxmpiqtss.html

C#:   public string Greet() => Name;
来源：http://hz.zhengqikj.top/gtpbbuzyhj.html

[G05] 继承
来源：http://hz.bjfxy.top/gtwsytpduw.html

Py:   class Admin(User): pass
来源：http://hz.haohaochexian.top/gtgjyomtmj.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtwgvvtzbg.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtcxgpdugx.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtxqgtcqqw.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtoyxujmdp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtsetijgon.html

Ruby: class Admin < User; end
来源：http://hz.zhiwuduotai.top/gtfqjptlhw.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtuznwctdw.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtlimcvsxv.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtdkecgmlg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtgvmbgaax.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtrqiiapix.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtrtwdrlxt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtzzyahvml.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtgchjrghu.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtxbtgrawl.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtjaxvvvhr.html

[G07] 调用父类方法
来源：http://hz.zhongyouzk.top/gtqcaqshgq.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtbieubrch.html

PHP:  parent::greet();
来源：http://hz.52xcode.cn/gtspghctxt.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gthvccinfx.html

TS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtbcossmzo.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtxumgtgyh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtvxdvscvx.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtidegdkak.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtdkpxvrlg.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtlfqsfxnq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtzhbhfvrl.html

PHP:  public static function f() {}
来源：http://hz.nanxuanxn.top/gtmbzemwfs.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtmmbdflmv.html

TS:   static f(): void {}
来源：http://hz.guowangkeji.top/gtpnmuoeui.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtwndmxdtw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtsusodnok.html

Ruby: def self.f; end
来源：http://hz.hammf.cn/gtaiutgiza.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtqroryfrs.html

[G09] 接口 / 抽象类
来源：http://hz.jqgufenzy.top/gttqwkdvkk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtqtyoqaxq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhixingplan.top/gtbyxjcpey.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtpmkacrbb.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtadrwlall.html

Java: interface Shape { double area(); }
来源：http://hz.52xcode.cn/gthckdmqww.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtiovgiuhe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gtshbafxjj.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtlrfjfoai.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gthsoousyl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtadjcuavv.html

PHP:  public / protected / private
来源：http://hz.jinqigufen.top/gtxvqegeqq.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtahxdmirn.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtfpesbvsx.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtjcstekdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gtcyecgvwm.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtaugphoqk.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtsagfbgmx.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtmdbcgrch.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtpquqkhrb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtjdqzkvvn.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gthqmskmud.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtqctpicxj.html

Java: public String getName() { return name; }
来源：http://hz.daria6918.cn/gtowldbpny.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtyauzltzx.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtxamovnil.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtlthwedeu.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtifjzmndi.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtctfihwgv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtmnjybqqw.html

JS:   toString() { return this.name; }
来源：http://hz.yuxming.cn/gtzncdihsz.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtrfhzwznh.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtuepjstzf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtizvrtgkn.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtdttatkdj.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtmsytkhwg.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtbevbdlid.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtcibupfpo.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtcfuatxno.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtwepcbwxg.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtmcfvpzrr.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtmpydyyvw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtyehynehs.html

Ruby: u.is_a?(User)
来源：http://hz.316326.xyz/gtqncnsjyj.html

C#:   u is User
来源：http://hz.zhaomingkeji.xyz/gtpuesondc.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtlrgfugte.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtmbaysomk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtksnevrnp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtnjbwyeke.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gttkqetuue.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtnujxdgqy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtkyqfuljq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtjjtfkgvv.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtwkzicdkp.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtfqlvnpqm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtbgymruca.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgufenzy.top/gttesleicu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtuchybfgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtlaihgxun.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtrubgujin.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtlikrucuv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gthjwmqdix.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtwkwngpim.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtfhvngakt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtwbeotkbv.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtmxtfkozz.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtkmopiund.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtbvhmhmwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.snrcjt.cn/gtibdrqmom.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gttuplsjhw.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtolrhcsiw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtbgiecbrh.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwcfokjks.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtuiqpcyqt.html

================================================================================
来源：http://hz.havefunace.top/gtxaucixgo.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtrbknshyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gthxlwdwdy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtrwtogkba.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtiacggrvi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zdqjudy.top/gtahgwyncw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtxscpisgb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtfzxyiupt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtngafagfd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hywenlv.cn/gtxttjufhe.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtthhlrzdr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtiqindcvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtsshoxvaj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtqmsgahhi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtcalasrwo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtnadfbvqc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtszqgamub.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtulhpinnx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtpuqficqj.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtezbkpsbo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gtzjnrxjyd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtfzehpesm.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtpqpfmqwr.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtqwllunif.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtdqlwfjcr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtwmftxvzo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gtjcmlkxcb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtvjdmkpud.html

[H04] 自定义异常类型
来源：http://hz.aibaodan.cn/gtnursswjd.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtsexkxski.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jianghu66.top/gtwfiftijw.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtuqwepgwz.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gthvjunyra.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnqzz.top/gtqcrrztzu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuanzhike.top/gtiaivhpaf.html

Ruby: class MyError < StandardError; end
来源：http://hz.smart0.xyz/gtoxgfgbdh.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtwzmfdiyz.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtpxtcfkkm.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtlwjbdozr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtynaxxjls.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtthobrteb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtwkaasvyt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.snrcjt.cn/gtgtcnejon.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhaomingkeji.xyz/gtfosdzhsx.html

Ruby: rescue ArgumentError => e
来源：http://hz.shuidangran.top/gtmhshzmlq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtsoqpdfwc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtvxpybdnh.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gthvghtmql.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtpglwwzfl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtjderrdin.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtncgookzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtzxzzzpik.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fengsongda.top/gtpeoybkkb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtsgpdxivt.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtdhxwgvpu.html

[H07] 断言
来源：http://hz.tanke756.top/gtfdccuaxi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenzaomai.com/gtklzcohsz.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtnlrhtxqw.html

JS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtclhzhyct.html

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtmxkytwju.html

Java: assert x > 0 : "必须为正";
来源：http://hz.feifeiyinyue.top/gtpepxgngn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtdblpmnyv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gttqfrhuky.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dashuyun.cn/gtmympjoux.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtwmuovgmm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtepzdyesn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtjuniklmx.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtkruxakrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtsekpstnl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtcjvknwuv.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtuviicybj.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gtumaaterm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gtklgwepsf.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtxdnvydmc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtqocgjxmm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtpcnrhdhz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtlrkpsxbc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtfmwvmpiq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtperfycix.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gtamfawfiv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.meibo888.top/gtyizddzxb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gtgvtyirzr.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gturfueqve.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gttrfsrwny.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtltbsmdgr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtxncelrfw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtzmqabjoz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtuzojswwz.html

Go:   defer f.Close()
来源：http://hz.jqgfzy.top/gtqgfklphm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtsvznjmyr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gtoetwjdac.html

================================================================================
来源：http://hz.cdnleiting.top/gtastwksdo.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtfiutdlxq.html

================================================================================
来源：http://hz.cqqwz.cn/gtqrhwoivd.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtkdluhnri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtzliyrgqz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuetiantiany.cn/gtqtdjmuwc.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtznbezkes.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtsvapdrxf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sysykeji.top/gtnyzvevxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtpnnqdmhe.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtuwjewbwi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtfxwzrksz.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtfnhwmoxj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtjnagvkjs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtnxsyzmqr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtkcfqplny.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gtlnhykmtj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtccahfuoc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gttfmbdqgj.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtoohxlpym.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtnlsnwywe.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gtvjxhavan.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.mhx1999.top/gtmvlpmznb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cqqwz.cn/gtdlyswkuu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fengsongda.top/gtuukxeysw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtlzbpeuoz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtynctfhhi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ppjwa.cn/gtbwdgftfo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtwakdfoab.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtnzbwuvvv.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtipeiqccq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtzonvkrgj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtoyxqitlc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gthmzlmrry.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gthumbeqjl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtxsyghjpx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.smart0.xyz/gthlxbgkmk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gteevmjred.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtgbcooqwx.html

[I05] 按正则拆分
来源：http://hz.9152youxi.cn/gtxwbcfxgp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtqylpuqda.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtlwenkwrc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gthuimaxdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtpxgcjutq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtafkfqqzd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtsfdmrhpm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtlvwzmvqz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.c1oappe.top/gtjbjkmfby.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtagwzfajj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtvsocqvbp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtcsnnecax.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtcqydzihh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtqyithtvc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtgdcnrawo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pengpengdd.cyou/gtxpcanlmb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtnalapjhj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtigjhimsl.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhiwuduotai.top/gtrpekshsi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtajwrkvhp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtccgqygqz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dianchejie.cn/gtminpteyw.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtmtubophg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xziqi.cn/gtlftzfkbw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtdnolwxwh.html


<!-- 参考信息 -->