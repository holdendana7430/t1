代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhoulong.xyz/gtobwcxtjx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gthgadaoai.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gttmomnqjk.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtmmoohuzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtmylhilsy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtvdaeedcs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtcgqfbbpr.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtfkndqget.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pycfn.com/gtzeyaefgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtyeroyojz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtotnjnfyg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtvimrfpzl.html

================================================================================
来源：http://hz.shzxlz.cn/gtptvdharo.html

G. 面向对象
来源：http://hz.shuidangran.top/gtpzytxemu.html

================================================================================
来源：http://hz.yj20258888.top/gtwoyrycan.html

[G01] 定义类
来源：http://hz.svipenyu.cn/gtumsqelwj.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtdawcrtto.html

PHP:  class User {}
来源：http://hz.zhijiandao.cn/gtoacbcejn.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtojnroxxl.html

TS:   class User { name: string = ""; }
来源：http://hz.haohaochexian.top/gtgmuaxpgj.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtpidopbkf.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtwzbabkmz.html

Ruby: class User; end
来源：http://hz.zhaomingkeji.xyz/gtvmexfsaj.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gttottgidl.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtvynpcluj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pengpengdd.cyou/gtlqyrnjbc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtylepweyn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtrdtmgnwi.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtrcovrixv.html

Java: User(String name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtasdiafmu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daria6918.cn/gtzitcjppo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jianghu66.top/gtzztubukg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtbziyreqb.html

[G03] 实例属性
来源：http://hz.shanyushiyangkeji.top/gtxdbeuysf.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtauhkcszk.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtzubaoium.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtqnrpfesr.html

TS:   name: string = "x";
来源：http://hz.ydzc1.top/gtbnwmpxvg.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtnrgmppsf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtsvppbjue.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangtech.top/gthgqbonpk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtyqbtxpjf.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtgrojqxjx.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtsbqfrepc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtvzandqop.html

JS:   greet() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtlujpdrmf.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gterveqwjo.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtevgabtyn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtjmcxduac.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtsgieliub.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtlyzukirb.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtkytffplh.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtslkqqxfz.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gtmlzijhaj.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gthnssxgmo.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtmpgyrysa.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtpefnntja.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtvullughz.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtmtlwqsjz.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtzepyqeys.html

[G06] 重写方法
来源：http://hz.chenzaomai.com/gtappchnoz.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtxrxohjfp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtgrgadlnz.html

JS:   greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtabksymur.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtwphxmisd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtqnxsuppo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtrurtbgrt.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtzhndmmty.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxinkj.top/gtoildbgyg.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gtwvetdypx.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtwykhbcbs.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtsbbhmvkp.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtgoowvwva.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtykotzghm.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtqwsslica.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtvciqdlzi.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtmlkatrzn.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtagcxkwit.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtbpvavbvp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtkctwnqjl.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtnaebkbye.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtzwydvahz.html

TS:   static f(): void {}
来源：http://hz.nwbrower.top/gtsvlnnccb.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtqvsnqhhr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtswjfdepq.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtgwiilfpg.html

C#:   public static void F() {}
来源：http://hz.yonumen.top/gtyvdvyoqd.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtxhwdggqg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtgmwqlobw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtvcurcyyf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gttfddmocx.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtznvuwwrv.html

Java: interface Shape { double area(); }
来源：http://hz.zycfv.cn/gtuwhfculv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtponljnpe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtptkmxvmv.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnqzz.top/gtwekojvnd.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtmdagyacs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gtadrsjybe.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtuupmnsml.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtfqjqdnzo.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtdhmzecak.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtxtkvtlom.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gttnrohtiu.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtpjctsbmy.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtdkjmtcmk.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtiqczbjvd.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gttxwgyyee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtiusxgrlx.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtuynklizu.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtdvytvcom.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtdfmazfth.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtntpntkxr.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtfnpzavam.html

C#:   public string Name { get; set; }
来源：http://hz.guowangkeji.top/gtuhyejdgw.html

[G12] 对象转字符串
来源：http://hz.yuanzhike.top/gtiugkfjlt.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtfhvjiiff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtjyokykfs.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtkimaqfbx.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtxrgmnhst.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtwuzagnar.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtqvjkdiyc.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtvplowxpx.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtnqxehcvf.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtdbzdodrm.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gthuflewwf.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtrhjytfiw.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtvodkxliq.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtwhhhtrii.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtcjchkwtd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtpgfmpbmh.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gthzdcobye.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtszmvfrvk.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtqkopdnqp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtzzseujtk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtjupiybvg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtbeoynfme.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gtnpfamouz.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtfdaeigie.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtrarptdai.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuanzx.com/gtggybpnmo.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtcczkcphu.html

[G15] 枚举
来源：http://hz.yj20258.top/gtsdtnpjwt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ywan-chungtsiang.top/gtigqdylbe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.redwolf501.top/gtuviercgu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtdthudnzf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtangihiwt.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtgrcgwplu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtzxlacvor.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnqzz.top/gtjodqkkez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtkxbgdukw.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtpzmnmdhn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtxoeogtuk.html

PHP:  get_object_vars($obj);
来源：http://hz.yvedp.cn/gtwqrjqwyb.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtfjkhwgvm.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtjmjxjidn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtfnfdkqsl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daxiang520.top/gtdgiiwkef.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtrpdqwbrv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtsgctbgji.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdbsdbwio.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gtyqbdputc.html

================================================================================
来源：http://hz.9152youxi.cn/gtrtmapvxe.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gtcpnvfkwm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gttpgzadpr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtgrzwmrjr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtutmeswvw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gthqdmewci.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.vqdsnc.cn/gtkoybuqjp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gtyvwxcqpn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtwezdqenq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aibaodan.cn/gtdppznbyh.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtzafocsex.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtagtjqxvo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtkxsirdrt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtxlkjjvcm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtgovhomgx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtruhwezxa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtcneabypz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtlqjrxlss.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gzhubu.top/gtazunucfs.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gttwcjtppo.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtqxosbtlo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtucnforsr.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtsqswqihi.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtmhbmajmn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtlkqksqwv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtapddxojl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtujbbzasw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtwdvmgkaa.html

[H04] 自定义异常类型
来源：http://hz.dashuyun.cn/gtukhmhlgo.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtftipcdcz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtndyfpluz.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtfccvikqy.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtevcmvzdp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gtkldrbmlv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtspizbcmv.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtydoepmmu.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtzajehkdm.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gtsonbrqve.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtwljqvcxs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtmtnozmxm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gttocdpfnc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtpaygipuo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtxxwzvqqk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtrtrkmzta.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gtxafngfyz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtarguryny.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtypogfjat.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtjlzaebht.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtbzzllnkl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtfsehbefh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtbbvgsvwh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gtokdgfkep.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtwyifrfrp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtmknlczek.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtlvnrviql.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtthpcmevh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtrhcoijvb.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtrakedoyu.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtttbkhkje.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtainiptaz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtpburmgpe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gtobtetxjn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtdkhxgvju.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnxiangtu.top/gtffktouxs.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtwajftcgd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.meibo888.top/gtvmeqfyxs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtjwfcuuid.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtiapsuhrq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtygggjmib.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtojhpiont.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtlocltgrj.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gteukcyeam.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gthuytnckq.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtnlcakpfa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtfkdzifxn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtzosvrtoy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtyoqzpjll.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtvtqwpkhk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtkicvvode.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gtsfysgsac.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtatqyhoen.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtinbxhfab.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtttyhidbn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gtlnqlxvwi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtrvduyfoh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtoaqbqxti.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtefwmcaze.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtahvtnvzj.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtdvxxjndy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gtiitnnjez.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtaatghqjd.html

================================================================================
来源：http://hz.hysaishi.cn/gtezfvvtrp.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtjcdyhcnp.html

================================================================================
来源：http://hz.cucudq.cn/gtbvnsqoqg.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtbopbyehd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtrclihnsj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.kuanghao11.cn/gtzozugfcd.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtyreuauth.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtaysvgapm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtvpdxrzpp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtbwbtuzgx.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtltwwuoaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtfnzumrnq.html

[I02] 提取所有匹配
来源：http://hz.quarkkingdee.top/gtstvhvcbh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtltccubyf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnxiangtu.top/gtckthhbab.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtiuhzofxv.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtbavqgjtx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zycfv.cn/gtalbwekfx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gttexicpow.html

Ruby: s.scan(/\d+/)
来源：http://hz.kuanghao11.cn/gtdkjbxpir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhoulong.xyz/gttozdozcw.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtshvklzrm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gaohongyu789.top/gtghxribgk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtvctnhwmm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtxvlvylir.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtuldphxad.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.vqdsnc.cn/gtvwyphsrv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtghopiick.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gttukyihzu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dianchejie.cn/gtsklyrnyg.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtgjkqkfos.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gttkydycyy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtfqqkvfix.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtlkvyvutx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtigkvpgch.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtjzbfirtk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtmuluqhdw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sysykeji.top/gtiuwidels.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtlrbgzydx.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtzodsluwv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtpccrlqyw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydzc1.top/gtmbcbkvpc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtgjziahzj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtgmhrvrka.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtcltixcqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gteaynbiln.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtzhxscxgi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtleajaool.html


<!-- 参考信息 -->