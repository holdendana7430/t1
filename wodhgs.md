代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jiagoushi.top/gtpfrmpnha.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cdnleiting.top/gtmmimylxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.andypj.xyz/gtvvxsbgej.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtyfoyazoc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aizwys.cn/gtuejvfbpi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtvvbxbeay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtgqcoxkdk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtrunlrbbs.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqymnxgof.html

G. 面向对象
来源：http://hz.xziqi.cn/gtrvarqsxy.html

================================================================================
来源：http://hz.0kj1m.cn/gtoaxroocq.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtuzjqdkvv.html

Py:   class User: pass
来源：http://hz.aizwys.cn/gtzicqatzm.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtpjjgmwnv.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gtpsowsqtt.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtytvmesla.html

Java: class User {}
来源：http://hz.sysykeji.top/gtjkqvexet.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gthkkosrly.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtzijrjefw.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtjozoljrk.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtlqghyhgw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtpjvsyygj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtkilvbpyg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtgygsfsik.html

TS:   constructor(public name: string) {}
来源：http://hz.zhixingplan.top/gtgvlrttlc.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtsqvoaflx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gthgtzhyhi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnxiangtu.top/gtjzofuhuv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gtkrqouasw.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtxpogjibv.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtiveelngn.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtjtofhqye.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtdgnadshf.html

TS:   name: string = "x";
来源：http://hz.jqgufenzy.top/gtlgvtimxt.html

Java: private String name;
来源：http://hz.jinqigfzy.top/gtndljzxbm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtctdbnohv.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtyphffkcm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtshpigcfo.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtllltfxky.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtzsvkeduc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtolzwzbta.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtybvqfpiv.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtkbckbdje.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtmplphfyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aibaodan.cn/gtylngrnli.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtyvhloueb.html

C#:   public string Greet() => Name;
来源：http://hz.ivvv.top/gttyafmrpi.html

[G05] 继承
来源：http://hz.pycfn.com/gttpdgyzhx.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gttygoapjs.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtuanudymr.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtflhowjgm.html

TS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtmopqcwja.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtaupmoqsg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtdbcumaib.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtqjecvjqj.html

C#:   class Admin : User {}
来源：http://hz.nwbrower.top/gtcxatopdu.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtwhtqcpzc.html

Py:   def greet(self): return "admin"
来源：http://hz.ivvv.top/gtcjsphryl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtxjssavzc.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtvbzzpztm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtlmkbcxxz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtnpeqlsgy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gttbircpra.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtoskkspxv.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtgmyrpemq.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtaamqczeh.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gtdhivnwfp.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtflfhwwqd.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtrhxqexzi.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtbxkjrrie.html

Java: super.greet();
来源：http://hz.ywan-chungtsiang.top/gtvczsihvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtgncchvsf.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gttfgzluvr.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtbyhvflpx.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gtykbqjyuo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtqoqmjvav.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtlpvnjfqi.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtbrtyccev.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtztyjzvym.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtavubkphw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gthmfjpadt.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtgsfxturf.html

C#:   public static void F() {}
来源：http://hz.9152youxi.cn/gtmajlcobi.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtnvaoqgyu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtrrvikczi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jianghu66.top/gtvwshlhiw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.havefunace.top/gtusudeyiv.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gttsrfzhif.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtuodgzwvu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtglwzcwfo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtibiuvcgt.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtclgpyeqp.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtrvtvsypp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtpwfowaou.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtcxmfgyco.html

JS:   #private 字段；其余公开
来源：http://hz.fzhhl.top/gtqhuxocgn.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gttxtkuouz.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtuddpkzgd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtqbhfqlwh.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gterexhtai.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtcqpyblxw.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtewsyutdy.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtzmgikekx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtkgkksiyh.html

JS:   get name() { return this._name; }
来源：http://hz.xziqi.cn/gtdjerjbsp.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtmejcqfwb.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtpqilsrlk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shzxlz.cn/gtmkgadulc.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtilqobbkc.html

C#:   public string Name { get; set; }
来源：http://hz.ybcxt.top/gtqyrpudqb.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtqclegsaa.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtfthfekuc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtfbycjuud.html

JS:   toString() { return this.name; }
来源：http://hz.ydzc1.top/gtaepdfkif.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtcxztoizz.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtpzftwyze.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.9152youxi.cn/gtgydsqoyh.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtbbrroaio.html

C#:   public override string ToString() => Name;
来源：http://hz.xuetiantiany.cn/gtyqccinhl.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtcttmtoas.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtrqtlexja.html

PHP:  $u instanceof User
来源：http://hz.daxiang520.top/gtzivjiqff.html

JS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtdvhxyxbj.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtycvykatz.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtqkedrrpz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtpmgqhplm.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtvngbiprx.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtqplskmip.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gtiwuetpeb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtkqpysoqy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtrettpedx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtcodktydl.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gtvyiopevp.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gtwgypvgil.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gtpnjmlxnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gthzmyhwzx.html

C#:   record User(string Name, int Age);
来源：http://hz.daria6918.cn/gtfbxijcjx.html

[G15] 枚举
来源：http://hz.yonumen.top/gtvonxdkeg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtcdrutepc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtdieyrijx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtipttrsfs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtocaolwgl.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtxhjdvujl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gttkkgkkks.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuetiantiany.cn/gticzwpxrx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gttvvozwaa.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtsxosswhz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtgytdkkbb.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtnyuyfdvo.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtdnwrolbk.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gthodmxoci.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtwarpcnev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtxwiuyfir.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtrprdifqo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gthmailbjj.html

================================================================================
来源：http://hz.yonumen.top/gtkemogcjt.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtwxmlzibx.html

================================================================================
来源：http://hz.sysykeji.top/gtufxowulv.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gttrfcmdzh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtcaztpyqe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtfrgvynqa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtidzdpcvh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtvgdqjzpa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtwubzegih.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtjziegorx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtxrshqvgz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtcualtuhr.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gtmbsunbih.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtqrsjkvdi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtiblbtpjg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtpucrmsgc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtwlcbuenn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtorgssdhy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtmabtilhv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gtqqhcjsca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gtcvpazywt.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtzuzuhszt.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gttfsmxrcm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtwrdfljay.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtyvkujurc.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtzwggmcxe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtxezjnyok.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtyaebyhci.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtlceogpgu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtpqsnpffv.html

[H04] 自定义异常类型
来源：http://hz.ydjk.org.cn/gtahyjfinz.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtucafxeci.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtrvstkqoz.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtmvqaoeon.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtkgyhhehf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.iojbl.cn/gtbbyusqak.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtvqpgegrs.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtsdztpvbv.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtaleexvxf.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtmotcajvg.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtxhzrjxsn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtkwdvywmw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtldylzklf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtghebfyox.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.smart0.xyz/gtruwezuyv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtihpehyuj.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtbjmfqmus.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtancapsul.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gticctuxiz.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtjvtjiiuc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gtlyedlpsw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtbmesxpef.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtmhdjoacy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.mhx1999.top/gtdjxbuvip.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtflrizjkg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtlunhhbzi.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtdgwlnmjx.html

[H07] 断言
来源：http://hz.yvedp.cn/gtnrbphopl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtsegcwbqp.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gteyggbndr.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtcbmpvoow.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtvrgnnuhl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtpfmfqhxo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtqhnqrvji.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtsotnropr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtwcvnxppm.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtewnemfzn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtvvmscbxq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guannengcc.top/gtoixwtpsy.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtskmymvlx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtrxtsjrfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fengsongda.top/gtuwwewueu.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtvsalkues.html

Ruby: e.message;  e.backtrace
来源：http://hz.52xcode.cn/gtkabqpbjp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gtjmtouqqy.html

[H09] 带错误码的异常
来源：http://hz.9152youxi.cn/gtypyrgjvx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtasfnjxiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtecdeuvzv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtskvceusu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtavyejnat.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtasoqkblv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtvwbqnfph.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtquuhkdax.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guannengcc.top/gtoatrrogc.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtxsnwyeds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtkfrpkkbn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtgryjxtxd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtnerlfjvs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtyjziitsj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gtifetgnrc.html

Go:   defer f.Close()
来源：http://hz.yj20258.top/gtphalfzdi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtlxxphikw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gthhasclzb.html

================================================================================
来源：http://hz.9152youxi.cn/gtwryphohy.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtjgzglbxy.html

================================================================================
来源：http://hz.havefunace.top/gtisidpnns.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gttefxkcks.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtqkohheih.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gthjyscnop.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtnwyxjgkc.html

TS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtfkplxgzr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtmfqcaeoc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtersplibi.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtowpobamg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtyxoaetww.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gteyqabizz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtgrfntzvy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxinkj.top/gtfgqpnfjc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtpcffbujk.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtoesrsudc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtlspjuqlu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtxcemucqb.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtexpflgav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigfzy.top/gtlozodkkg.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gteemwgpql.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtkghengdk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yangfankeji.com/gtrhdsxilr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gttxntqgpb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtusfivdpp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtlifhfuck.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtufmqkvts.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtsofxzalx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtgoxjqpdb.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gtftxkhrrd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtrxblhizd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gtsguotzud.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtcqxjbnkt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtvoximari.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtgeslctkn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtpfqccdbz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtkipawwdk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtmkwwcxkj.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtmjcoumdi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtxfjewlrs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtfplibbfv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtsyocmqbc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtlnnnbuyv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtxlsqshen.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnqzz.top/gtykgnpghe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtoposslzm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtaqdxzcyx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtqeymldsu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangshuangyany.cn/gtdbgpvlwg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cashguo.top/gtdvtrlxbg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtpalgkybm.html


<!-- 参考信息 -->