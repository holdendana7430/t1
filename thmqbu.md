代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtsorwlklc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtelmolpdl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gttmgsqabq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtihjszxoe.html

================================================================================
来源：http://hz.shuidangran.top/gtpkmvhbcn.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtfrfctotz.html

================================================================================
来源：http://hz.chenlongwang.top/gtotlggwat.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtbmzouwlj.html

Py:   class User: pass
来源：http://hz.sweek.top/gtgnncgyru.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtcvnmcatg.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtfruenvog.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtqbtocsbh.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gtxxqxqant.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtekdaurxz.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtvbybvtji.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtjqfybcwv.html

[G02] 构造函数
来源：http://hz.daria6918.cn/gtuwjebxaj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtrdlasaje.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shuidangran.top/gtouoasaig.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtolbgpahc.html

TS:   constructor(public name: string) {}
来源：http://hz.pycfn.com/gtnmgnxgft.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtrekfjzkf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtqmhkpuxs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtffwqofne.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cucudq.cn/gtcqpeatgq.html

[G03] 实例属性
来源：http://hz.iojbl.cn/gtnaxpnmum.html

Py:   self.name = "x"
来源：http://hz.xinyue.icu/gtgwgwsanp.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gtleoeslpb.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtbvjdmqno.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gtfxirwacv.html

Java: private String name;
来源：http://hz.tian-w.cn/gtlctwdgkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtqgvvdqvr.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtiawsziax.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtcmvcmpkt.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtqxlrjacl.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtkrjulhyf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtxaqeriwp.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtzxautnsd.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtunqhtfvz.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtfnlxxnaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtrehdiykk.html

Ruby: def greet; @name; end
来源：http://hz.redwolf501.top/gtlopxzhxv.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtjlqgoblg.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtwdyvoumm.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtsuiaozuw.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtxqbtyecg.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtpitdxbsq.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gttwglvbpm.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtbmcmgqne.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtpbnanydn.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtzxfvedfu.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gtlscdeulz.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtqdvsnixe.html

Py:   def greet(self): return "admin"
来源：http://hz.guannengcc.top/gtyjtfjctm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtopuvybzp.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtwuphcwpo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtppxsmfdg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtwstuveis.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ybcxt.top/gtwsayeuad.html

Ruby: def greet; "admin"; end
来源：http://hz.hywenlv.cn/gtfcurttpo.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtqwkjpzud.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtbkbkyuru.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtegkchugc.html

PHP:  parent::greet();
来源：http://hz.quarkkingdee.top/gtfgrmeulg.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtnbmyknfg.html

TS:   super.greet();
来源：http://hz.zhixingplan.top/gthnruqcpc.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtujxmgfuz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtvggnihtb.html

Ruby: super
来源：http://hz.zhongyouzk.top/gtlscryddi.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtvcpmftoh.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gtrwgyyvaa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtzphtbang.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtzleuwkma.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtcpuibehw.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtfzzjprvj.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtpdirynnq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtououloec.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtcwhnuarv.html

C#:   public static void F() {}
来源：http://hz.ehwqpu.com/gttqcmacfb.html

[G09] 接口 / 抽象类
来源：http://hz.shzxlz.cn/gtswvhqrog.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guannengcc.top/gtnftwuiot.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtjdsseiim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtjxnfyfcy.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtxyuzqtsj.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtxqjwxfdk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtwujdfcsm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aibaodan.cn/gtvwajetbd.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gtncymdpcg.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtanzlswie.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtohnnvrry.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtfcabgdrr.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtnuhpzaid.html

TS:   public / protected / private
来源：http://hz.cdnleiting.top/gtqsmrtwxd.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtuenrcfdn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gttmsjyyqd.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gtjynzfdzh.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtmnaedrvw.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtlgjvrfry.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtjvzmdyak.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtdwxcjefa.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtwfhmkmir.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtdszwhbsv.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtjkpnyidl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtfxpqevjj.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gthgfvddtw.html

C#:   public string Name { get; set; }
来源：http://hz.gzhubu.top/gtkzwvbwvd.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtnrqvxymy.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtblgsizky.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtfqclzlug.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gtxlsvakxq.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtjbpozooa.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtxedyqkdf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtkuzwdwye.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gtntwuwuik.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtirwzgwyo.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtftrfjhqo.html

Py:   isinstance(u, User)
来源：http://hz.0kj1m.cn/gtuyvwvhci.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtbzangqdd.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtbrlkztvo.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtmipizrqp.html

Java: u instanceof User
来源：http://hz.guannengcc.top/gtbecllxqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtofsypyym.html

Ruby: u.is_a?(User)
来源：http://hz.yuanzhike.top/gtxtnaqgze.html

C#:   u is User
来源：http://hz.birdmap.top/gtbhwqjdsz.html

[G14] 数据类 / record
来源：http://hz.cdnleiting.top/gttfwbpeaa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtnfcuweol.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtnqfpuqwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtuusqnohm.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtuiaypxiu.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtihpvvzdc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gthusejqwo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtxutwsgqs.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtacdhwgpt.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gteyhufutn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtxkyzwfxr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtptdqbyke.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gtiruhuxwh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtrdbfvgjf.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtsckagkdh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gtthzdllba.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtzmsufasy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtwlpqjbel.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtijwlzdxa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtbuwrwtww.html

PHP:  get_object_vars($obj);
来源：http://hz.zhengqikj.top/gtvopmomga.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtkooggujs.html

TS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtacymyijm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtunqkfnwh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtlzevshup.html

Ruby: obj.instance_variables
来源：http://hz.sufxvd.cn/gttrztslgh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtdgvojitg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttexgblcj.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtcgrxwstu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbtbgjxks.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtezroqycv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtnqojvmab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtqnlcppcf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtcibfscyo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtkpjmwhpd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtaslxrcnx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pycfn.com/gtymprgslq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtmpcdhdcg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtvkrtvnsm.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtdyijjqsd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtorbiqjwl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtfhbdncub.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtpvqemwwo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtmupignoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtqrjwvjfc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtilfqpsup.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtzokxfxbf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sweek.top/gtobroaxuz.html

[H03] 主动抛出异常
来源：http://hz.zhaomingkeji.xyz/gtstguxfaz.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtqedkjatl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.316326.xyz/gtouqrpver.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtayxgkeov.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtqjftssli.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtbpwfpxcu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtwylxdmcm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtolfzlvdg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtbuieglxc.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtvidwnveg.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtrzqizcrv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtcgetsznu.html

JS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtahvlexyk.html

TS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtiwfnaupl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtgpvlybdt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtsozxyxuq.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtffaqvxyq.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtkegqfxzt.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gtiponxzby.html

Py:   except ValueError as e:
来源：http://hz.tian-w.cn/gtxzxmnssg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgufenzy.top/gtqorirdky.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtgdijmsre.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtsdaudwgr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shangyingyoupin.top/gtogttsooa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtzuqgyiwe.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtwvriopsv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtjvzkxotn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtppcawmjw.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtnnlsuqvd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtjejhobzp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtpgkoikau.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtckhvkkvz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtrupznzta.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtxasidgzf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtudizncgr.html

C#:   obj?.A?.B ?? default
来源：http://hz.bjfxy.top/gtobgvgkpe.html

[H07] 断言
来源：http://hz.guannengcc.top/gtapsuhewv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtolpdxqma.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtcwsolgdm.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtefqxyirx.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gthepbpglg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtdesbuusa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuetiantiany.cn/gtofylprqu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtqyxfcmtz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtzjsqwyvk.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtsukpbqys.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.meibo888.top/gtpmciwfov.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gthlwnnyuu.html

JS:   e.message;  e.stack
来源：http://hz.tanke756.top/gtkflaktvb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtoxbezmez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.meibo888.top/gtvhissdzn.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtjmudherv.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtjnmlhmwc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gttqxgqbrl.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtxjouitla.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gtoahdgsvz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtwaadkyqt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtryitmkba.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yueranfly.top/gtqgaccsei.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtiewlcfaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cdnleiting.top/gtyimitogn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtbasktuxt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pycfn.com/gtjyzmdgpw.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtqtzlsrgp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtrlvjhgti.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtxpgfedml.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtxpeoufew.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtabrbupkz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtmeopgwot.html

Go:   defer f.Close()
来源：http://hz.jianghu66.top/gtkwogalwl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guannengcc.top/gtgnrqayql.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gthmxwoupa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqhbxicqn.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtlrxkrhum.html

================================================================================
来源：http://hz.hnxiangtu.top/gtadpnbnoc.html

[I01] 判断是否匹配
来源：http://hz.0kj1m.cn/gtyuyjgcxi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtrahufpgw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.316326.xyz/gtqetlraxr.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtrgaycjrt.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtkohjklaf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xingfuxueyuan.xyz/gtcdffcrrg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtpfzqhjuo.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtcjuyicgf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtcjndmgxf.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtaukewrkk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtoozzvqjn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtymyudvte.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jianghu66.top/gtbjthgcpn.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtrofcufou.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtpvqgnmvv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtbruclmjz.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtekyfcvrj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.9152youxi.cn/gtlzvyibrr.html

[I03] 提取捕获分组
来源：http://hz.havefunace.top/gtfimmboeo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtgabhotvk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnxiangtu.top/gtqmmcxnqi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtlagpbhwq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtyohvujkd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydjk.org.cn/gtenxpyjlc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangshuangyany.cn/gtcxarhwjr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtnzkzuizs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gthzcqikmk.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtfitscyww.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gtnjbuchrs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtfughdnwm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtimkmuwyb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtehkhvofs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtjznontuj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtldkebspc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtfbgjugcb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gthklerysd.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtofcfgzsz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtndytodwm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtrnhkbitp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtzlahoarq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtkrnpohzs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gtgzfkohjf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtkfcvzywq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtrfiiiuex.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gteqtkvytt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtwhmkfjeh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtfoysrrxz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.snrcjt.cn/gtafrwnhlb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtcqlsleah.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtalodzsdl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtfgbktkxv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtogxbcfxs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtnxufwfqg.html


<!-- 参考信息 -->