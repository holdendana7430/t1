代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigufen.top/gtkaxzrwgc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtgybhbqny.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gtfznemajt.html

TS:   // 同上
来源：http://hz.yongpay.top/gtfwwxrjvk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtonxxrupr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtgdhxobki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hongshengwenyu.top/gthvnszksw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dashuyun.cn/gtpyyycdit.html

================================================================================
来源：http://hz.jlsjyb.cn/gtddmwoqnj.html

G. 面向对象
来源：http://hz.sxryk.cn/gtkivgeksx.html

================================================================================
来源：http://hz.aizwys.cn/gtlknyuove.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtbbjzruyq.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtdehburvh.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtoclkmqzy.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtrjmtrqlg.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtvbdmssft.html

Java: class User {}
来源：http://hz.nanxinkj.top/gtjxlccyyq.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtdypykxwv.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtqsikrbsa.html

C#:   class User {}
来源：http://hz.ybcxt.top/gttvwndtbw.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtlbcuhvmg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtduoduyse.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtfgojhbri.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtxpiwfjnn.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtalyfulgk.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtiwnqecmo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtillmjzpk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtrmalmlat.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtkgtuiosd.html

[G03] 实例属性
来源：http://hz.yongpay.top/gttxnqmawb.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtuzhgwesa.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtizdufvga.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtkirnmtjg.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gtkokkwgvx.html

Java: private String name;
来源：http://hz.jiagoushi.top/gtkjfyikts.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gtjvwipgtq.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtlgoqxloj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gotoacloud.top/gtnfjxhyni.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtxrgfkgut.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtgrvbymhh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtyxizhopv.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtlrsmclgk.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtvljnkutm.html

Java: String greet() { return name; }
来源：http://hz.kuanghao11.cn/gtutbeqrrf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gttvnluisi.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtmxdnwybx.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtxysqafgs.html

[G05] 继承
来源：http://hz.xziqi.cn/gtlgvotsrc.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtoqlooywe.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtadfawtzh.html

JS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtrqkmodym.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtimaryuaw.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtmlhnknbb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gtvpurczqh.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtmlaptabu.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtlcmkwlor.html

[G06] 重写方法
来源：http://hz.yuxming.cn/gtfhsocplm.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtjeatnwsf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gthhmvngrq.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtengahaxj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtcivwemxu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtxirvfuvt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gogol.net.cn/gthypeihnj.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtdxrrwckj.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtsfiyerbo.html

[G07] 调用父类方法
来源：http://hz.sweek.top/gtguvtktvs.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtlctpvzto.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gttwrmgobs.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtvnzqgeql.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtpjxvgazq.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtjvscqung.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtmwlgjttz.html

Ruby: super
来源：http://hz.xinyue.icu/gtexcbigej.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtiklbfdck.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtaerwprnv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gtvrgyibsl.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gttznjtyfc.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtozbeuhnf.html

TS:   static f(): void {}
来源：http://hz.tianlin.xyz/gtuvstbiab.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtlyzswypg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtsozvyyww.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gtgcgxjydt.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtxdjgvtmj.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtyzmmmciq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtaaglrdpw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtcoeqqffr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtmvdbguxa.html

TS:   interface Shape { area(): number; }
来源：http://hz.andypj.xyz/gtjzexbcla.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtqkouoxlh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtlophmbjh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtcbtbuzpz.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtqagewpnq.html

[G10] 访问控制
来源：http://hz.shangyingyoupin.top/gtswwaachm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtlxcwbrhu.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtmfgovfaf.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtyydtypuq.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gtjwylmyeg.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gttiotsiwz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtrxosuiwc.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtikligqgb.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtjsqtestw.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtjmgrlavc.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtquzhvpcb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtlymlzahs.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtsbcnqnsm.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtpzkvulon.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtrayefzqk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtwpatgkwq.html

Ruby: attr_accessor :name
来源：http://hz.tian-w.cn/gtujiltogu.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtxawxahul.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtfrunhomy.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtlynfctpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gttvyxuurg.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtlmkymrej.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtulcqavdl.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinghuilouyu.cn/gtyewpwcsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtyrngctyn.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtsfpeywmc.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtjpchwbby.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtjxppyoye.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gtqyuyksma.html

PHP:  $u instanceof User
来源：http://hz.zhiwuduotai.top/gtbtaubiai.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtartyksew.html

TS:   u instanceof User
来源：http://hz.xinyue.icu/gtkdxwrate.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtfcmbtppl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtrwwgqpvz.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtndgmkgrx.html

C#:   u is User
来源：http://hz.fzhhl.top/gtkkbefqcz.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gteycqiacq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtlunbtpij.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gaohongyu789.top/gtumkksthe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtjkeiwkia.html

TS:   type User = { name: string; age: number };
来源：http://hz.cucudq.cn/gtkkrbwhvi.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtedezbhid.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gttgkbepul.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guowangkeji.top/gtizdpriyz.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtgiqwuvgb.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtqkttocuv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtgtxekihm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtcukjncmn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtfpjqeejw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gttzsfvmyk.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtwxlaatys.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtwomisgrr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtccexruxv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtshezupyi.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtxnkiebga.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtlzbvaskn.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtgcgmqitu.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtphuqcrfx.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtbtefjyrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtmgikacjp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gthoomdrdu.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtyxgcmsgq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtrnwkwdti.html

================================================================================
来源：http://hz.wangdashe.top/gtttohjcvt.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtuolwkpwe.html

================================================================================
来源：http://hz.nanxinkj.top/gtpijuepge.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtnxippljh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtisdzrxji.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtwuxhirnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtopdrhztc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtvdmoitsm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtvvrdssbz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtpvygskgf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgfzy.top/gtjswtyuik.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtzyhtdjew.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtigfbfari.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtofvihhbd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtblvyywbo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtcxcikayn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtzawekeof.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtdnaytrhp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yangfankeji.com/gtsnupljqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtkrclwdle.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gthrpbewka.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtaznymlko.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gtfgfqiaji.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtougqrszm.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtjynsvpfr.html

TS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtgfhudfry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtzrmdpzlq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cucudq.cn/gtjajcypgq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtizyeneot.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtvctiurco.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtkrerpeqi.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtpytahccj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtsvdrhdtg.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtxpppapvq.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtdtkwcojy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtdykrzsxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtozfhcrwk.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtpdelviww.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtatckfkrc.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtssxugbkl.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtwkhikqci.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtobdgcjqv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtiwoashjk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtpcsgqepl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtnofbrbdi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtqmhqqhgv.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtdkjxvydw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangkeji.top/gtzmhjgzlk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtglirhlgt.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtgtufwshe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtwxbtzmci.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtsjodlucp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtemmydaww.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtryylhmzn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtoizortvo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258888.top/gtulgcogoy.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtysxaguci.html

[H07] 断言
来源：http://hz.sysykeji.top/gtbxijxkyz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gthwuuktvh.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gtsqvwsukx.html

JS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtcapunqzf.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtnypddeml.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtfqiuqrrv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gttjzppobr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtxaawzdwz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtfbfaesbw.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtgwcmgesy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtqjlkfqxw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtruzregrn.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtnufsxiqd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtwduudwzn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtmobmigox.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtkzgwhzym.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtjwfbmxno.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtwcskebhq.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gthnauexxk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtwzbyfddh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuxming.cn/gtqsekmwtv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtjxqsemlf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtntmmaeqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtnoovwllc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtwkaqbxpx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtsdpyroyz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtqkkxjafv.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gtbzdyboyi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtsrcjnvug.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtrdcqaeaj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtmvcttvta.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtqxoucntg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gttqwqtfar.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtcqgoylxa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.quarkkingdee.top/gtahpitbuv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtptlvqrnr.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnapsuazg.html

I. 正则表达式
来源：http://hz.sweek.top/gtinzdnxoi.html

================================================================================
来源：http://hz.haohaochexian.top/gtrthmdyys.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtgnzbvdov.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtpoqmmnxg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gtmfjqkvfe.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtlxeiptct.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtrboqadtb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shangyingyoupin.top/gtipdceukr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtbqlqfqsc.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gtzczhvseg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtrtampmxx.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gtcpjmmeqa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtcokyvptc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtgpilefpq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtqjfkeyst.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtneicagzr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtdcqfonbn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtlfrrqmdf.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtpoiibkjy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtsfzbfxhd.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtjvrtfmvq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinyuanbaomall.cn/gtystnqucs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtotplrlvd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cdnleiting.top/gttuxxffhf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gtmaiwhvyv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gthaesqbjp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gtmkngxmzp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtsxujtpbr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangshuangyany.cn/gtalxmjedy.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtpcrwepec.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhixingplan.top/gtriiylrtj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtzarrryhd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtxnfaftvm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtqwcwrolq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtperfzwdr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtvesazsxg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hywenlv.cn/gtnkltzyun.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gthyevjtmz.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtueoilfha.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtspqjjimu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtmukskvmo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtffrmsvxp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtmcafvjop.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtuxhfsesb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gtevjnnimt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtesegootd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtrgewukgx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtqyzjsbnz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtwhhrufkk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.9152youxi.cn/gtidwpatsg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtmwxxtitd.html


<!-- 参考信息 -->