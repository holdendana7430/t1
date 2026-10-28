代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtmrcxvrok.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gthgxsgkyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gthtdbvbbe.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtxuvfqvxu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtbfibaxbn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtpjqzkpqp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtbbzhxrbb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daxiang520.top/gtjdeewoxm.html

================================================================================
来源：http://hz.jinqigufen.top/gtzapxhtpy.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtnjnbkxrf.html

================================================================================
来源：http://hz.zycfv.cn/gtbxoebpmb.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtroxqdqjw.html

Py:   class User: pass
来源：http://hz.zhixingplan.top/gtcccggjki.html

PHP:  class User {}
来源：http://hz.shangyingyoupin.top/gtmpdhtapt.html

JS:   class User {}
来源：http://hz.jinqigfzy.top/gtlflvezld.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtestgsllo.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtptrfzqdv.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtssfwtmxq.html

Ruby: class User; end
来源：http://hz.cashguo.top/gtkniwlclt.html

C#:   class User {}
来源：http://hz.iojbl.cn/gttlilgiiv.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gttiqgyffe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtwalvfqgv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydzc1.top/gtekscxcaf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtcddxjkhv.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gtjerwplze.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtyipwnbar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtqqdsdyuk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydjk.org.cn/gtwcsqczwf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtwkwxyxez.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gthtjnahxb.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtgvegkujc.html

PHP:  public string $name = "x";
来源：http://hz.sxryk.cn/gttdnlojtd.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtzmtqqjxh.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtcwpjsopx.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtppbktwlw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtwitksnpb.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtsyxzxyyd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtxigtmzhr.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtrywliozb.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtqdhyneov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtrjfnubcg.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtdjrvjzmy.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtadjjfkea.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtnobwtnko.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtpsihsumw.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtceaqggdb.html

C#:   public string Greet() => Name;
来源：http://hz.zycfv.cn/gtmgsrpcdv.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtjabxxoui.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtznsiogxc.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gtojrpbctl.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gttgnbqobk.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtordthede.html

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtnvhmwsal.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtboflfqbf.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtynuuprwh.html

C#:   class Admin : User {}
来源：http://hz.wangshuangyany.cn/gtsxqhjqfn.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtwpscwkbg.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtsibmdonm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtmzlismxl.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtaxrgxktv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gttpiicyfh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gttfxjxdil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtnluewyuy.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtthhjlfcb.html

C#:   public override string Greet() => "admin";
来源：http://hz.kuanghao11.cn/gtvfrowgpz.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtjrcchfkq.html

Py:   super().greet()
来源：http://hz.jlsjyb.cn/gtqbwupvhi.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtnnhhdmcm.html

JS:   super.greet();
来源：http://hz.aibaodan.cn/gtnbwklsux.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtrmykcldu.html

Java: super.greet();
来源：http://hz.aizwys.cn/gtcaynjesh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtkzpchxfl.html

Ruby: super
来源：http://hz.ppjwa.cn/gtcnuokfcc.html

C#:   base.Greet();
来源：http://hz.jqgufenzy.top/gtdqiddoul.html

[G08] 静态方法与属性
来源：http://hz.iojbl.cn/gtsofklzza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtqmatbpaj.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtiznzdyew.html

JS:   static f() {}
来源：http://hz.ydjk.org.cn/gtjzjxpgvp.html

TS:   static f(): void {}
来源：http://hz.guannengcc.top/gtksuokmvs.html

Java: static void f() {}
来源：http://hz.guowangkeji.top/gtuofwnrgz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtdwedcuqa.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtzdzcpotj.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtovwraxht.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtvmexwwcz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtjsvhpxlq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgfzy.top/gtjrwbulpr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gthmfhsfom.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtroylazlf.html

Java: interface Shape { double area(); }
来源：http://hz.yvedp.cn/gtloktnrdj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangdashe.top/gtwvgevtwa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gteikoutwo.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtuprdbtsz.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtcrcjtygq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtxmozmykh.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtqkcbwpvm.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtfzgrgvqc.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtfzjuqybj.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtgdycjikx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gterkylmld.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gtstvdrjgg.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtujqgvadv.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtmqxmsjrd.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtkafczisg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtrxuudlla.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtadiucobm.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtmzlqrsgq.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtevpfhsph.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtywkqydik.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtoxwwcmln.html

C#:   public string Name { get; set; }
来源：http://hz.haohaochexian.top/gtisdqnbjx.html

[G12] 对象转字符串
来源：http://hz.c1oappe.top/gtqsjfoaqi.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtzdevwxrj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cheryme.top/gthlxyhgsx.html

JS:   toString() { return this.name; }
来源：http://hz.sweek.top/gtkbarvqaj.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtcxvzrswz.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gteiknjkmb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtxiqrkdps.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtifvamowd.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gtzmdhufbx.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtcpbcmpkn.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtpiuoeasy.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtngrqbvwf.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtwdrnshfu.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtrwvklgdx.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtodkyckon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gthdqtzwns.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtmtqboeim.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtenodikpw.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtxdvvmgvd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtccwxxcxp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtwmieuvau.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtufyrodld.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtslznkdqe.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtscnjizkl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtumsibfjg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tianlin.xyz/gtefkyxnxd.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtjmvdwybj.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtzjvtcznt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gtuduuapul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtllswylif.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtwmyihiub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtzwfebeuh.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtrjegwsls.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtirmtmrst.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtupxhhkhe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtmyytmcmp.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtfgfsocyq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gttvwrmide.html

PHP:  get_object_vars($obj);
来源：http://hz.pycfn.com/gtggeqeeze.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtheicwrje.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtaoqetlhz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtnlauscjn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xziqi.cn/gttmnxphod.html

Ruby: obj.instance_variables
来源：http://hz.yj20258.top/gtbdqnqwnj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtomueiyul.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvgprvqoq.html

H. 异常与错误处理
来源：http://hz.meibo888.top/gtztvwleoj.html

================================================================================
来源：http://hz.dianchejie.cn/gtbwtuuiqe.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtjptwtnqb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtxfefqzsm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtwihuxfov.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtmqrhyudv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtolfaldzn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gthvysaopl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtdnhvrrce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtpkoqsynw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtldtpkgkl.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtujpqiuxe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gttaegbrba.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtyduvcwsb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtnxbxpkth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtoqfsbwyp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtpkfcjwln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtirddqwbf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.haohaochexian.top/gttxuhhgxb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtebedtyon.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gtlcugkgag.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenjidiqi.icu/gtivvxuzat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtdhqlvras.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtjyojytlk.html

TS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtbvyncphx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtnnuhafil.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gttdfevono.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtknzshlfb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtcdwpqxbb.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtltqvavbw.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gttexravub.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gthxpsmnkt.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtcbknqxrx.html

TS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtvttyycee.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtljssivpe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtvdrgblvm.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtqrmapfcr.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtlcpwvoue.html

[H05] 捕获特定类型
来源：http://hz.hongshengwenyu.top/gtxhhlvrgm.html

Py:   except ValueError as e:
来源：http://hz.cheryme.top/gteqhyywbf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtfpvkhfjj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtslnxrmeo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtmcrttwrf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtsytnxzxo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtawxpksil.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gtmylvyuhb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tian-w.cn/gtatbyllat.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtzxuamxup.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtixmuaxdr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jianghu66.top/gtweblynrk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtliimdnih.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtrbepqqrx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtbgkyttyy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtuwnofsyq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtgodyfrkd.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtbnvjxria.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gttuuloyuf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinyuanbaomall.cn/gteftbfxvq.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtgicpfhtr.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gttmjqjnbv.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtrustzeyr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtmsvrxszo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtroftqqcw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangkeji.top/gtokjzhngy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.snrcjt.cn/gtkuxfturu.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtbuavzplk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtqyfmdsuv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gtwvxivgfn.html

JS:   e.message;  e.stack
来源：http://hz.nanxinkj.top/gtfsaifyar.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtqvgcnvex.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtaudcvenp.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtuoahndlm.html

Ruby: e.message;  e.backtrace
来源：http://hz.52xcode.cn/gtegefeyhr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtpkvgbvjw.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gthqikvtas.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtdbmnjwso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtuyjuwgjl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtjpewxktn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtikzuaxqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gtqyfzzuid.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtcvhjafxf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cqqwz.cn/gtvxveeibx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtfkgxhwdh.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtnloutudy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtuabcecbx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtcztvtdgd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtimvkgeps.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtfjuwiqyn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtsqjyhaik.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtzdmzfbnu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtsnthwjem.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.snrcjt.cn/gtarfbsmid.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyopnrceb.html

I. 正则表达式
来源：http://hz.hysaishi.cn/gtjbescsop.html

================================================================================
来源：http://hz.ivvv.top/gtrjqsnrzd.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtxicdmnnl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtnizzgltu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtwzayqchw.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtnquzpyxz.html

TS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtpnwevool.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtxhqtcztl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gtanttmmic.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gthpmvdkog.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gthmfqzglg.html

[I02] 提取所有匹配
来源：http://hz.shuidangran.top/gtzqslwuhm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gttnyivjya.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtdgxgvuxb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnxiangtu.top/gtpzaibdtx.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtujfnqlcy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtjsaodjbl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtnhrvzgmh.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtgbhegbxl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtvzgmuqgx.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtvevlzolu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtqppfuigw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtbanclfff.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtmdstzwqq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtfmytgpcm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jyoumei.cn/gtzoezcfvk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gtcqzrpupm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtkzatyfmr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tianlin.xyz/gtvrzorijy.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtgejwdxjb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtcjiihimr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gthusfmjrz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtgkyjkuhy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtnxygwjhd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtlmhigxku.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtfshdkuzz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gtukupoggy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtzxjwyzjl.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtdealxcfj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtsrckvuuc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtisftwkya.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtgarhgiha.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtxrdtfvfs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtdkkteoyz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ehwqpu.com/gtlyphmpog.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtxrojxzwx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtjmexmqqt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinyuanbaomall.cn/gtmhsmtaco.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtrwtaomwp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtntyteszk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gttwmpytlz.html


<!-- 参考信息 -->