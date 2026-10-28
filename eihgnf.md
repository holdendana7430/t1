代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtqvselkxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtgoggdrju.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zdqjudy.top/gtsbdobmck.html

[F12] CSV 读写
来源：http://hz.yuxming.cn/gtpaixggku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtsvhkawqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nwbrower.top/gtieyqtzge.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gtsumullqw.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtoqirpvtt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtszezqhco.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jiagoushi.top/gtcolukhxo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sysykeji.top/gtzwqmrxwt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.smart0.xyz/gtpfxhsiry.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuoygtrhh.html

G. 面向对象
来源：http://hz.ivvv.top/gtbbclbsxo.html

================================================================================
来源：http://hz.dashuyun.cn/gtfymrcpit.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtjyaoxhar.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtczdehgrj.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtfrokzzuj.html

JS:   class User {}
来源：http://hz.yvedp.cn/gttlzcadfi.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtdptnpyas.html

Java: class User {}
来源：http://hz.daria6918.cn/gtwygbhwaw.html

Go:   type User struct { Name string }
来源：http://hz.shangyingyoupin.top/gtblsjfufp.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtepftiwnk.html

C#:   class User {}
来源：http://hz.hnqzz.top/gtaivqmrru.html

[G02] 构造函数
来源：http://hz.birdmap.top/gtjbqjczub.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydjk.org.cn/gtuxjudvbo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtqtrpsces.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtvabqmnvq.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtqnzzuedj.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gtbqbygefq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtuptozzme.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtrcbyzyed.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtccxsjusg.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtimbprodo.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtjdgwjmhv.html

PHP:  public string $name = "x";
来源：http://hz.jiagoushi.top/gtshhhxabl.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtusoylzqn.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtclmltobn.html

Java: private String name;
来源：http://hz.nwbrower.top/gtfftoxxsm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtenkkfhcs.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gtqtvjyvsb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtrofbsfbc.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtznqbpvjh.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtduqwlfgf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtbuatcnrw.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtgirrpuzp.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtgemsqzsg.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtljvpwezf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtirhpbqqi.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtjsmgcgyx.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtdlurzoxl.html

[G05] 继承
来源：http://hz.fengsongda.top/gtnbxaoqyi.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtzfkguywr.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gthvtuglra.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtbgvejjsg.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtatviezyp.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtdsgcmmci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gtbhyvjhrl.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtbfakpvfn.html

C#:   class Admin : User {}
来源：http://hz.zycfv.cn/gtpjvhjykf.html

[G06] 重写方法
来源：http://hz.52xcode.cn/gtxdmufafu.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtjmugstbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtzszhstry.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtbbwjtzxz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtvrmnlmzr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtdthwppgm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtlwuceojo.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtebfwvfji.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtddygizmt.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtbvhugglx.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtgxmohfba.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtcwgwbpsm.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtaqcgnjkv.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtofcagayi.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtskhjnedh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.andypj.xyz/gtwxgqcxte.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtysghhltv.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtwzcxhnul.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtnvyfzdpy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtzfgrvdpt.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtfcphtljg.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtgsswpfyd.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtdkvjrgkh.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtwrsgcsed.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pengpengdd.cyou/gtpbiiddjr.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtmkpfqwrc.html

C#:   public static void F() {}
来源：http://hz.jianghu66.top/gtndpnlqsi.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtpqsfilww.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydjk.org.cn/gtucwnresh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtxmnptxcw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtacssaebw.html

TS:   interface Shape { area(): number; }
来源：http://hz.pycfn.com/gtiwtrwpkw.html

Java: interface Shape { double area(); }
来源：http://hz.yueranfly.top/gtxpvuupgn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.svipenyu.cn/gtwvzuabki.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgfzy.top/gtahltjmhn.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtbmkmvgei.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtmptjborz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gtflidxvdf.html

PHP:  public / protected / private
来源：http://hz.yvedp.cn/gtmugrneev.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtyyszdovv.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtqqefbzje.html

Java: public / protected / private / 默认包级
来源：http://hz.yonumen.top/gtretuqzwn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtjtueynwy.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtdihhiwbx.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtlvwgytey.html

[G11] getter / setter
来源：http://hz.feifeiyinyue.top/gtnkrnmvtx.html

Py:   @property 与 @x.setter
来源：http://hz.jianghu66.top/gtmpabxcjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtwtiouzhg.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtjrxbgraw.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtpenacesy.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtxxhzdoij.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtniyieaop.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtwgsznxrf.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangtech.top/gtvcwcjsuy.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtptqirbut.html

Py:   def __str__(self): return self.name
来源：http://hz.zdqjudy.top/gtfkpctcze.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtilputmog.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtxyshzabn.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtholxenir.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtyltqlyoc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtgybihnsp.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtyqsqjevf.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtzcrmxxok.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtnhixgdhg.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gttxxzodml.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtsxwzbxnu.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtrcfqoxyz.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtilgmkned.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtzgdgfdjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtqavrlcpy.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtfmxjrjua.html

C#:   u is User
来源：http://hz.andypj.xyz/gtujfuqvev.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gtsolrdoza.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtuksuxdip.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gteixrhikq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtiinjkwik.html

TS:   type User = { name: string; age: number };
来源：http://hz.xinyue.icu/gtxvztgxqx.html

Java: record User(String name, int age) {}
来源：http://hz.tian-w.cn/gthletrcrg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtefspygob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtvbuqfrhr.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtlmammxtz.html

[G15] 枚举
来源：http://hz.cdnleiting.top/gtcndriges.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtptxxoujm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtuizudfad.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtbrihehwg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gttyxtstwc.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtmfmnxtzo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtzdizrwau.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cucudq.cn/gtbkqehyhv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtqffqaecg.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtmymtpbji.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtbyevvieh.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gthswurbzl.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gteodrigwd.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtcxazjzni.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gtepczzvli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gthcecdviu.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtzfiruliy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gttefyaegk.html

================================================================================
来源：http://hz.9152youxi.cn/gtxyeqomdt.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtfypdzjud.html

================================================================================
来源：http://hz.gotoacloud.top/gtlbvzefbr.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtbykpiumd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtedmxfaks.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gtcuumtmnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtivvqvybn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtzxepgspt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtlmivzolm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xylfe.cn/gtbstwrxbb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hammf.cn/gtjxdnitgq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gthlwhdxuk.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtfrrcyrqp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtggvusddo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtmmowwbxi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtpsbhprnk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtqusjfbsk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtzejxepdg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jianghu66.top/gtwrcctjrd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aibaodan.cn/gtojimekzf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtdgppvyyu.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gttivumcmx.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtyoobgxyf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtfugrycyo.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtuesjojyi.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtzxwpfssv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtksikizdb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aizwys.cn/gthkarrxff.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jianghu66.top/gtknwnfeuq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtmqzjifrv.html

[H04] 自定义异常类型
来源：http://hz.zdqjudy.top/gtralkhxhv.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtiteozkae.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtcoegugwu.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtpwscvfpt.html

TS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtitcjbwdc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtegwukbmr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtomenlufj.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gttrkulidg.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtkzsmalgb.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtwjytvlas.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtzjirzlqu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtdjagtgte.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtynwlkyxy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gthatvfcaf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigfzy.top/gtdchdadpi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aibaodan.cn/gtgwusiygz.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtccfialed.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtvtsmehlf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtjdtcsntf.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gteigmadoi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtcobekszs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtnyssqvww.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtqijyzqxb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gtqixqvdes.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtvroazjov.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtfumgoysr.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gthupzijdj.html

[H07] 断言
来源：http://hz.zycfv.cn/gtjmcsvhek.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtdfokkbhu.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtrjguivpk.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtuajdfxsl.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtzrvsltcr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gtyvmsfzdn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtizrrmlgg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ybcxt.top/gttmuspxkm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtqjydoweo.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxuanxn.top/gttfzavuly.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtdgytcdrc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtcfrnunbq.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtvplloenf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtcchycqev.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtqooywzgn.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtfzqyanwf.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtrqluybrg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gtppjzfocz.html

[H09] 带错误码的异常
来源：http://hz.svipenyu.cn/gtriajcloe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtvohpfzmc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtgmpsyskw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtdyigreel.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tanke756.top/gtweuoyqjv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtkedxyxtc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtfgvczxtb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtjfmehacw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtyqbsoojd.html

[H10] 资源自动释放
来源：http://hz.gogol.net.cn/gtmlxsqbfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gthbbltccu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtnhofzrvj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtuqcemrgm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtyjwggyul.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtwqehrdao.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtwlmjktik.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gteafmbvzb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtyxchbvlc.html

================================================================================
来源：http://hz.pycfn.com/gtncisxejc.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gturzwaggm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlelgvnum.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtqfpjvdhg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtnaognhlu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gthiwmybxo.html

JS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gthlsefari.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtorjbulhl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtaaayceej.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtrtwnbfjg.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtcttvhgdu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtzvogqxov.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtdbmknmpj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtilqxxysa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtuvskwhco.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenlongwang.top/gtetufhoyd.html

TS:   s.match(/\d+/g)
来源：http://hz.hammf.cn/gttwxjfzex.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtfvhbmfzy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtjalvtwml.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtiavcgnhx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtmobvzfbl.html

[I03] 提取捕获分组
来源：http://hz.jianghu66.top/gttntmjixl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtvjxxarep.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtdiadibdt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aizwys.cn/gtueqnqodk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtbdsuqdbh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hysaishi.cn/gtiqtjefyx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jianghu66.top/gtzcsucmlr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtvzithcbi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.quarkkingdee.top/gtzhuobjbg.html

[I04] 正则替换
来源：http://hz.hywenlv.cn/gtdnsviytv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtpjbjplmh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtgxbqxwjh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtqculwmry.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtqlwqbujj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtgtmxdijk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtletrfylp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtrcqunprw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtdsclewuc.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtzdvatkcl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtfzilnkap.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinyuanbaomall.cn/gtnqtouojq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtnmfkbrqr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtjvccnuiv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yongpay.top/gtfrdefxxg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gtfaeplwxf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtfnkdoiji.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.feifeiyinyue.top/gtbipjxbip.html


<!-- 参考信息 -->