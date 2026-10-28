代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtfrspgqms.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtxooobgma.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtwjesgfya.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtxxyyxdmr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnqzz.top/gtnygfyhrf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtxsximwpe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtxphwmraz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtfhpbwgnl.html

================================================================================
来源：http://hz.zhengqikj.top/gtqsrjstuh.html

G. 面向对象
来源：http://hz.jianghu66.top/gtqpbwlgsk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtffilzedb.html

[G01] 定义类
来源：http://hz.52xcode.cn/gtecqooqnf.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtqvrnhsxm.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtgzpjsjlf.html

JS:   class User {}
来源：http://hz.cheryme.top/gttdgzreow.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtqfzhzeda.html

Java: class User {}
来源：http://hz.ydzc1.top/gtfwnecbyi.html

Go:   type User struct { Name string }
来源：http://hz.ydjk.org.cn/gtashnrbtz.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtmkbameay.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtxxclgzgk.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtiffilgen.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtcosqvuvd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gtugrmumvp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtwntswsre.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtptyjqrhq.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtjorsnigs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtgdxpawml.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jiagoushi.top/gtweiyoxss.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuanzhike.top/gtkulbkdes.html

[G03] 实例属性
来源：http://hz.pengpengdd.cyou/gtkfqjgjis.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtdzaybjer.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gtrwkwzfwp.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtnsdjhfxd.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gtvjinwmaa.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtawmpvoqd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtosgdcvsj.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtwenumuyr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.quarkkingdee.top/gtduteqsok.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtuknkrlwz.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtgwegbkbk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtavccbmze.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtkgxqivgw.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtamvhdttm.html

Java: String greet() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtpijyjaao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtukkucuwf.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtpmfnledt.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtxtyejxjr.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtiqoxxqlz.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtyaswwbzc.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gtmxjitjao.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtmbxnikwf.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtcaznknyw.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtyuhxiaoj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtiuafijub.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtggnjvywj.html

C#:   class Admin : User {}
来源：http://hz.shangyingyoupin.top/gtxeebzouf.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtybgoaimh.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtbnzhtuwg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gttcvcddwe.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtbtntzzqc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtxooymlon.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtxsfgoyve.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtkwynlzce.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtpbmlgcnl.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtxvefngyi.html

[G07] 调用父类方法
来源：http://hz.52xcode.cn/gtbzmaxwmv.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtfxpbwoha.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtybyckrfv.html

JS:   super.greet();
来源：http://hz.yvedp.cn/gtjvxatmsg.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtymunggup.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtgixfavyb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gtawtjxmzl.html

Ruby: super
来源：http://hz.sufxvd.cn/gtkcemehcz.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtbxmrivii.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtxswdnvje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtfnqrsvtz.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtxkysjnvr.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtbsfrnyit.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtwcppcpuz.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gtjuelgtks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gtzxlwgrvh.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gtgoglgoxb.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtupbzroxc.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtlfqhexmf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cdnleiting.top/gtyzjjvhrm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtsshhvfxb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gthmlttixu.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gthhyapgcj.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtyekcxgbf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.svipenyu.cn/gtdgqchjft.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtzxbpfrzs.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtuzlcjckh.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtavudtpyv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtdnefpvbf.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtthqoxesr.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtuuarkdcp.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtxbebkypn.html

Java: public / protected / private / 默认包级
来源：http://hz.yueranfly.top/gtxxatlrdy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtpzvjzkly.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtzxxpuzfx.html

C#:   public / protected / private / internal
来源：http://hz.xuetiantiany.cn/gtyihyvfbv.html

[G11] getter / setter
来源：http://hz.yongpay.top/gthtmehnbw.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtumxiqnmf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtjwroqxzb.html

JS:   get name() { return this._name; }
来源：http://hz.ybcxt.top/gthxuqvedu.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtlyjinbqy.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtkqvecmen.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtyuwnregy.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtgmshynde.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtotlpcrhm.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtcyiqdyuz.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gtsymdxiwh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtoypyunzq.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtcifwvnda.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtdpljlrir.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtuaykfgdo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtiedusixe.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtomrvrvuc.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtrsawdlnw.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gttsnbjlli.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtfvhwliei.html

PHP:  $u instanceof User
来源：http://hz.ybcxt.top/gtahazfsve.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtcbiotxxw.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtqpmydrnn.html

Java: u instanceof User
来源：http://hz.chenzaomai.com/gtrnkcbhay.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtdfvldhxa.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtauiojzwm.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtpdcbylfp.html

[G14] 数据类 / record
来源：http://hz.gaohongyu789.top/gtzbgycemo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtslfkelca.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtmimdwzoj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtxyvghjqz.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtzwyfqyyk.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtpjaxdnyh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gtuggxijxf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtgsksyqkl.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtsynlbgia.html

[G15] 枚举
来源：http://hz.sweek.top/gtvezudcqs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtnuvietje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtczhlgnxb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dashuyun.cn/gtxlfhxnwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtdyqjgkox.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtpwexwerd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtjdwexvdd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtsxuhuene.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtvcfnpxui.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtkkpwxdor.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtfnugtoyj.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtpcsvxejl.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtzwgdinnh.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtowgkhjev.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtpptecuqf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gttncyclif.html

Ruby: obj.instance_variables
来源：http://hz.hywenlv.cn/gtjsuyqscu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtqsxdihhl.html

================================================================================
来源：http://hz.cdnleiting.top/gtvmvlyzgv.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtlnunvrql.html

================================================================================
来源：http://hz.jyoumei.cn/gtcmqvaqye.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gttyalresn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gttfimubxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gtieygtnpg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtoduwhnco.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtialjufiq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gtzmacxhos.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtpdktsjnn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtwiubttjh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtuupiycwa.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtwjnsqeel.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtrcredkwt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gttpjwbucr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtemkzlsrz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtpsddsuvk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtlaurrndg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtglcvlrqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gtdpmmlqjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtpcnwnqcm.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gtvinaesrg.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtampatzkg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtijwtdsjy.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtlfdfbtim.html

TS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtkhyfirpq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtztjfzphp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtnfsatlmt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtpaqkyvrq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtrdqqtfib.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtllubhmdk.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtyqdausue.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtkgeumcbd.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtovoratvg.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtaglvqtxq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtrivwprms.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtoyobjgtz.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gtpaoruekk.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtjzgcikyl.html

[H05] 捕获特定类型
来源：http://hz.vqdsnc.cn/gtwdxsfpmm.html

Py:   except ValueError as e:
来源：http://hz.sysykeji.top/gtlcjbfktl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtgtxheloa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtnwcwbjwa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtyruejuix.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtfjszofot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sweek.top/gtpfkcptqb.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtlioqzhrr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gticjbicdi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtfeiqdhhj.html

Py:   value = d.get("k") or default
来源：http://hz.52xcode.cn/gtqinuvfdx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtjxqvlfer.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gteldpeavr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtxhoylknx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.havefunace.top/gttqfymzcp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gtvmxwzufv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtcflwgrsn.html

C#:   obj?.A?.B ?? default
来源：http://hz.redwolf501.top/gtuyqvldvh.html

[H07] 断言
来源：http://hz.tian-w.cn/gtzcqqrycl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtjmxkeczh.html

PHP:  assert($x > 0);
来源：http://hz.yuanzhike.top/gtvdmwiafp.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtdnnngjps.html

TS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gteiwasihf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cashguo.top/gterykhpdv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydzc1.top/gtlwjfhjfp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gttltjqvpd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtfujbpjtp.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtideoxmyd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtqrideeex.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtorkrcdww.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gtdraucmbd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtdotfoqyb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtimtcijbn.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtoyiyqqvc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtqseedqoy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnqzz.top/gttvzadord.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtrnauqcef.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtzouozzeq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gthfnhngua.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhoulong.xyz/gtqkeylinp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtmsluwpsj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtdgzdkrad.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtdoqpliaw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtmcqcbrom.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtnjtubwcp.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtwdhdmqzo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtvigvvadj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtogkzugee.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtpzkueejv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtnbajopws.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gttnqiopvd.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtmhcdolak.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gtmqnlylve.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtzozvhzeq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkhfypmrx.html

I. 正则表达式
来源：http://hz.gzhubu.top/gtsyyhxzqw.html

================================================================================
来源：http://hz.0kj1m.cn/gtpleovwjs.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtdqympuye.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtqtxlgnzq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxuanxn.top/gtzwcrarbv.html

JS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtzudwhibc.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtufursjdh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtlledfhqr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtrsjsaknj.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtqlzojqzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtwaajnsse.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtgcyycjaz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtokmmhvyx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtxmbetzth.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.9152youxi.cn/gtaojklafp.html

TS:   s.match(/\d+/g)
来源：http://hz.yueranfly.top/gtfyhfblix.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtpuhmggaj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydjk.org.cn/gtvnvrgltr.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtjpmylorv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtkzfwfhot.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtfrrmtptb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtpnhwyick.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtlmqojhfg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtfefffmih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtevrtdddv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtegdivowi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtxxtcsqcr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtkosiypkj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtrnqyyibe.html

[I04] 正则替换
来源：http://hz.ywan-chungtsiang.top/gtdtifexbv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtrtbzjyca.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtqbzxncap.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtmfsbzfpj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtikbcvgcb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cashguo.top/gtjxentldx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtyklsjofc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtglmututv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgfzy.top/gtcyvnbbmv.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtkmleqvcb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.bjfxy.top/gtwciejkbe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sxryk.cn/gtwvsjfvii.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtmkqgowcj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtsxebyzhs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtxjshjnfb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gthmrhkkpx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtluqwbatp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtdcsletvk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtosffqopy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtysessrve.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtrwuwrgmq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtibfkasrg.html


<!-- 参考信息 -->