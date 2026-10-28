代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtslvxbpkv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jiagoushi.top/gtwfgijkpf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gaohongyu789.top/gtokulbare.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtbtejkbkr.html

================================================================================
来源：http://hz.yj20258888.top/gtylcrowwj.html

G. 面向对象
来源：http://hz.nwbrower.top/gtnbcalkyj.html

================================================================================
来源：http://hz.yongpay.top/gtkqiphcib.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtrvmodzfv.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gtrwljdsxs.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtrtnslvgb.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtrfsybimb.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gtwhtczgks.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtgkvyvmar.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtqdbpeqns.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtrvxmycaj.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtojkxupsb.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtnzqzylxp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtnvtablmp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gtrfkprzul.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtvxvvyxyl.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtyejthnqa.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtgwggpcux.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtksetwdlv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtcaerwojv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtpokdeefm.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtozgxtnwm.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtspooocly.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gtdosslswo.html

JS:   this.name = "x";
来源：http://hz.dianchejie.cn/gtfnrlyqhr.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtbmyiibhp.html

Java: private String name;
来源：http://hz.iojbl.cn/gttmzxqaes.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtdvzpmref.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gticpmcoow.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gthreilrmh.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtyoaxpubp.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtvtuxnnju.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtdkabzibo.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtlhthhmxg.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtzuttbvpr.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtuwolelsl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtzqstmvyf.html

Ruby: def greet; @name; end
来源：http://hz.chenzaomai.com/gtbnkoqiua.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtaneufzrk.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtozjtyynj.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtbnkxilux.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtyeamkfln.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtsblnyyay.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gteryoaeit.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtjanprnyi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgufenzy.top/gtdsjxhrel.html

Ruby: class Admin < User; end
来源：http://hz.smart0.xyz/gtvtqiwpjf.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtxxigqtom.html

[G06] 重写方法
来源：http://hz.meibo888.top/gtodztighz.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtngewxbla.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtzehiywbt.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtgfepstgb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gttofpvpzz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtqwkrkpzs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gtdtnuyjdu.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtazjixmuo.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtvtxdvike.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtowcaddie.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtopebkdef.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtbvxyphrs.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gthbhxuufc.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtogbchhfd.html

Java: super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtejtekohj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtkfdndmrf.html

Ruby: super
来源：http://hz.cucudq.cn/gtzftzduly.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtciwutpnk.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gtchsgllpx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtyiwqqhss.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtzvzyllcf.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gteqpkrgqc.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtvsrshrev.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtfubksrrz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtutuexbji.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtmnaqgmix.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtfyldhqyh.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtgwarkrxl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtnopynmep.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtsunoooqw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtissrxvks.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtdioogswo.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtxyumvoli.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fzhhl.top/gtebxrzdgj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.svipenyu.cn/gtmkgxdwvl.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gthfjyauoz.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtraplvpnr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtfbmcmubv.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gtwoyqwykr.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtedlxlctq.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gtxfkpdetr.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gthuzpavms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtzrpzhaex.html

Ruby: public / protected / private
来源：http://hz.havefunace.top/gtyepngoul.html

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gtnfywsglg.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gttnvmgylb.html

Py:   @property 与 @x.setter
来源：http://hz.wangdashe.top/gtimvubpop.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtdgorwoxv.html

JS:   get name() { return this._name; }
来源：http://hz.pycfn.com/gtmfalbgrc.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtukbqqxqk.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtvcsygcpm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtlzvnbdey.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtvunhrhwa.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtqzqmdhir.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtgfjgfbob.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtrawkyyoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtddjfetkv.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtnjlwqgtt.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtouphjhvz.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtmcqbcqwi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtaisfaocf.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtsdtsmlef.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtypuilmbz.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtplnnvzth.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtcnitykud.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtshtecjwx.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtzggptnqs.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtruykuczb.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtspbfbtcq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtlwbcufhl.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtkvdynosy.html

C#:   u is User
来源：http://hz.cucudq.cn/gtvqqoiqcd.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtsayqeolp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtdxvwxcgv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xingfuxueyuan.xyz/gtfayjqnki.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhaomingkeji.xyz/gtotjgzivl.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtgknxsxhb.html

Java: record User(String name, int age) {}
来源：http://hz.gotoacloud.top/gtyagvlmnp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtorqytuhp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gtocktlibj.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtoxevqzfo.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtbiyahdht.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtkhkfkexu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtdymttnxr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtcnoacknh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtwnzkypxm.html

Java: enum Color { RED, GREEN }
来源：http://hz.ehwqpu.com/gtkaexbevi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtqcqpocnr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtsocsdqfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtrqwlugrq.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gttitsezsn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtcnagkbjv.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtgcegkiic.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtjlhzssht.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtljjasgbz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gtlhzubtyg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtywtijkkz.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtdlqyttnu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pycfn.com/gtzqcsjyxl.html

================================================================================
来源：http://hz.aibaodan.cn/gtlcrdsund.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtsbhiqiuk.html

================================================================================
来源：http://hz.dashuyun.cn/gtdmzdpsqx.html

[H01] try / catch 基础
来源：http://hz.sysykeji.top/gtiatjtfth.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gtmdbljpia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtfuptiwzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gthaxlscoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtxtewhqsg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtnjclqxti.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtaoyxujpy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gtlngwnsci.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtlrgnckte.html

[H02] finally / ensure 收尾
来源：http://hz.zhongyouzk.top/gtambdmvol.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtkhzawung.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtohsnjddi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtoodcbdgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtjoykvseh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtdsgsnzex.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxuanxn.top/gtmofzfgut.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pengpengdd.cyou/gtzriwqxnr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtnxqbyawu.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtaqzxjmse.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhixingplan.top/gtubxykjgw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtlzxctpds.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtugktleeh.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtqsjkarsd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtpehypadf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.quarkkingdee.top/gtuqxnqlll.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhoulong.xyz/gtnfnbxsrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtydnjaslb.html

[H04] 自定义异常类型
来源：http://hz.jinghuilouyu.cn/gtfqvosmwi.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtoywryqbv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtmsrojkwg.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtuhpcuaol.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtyieudzis.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtbzivtceq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtptxfvonu.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtnowwfwmj.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtmepcyrda.html

[H05] 捕获特定类型
来源：http://hz.daxiang520.top/gtbxwyujhb.html

Py:   except ValueError as e:
来源：http://hz.hnqzz.top/gtmgwzfkpx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtmmuvgvex.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtmuopompx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtkumjbpis.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtjxeduvla.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtwcxcrplf.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtltzruxxr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtiuzofqjz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtwbgjzwcu.html

Py:   value = d.get("k") or default
来源：http://hz.svipenyu.cn/gtzdhmjcan.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtyopqsolt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtvwqdirmt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtzexgzawu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydjk.org.cn/gtxwhkhvda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gtppggbkww.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtebqnvqpe.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtghwdlvil.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtytsewowo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtdzpmdedx.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtkbngxmwf.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtljzjspoz.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtllgdiiae.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtqkaauymz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtfelalfxo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gttlqwfcak.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pycfn.com/gtmnpuahuo.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtyhfziuia.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gttixwulcj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtemkgkbkl.html

JS:   e.message;  e.stack
来源：http://hz.nwbrower.top/gticwkxwdm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtakxniuxp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gteqfgcvfs.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtnomrflqg.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtcdilkfax.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtpaykpryy.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtfwoqvfpd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtemdqrbwd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtuqfockjc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtpppvzzpq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pengpengdd.cyou/gtbapopuug.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtwazzzqnv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aizwys.cn/gtoxwmnoho.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.birdmap.top/gtslkghbth.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtspbkavxw.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtsfzkdsuz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtwjcvjjen.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtihvzrtly.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtkpqrqjgu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtdxfspplg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtrtuhdbqq.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtsvyawbxp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtzmizfqsa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtbishuicz.html

================================================================================
来源：http://hz.hfpthk.cn/gtnjpqrrwp.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtpbiciowy.html

================================================================================
来源：http://hz.cashguo.top/gtuypvbjdy.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gtmtolwyln.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtqotclvcm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtmeypljkk.html

JS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtqapunlox.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtxhhvhsbt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gtbaizoeiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtfbeuquqh.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtdwlvbzht.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtoqgrdajp.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtayhnkpof.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtblqptpyd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtkzotmfvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtyclxhook.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtchdlqqev.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtmvkfmvdm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yueranfly.top/gtffhlckvo.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtzkohufth.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gtyvdjsxqc.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtqijjdesj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtlovbpgnr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtfcuiuokw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtkvrtrecc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.quarkkingdee.top/gtoajdetxe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtvlufgdid.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gttibqzqie.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangdashe.top/gtvcbvbnxx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yvedp.cn/gtksiyrirk.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtpzbrafbd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtxhruokqw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtbdaetotl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtbgscldna.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtikixrbvr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gtppxdqplk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtypskjhqt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gthnqormum.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gthyioamgz.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtnpewrndx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtwdmdmmuf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtogrzdhfn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtazfupsdo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtdfurhtex.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtnneboibq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtupuncwgs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gttmqdtdyk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtvzkvvytc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gttutubonc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtctodcbyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtnxvvdwbq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtgynnjneo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtphcghcja.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gttmctrsgt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtythogras.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtnpyicwac.html


<!-- 参考信息 -->