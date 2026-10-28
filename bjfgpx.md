代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zycfv.cn/gtjsjvfplf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtatedehdn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtbckbsajz.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtlwihtopd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gtvcpkqzfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtktraedla.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zdqjudy.top/gtwxmmyhia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtzrkqfeid.html

================================================================================
来源：http://hz.iojbl.cn/gtwwadmqhz.html

G. 面向对象
来源：http://hz.yvedp.cn/gtmwkqvsob.html

================================================================================
来源：http://hz.ppjwa.cn/gtpymrcbtu.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtlspfijyp.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtigqlxgjv.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gtsyonjfjy.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtsntcklfd.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtkijgicud.html

Java: class User {}
来源：http://hz.jyoumei.cn/gthnkdfgdn.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtsirytbem.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtgyftpexl.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtljrfgtoh.html

[G02] 构造函数
来源：http://hz.zycfv.cn/gtoxwqrepy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtnodcjavi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtghqstobx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtlbbxxzmo.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtfjiffaau.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtfeleeptf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtzezkcfuo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gtzqolzsxb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtvqxeefku.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtjbrqvifd.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtmsmxemuq.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtgadfjpnf.html

JS:   this.name = "x";
来源：http://hz.52xcode.cn/gtlmosdssc.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtuqjhqndz.html

Java: private String name;
来源：http://hz.birdmap.top/gtkgndrbbn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtsqdevgcw.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gtaxhfcscv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gtmpigxwix.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtzxaerusm.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtdkzjyltn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtzlqcobbg.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtspfhcbxy.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtizdulsxn.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtpmvncjdo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtqluinnpg.html

Ruby: def greet; @name; end
来源：http://hz.ybcxt.top/gtwloecues.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gtxlcrxehw.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtgbpzejwr.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtmvptbvvs.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtyxdvzbcj.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gteudglans.html

TS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtyzfjfwoq.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtrdjalpwl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtxoqgdjmq.html

Ruby: class Admin < User; end
来源：http://hz.fzhhl.top/gtdjslfcvj.html

C#:   class Admin : User {}
来源：http://hz.shangyingyoupin.top/gtrhvnxhbb.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gtszpzdnqr.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtdzhndjpm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtnzrxqnhf.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtixkrizub.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtbvtbwjsv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtpxvwmooi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtigqwghaj.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtcdmqgyax.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtwundchgo.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtxiuxayzh.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtrsadyfyh.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gttxmgikhk.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtfdiiogpq.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtzagchjkz.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtvkdthaxd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gtpmtcegiz.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtrvsxctxy.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtdhqhtluf.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtbtmhloef.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtgcwgszrw.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtnotckekh.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtxrdkgvfr.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtcsjrason.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtdtcrzsfp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtnbcfixkj.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtplrispny.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gthbqsbkuf.html

[G09] 接口 / 抽象类
来源：http://hz.316326.xyz/gtogdbncgj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtutfqhlug.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtemebszle.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtebhywmev.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtkgfpfgwg.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtffuphiav.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtfquczgbl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtkrjionfz.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gteqvyoboj.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtwlgvyizd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtbxihjnrf.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gthkhqkejr.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtxeoffsom.html

TS:   public / protected / private
来源：http://hz.cucudq.cn/gthjhotrab.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtsxuhhuel.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtuguhdkpe.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtkwbnvqwj.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtbeoxhrad.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtnvpxdfyh.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gtntuvbldj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtfninbhpw.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gtzybgwyux.html

TS:   get name(): string { return this._name; }
来源：http://hz.feifeiyinyue.top/gtgpcweuoo.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtwqwxncvz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtmedewprm.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtfhfhstyy.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtbhmvxwro.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtkuujbcmj.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtkpqwoumk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtuhalurgq.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtkskjzfmo.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtujypkkll.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gtkyvucfoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtgvmzelyj.html

Ruby: def to_s; @name; end
来源：http://hz.fzhhl.top/gtsoawzuzx.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtdjslsawe.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtryiavdga.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtsnwbvbnf.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtabappqfn.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtnvcvlthh.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtfiodduyc.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtbolzbemq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtbkokkdza.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gttdsbvmih.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtuxptbaap.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtrsthzuix.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtjzymdfhd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtqcvgewct.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hfpthk.cn/gtncapzqbp.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtlwvkpqim.html

Java: record User(String name, int age) {}
来源：http://hz.ppjwa.cn/gtfrmjurws.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtmchlryve.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gtzxoyrrhy.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtrfjesrza.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtyzrndhgo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtoovxkqza.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yueranfly.top/gtexdoisiy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtlrgmkkaa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtfcoxsqai.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtzdzljrkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtbxeumlqr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gttdkevlpx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtctozmnxw.html

[G16] 对象转数组 / 字典
来源：http://hz.daria6918.cn/gtwtskobvk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtncxlnjyh.html

PHP:  get_object_vars($obj);
来源：http://hz.yvedp.cn/gtajzijutc.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtkbjavxee.html

TS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gttgtjkjer.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtkoyqctda.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtfpuiqcic.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gttdexuxzi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtpbsfqded.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmwxlydyo.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtzgkydrim.html

================================================================================
来源：http://hz.sysykeji.top/gttnfxqnam.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtuhenqjsy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtwqemtzsi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangdashe.top/gtpsmlwlhn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gttrrmifyx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtdkhamivn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtobisumfh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtpbhukaun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtheamvgyv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtdscpitef.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gtnejpgval.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gtykmrfklc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtnidopdsm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtudnszoev.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtxisugrmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtqntfhmas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtjxyisoqj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtvhuakuys.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtstybfqot.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gttobhvftf.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtnadhrlgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtxkqdhtgt.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtyuhkgeiq.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtfylgvlmn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtbvekrnac.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gteqmzhbob.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtkohwakcv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtypgxmlyx.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gtgpckbaqb.html

Py:   class MyError(Exception): pass
来源：http://hz.ehwqpu.com/gttikzicqt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtvgexyzvk.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtobbovfec.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtellsknrv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtrjqslnmm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtdvldkmml.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtggiboetc.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtgxcjkovc.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtupxozbpu.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gturvgeaeh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yangfankeji.com/gtgfsizfps.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtqajhsdzy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtcozzziff.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtiadplshn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtkmncmatz.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtuejeeoip.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.redwolf501.top/gtwphabuzw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuanzhike.top/gtqntdfmdt.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtqeqvpqyz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtcdobqcsq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtmyddgcvg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtohpyupds.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenjidiqi.icu/gtfyzqqccd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ybcxt.top/gtlpseittv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtchfsjxax.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gtcrxxnumk.html

[H07] 断言
来源：http://hz.yj20258888.top/gtsdfdttif.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtbxzbveoo.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtcxgralef.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtuzotrqhi.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtgknemdnc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtmyxrvvpp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtgxewtwak.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtwmkoahkd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtsmhrazdz.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtrcmgsrtu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtqexovwmv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gttwmxfaut.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtgzbashmv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtikeslndg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtpqlfkrkm.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtdquhfvve.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenzaomai.com/gtnuiuzpio.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtnhvkhchy.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtryvbtqyr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtvxuawdni.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtyscilnyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gteoosclku.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtkncupwol.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gtxrsczbhm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtbeznywog.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtoqqntnym.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tianlin.xyz/gtfdhsfazo.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtycunsvby.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtdvernfwf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sxryk.cn/gtjumswioy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtcfyawzmf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtfjbbpdnv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtggtisvef.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtjfeovwfw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtrmtwqirg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtbjxnavvp.html

================================================================================
来源：http://hz.haohaochexian.top/gthlthzmmv.html

I. 正则表达式
来源：http://hz.hysaishi.cn/gtggwsepky.html

================================================================================
来源：http://hz.yongpay.top/gtehjkxzzx.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtzsadkfvp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtkkgtctch.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtoekeojov.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtokwjdydd.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtqqxauoqz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtgpzdgvbb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtprdfkjmp.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtblysyopt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtvmxxwxvr.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtlvvgitja.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258.top/gtpcxtdylf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtsoaaqpdh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtvxegdspw.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtzzdhbjrq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtbrqrlekq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtaakmifxi.html

Ruby: s.scan(/\d+/)
来源：http://hz.meibo888.top/gtfinowstt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtohmlyyzy.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtsuieanyx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtduhsoeth.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtmdbpuevd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtrdigpbrq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtelyfnfen.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtayjdgffg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.iojbl.cn/gtagttlqdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtuldwwsrp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtvqvtcbho.html

[I04] 正则替换
来源：http://hz.pycfn.com/gtdrehchgk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuetiantiany.cn/gtfautxncl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtlebjghke.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtlsbxrdsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtqbouwtxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yanxiufei.cn/gtenbhdyof.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gotoacloud.top/gttzirciqa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258888.top/gtqouyqwff.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtdzhdlxrt.html

[I05] 按正则拆分
来源：http://hz.c1oappe.top/gtlcistmmp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sweek.top/gtcbmuwpoi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtnyyesyls.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtuipsbqzx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtjckhqbtp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtpwevmrlo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gttiiuujpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtroatgzks.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtqycopsjl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtfpsvylkr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtpgvyupnu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtvlgfsapf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtyfvexggb.html


<!-- 参考信息 -->