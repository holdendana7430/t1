代发 wailian999

Java: class User {}
来源：http://hz.pycfn.com/gtuuxtcvoy.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gthqpibugw.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtmziibart.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtrxpnhuzz.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtcchikybx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.meibo888.top/gtuazkkxsu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtqhbveeng.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtbznboenn.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gttffqvand.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtjxufstdt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gtcwpguvhv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtqqwhappm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtfribvqci.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gtfwcednyf.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtufayozks.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtxgoamqyt.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtweyvxuio.html

TS:   name: string = "x";
来源：http://hz.jinghuilouyu.cn/gtgjhhuenk.html

Java: private String name;
来源：http://hz.yj202588.top/gtdwalgbyh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtskhbnrnk.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtwwgthkcu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtuxbbrgoi.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtckuxvvne.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtefkfnuhq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtkxhjgxxu.html

JS:   greet() { return this.name; }
来源：http://hz.hnqzz.top/gthhmbgijp.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtgkvifqod.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtoradatqg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtmnfombve.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtfdmxnhgc.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gthxvmxyft.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtikpryiyk.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtiusdyttm.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtdlxbfhej.html

JS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gttpdinogq.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtjrcmncta.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtvdebvuwq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtlchvejrk.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtcooszypl.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtxohwhlmr.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtrmgjzwsp.html

Py:   def greet(self): return "admin"
来源：http://hz.shangyingyoupin.top/gthjbhhbrh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtafnnreli.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtcahphwmb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtzgjxboui.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gtwitdrtak.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtokbbqsac.html

Ruby: def greet; "admin"; end
来源：http://hz.0kj1m.cn/gtdlbkizea.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtqtaaufmw.html

[G07] 调用父类方法
来源：http://hz.redwolf501.top/gtbgtzhmlj.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtwwtfsiaw.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtkcsteeba.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtdaopnmsa.html

TS:   super.greet();
来源：http://hz.smart0.xyz/gtbahbxyxl.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtczjeabin.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtetlqgcpy.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtfdnkofbx.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtwfgfqvej.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtupmrkmpl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtmdbrolrn.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtfmhkuqaq.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtmwzolrdn.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtoxunwtqv.html

Java: static void f() {}
来源：http://hz.cdnleiting.top/gtwcrgktsx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtnghpfeyb.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtzcbmdjzj.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gttlwwdpcy.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtcnnkcjnn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hywenlv.cn/gttllenrrp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ppjwa.cn/gtatknynuq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtefvuidyy.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtkhqbuqip.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtskauaodj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gtzkeeirut.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtegobjyuz.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtqjocjxee.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtugvsudma.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtgmmgevti.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtvdxlofgj.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtwpbafgst.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtcravcgeu.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtpzibimgk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gtneyomlbr.html

Ruby: public / protected / private
来源：http://hz.ydzc1.top/gtvxyzpyep.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtstconbdn.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtyninbixu.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtdnmsjipj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtsuejgner.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gtghvsugug.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtprexeick.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtivjanmpo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtdyqewblb.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtcqjhrqkr.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtysgxrdvj.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtinbodplc.html

Py:   def __str__(self): return self.name
来源：http://hz.daxiang520.top/gtoassakyp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtzicfuwzi.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtkvryzklc.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtqbdscncg.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtbfgaitsx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtgxxkziai.html

Ruby: def to_s; @name; end
来源：http://hz.tian-w.cn/gtdtgtinsf.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtshzjyfzs.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gturmpycgg.html

Py:   isinstance(u, User)
来源：http://hz.yonumen.top/gtmooeuwom.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtbylwsenl.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtrbarkkrs.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gteypjbzyu.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gteqwvmceh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtcfbaqvls.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtdsvtjifc.html

C#:   u is User
来源：http://hz.jianghu66.top/gtnuetpirp.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtjfnnlzbk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gttvfgahpx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gttcrqumlv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtqlogyhfc.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtfboukdci.html

Java: record User(String name, int age) {}
来源：http://hz.yongpay.top/gtepzwmyjk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtdukedglp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxinkj.top/gtugkqfqve.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtjagghukf.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtnhsoovrz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cqqwz.cn/gtvnhltiiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtswsliyuk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gttjepbvmg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gttivpyrwz.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gtatuqtvve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtkjcswqke.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtnmdsdhlj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtzqbojekc.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtqyfgditz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtfccijqjs.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtvbcwcnip.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtumjcwvjv.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gthkhoizoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtuceiujbs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtkjfckmbo.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtyzbmlvqu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtsdoklazn.html

================================================================================
来源：http://hz.yonumen.top/gtywbercpd.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtlhhaltqx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxhqnckxq.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtnajboffw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtzgvyhtko.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtgqfmugtm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtuyliqpqp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtqkgkfrth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aizwys.cn/gtxqpdzaru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ehwqpu.com/gtvwhakmnk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtvslxmjfl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gtytoaatss.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtifjcqxpp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.feifeiyinyue.top/gtsgqbzuja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtfedyfrqb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtssabrwxe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtrhhlssus.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtolmujrbj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtzindhhjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gtomezsbgw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhongyouzk.top/gtpscnjjql.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtzzirujfm.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtvtvrqutg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtnwsdypuh.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtmcxalzxb.html

TS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtskvwozdf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtzbwocotz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtscyelccj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtdudfmjgu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtczllubsx.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtvgekrxoo.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gtpdbusirp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtmdrrdime.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtzzczhflq.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtbjqdjrtp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtbcdezvyw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuanzhike.top/gtcagetafy.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnxiangtu.top/gtakotimdj.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtayubdfxj.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtxcyaccuy.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtlkrwmlur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtxtqrvdtd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtpgdummeb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtrofksjwm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtxdflfpwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtlfipfjmf.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtufylhqpd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtapohpinm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.c1oappe.top/gtaqiuefep.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gtiurzgbvr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtqvjgkwgp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtyjjvvtbf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtyihdxacg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cqqwz.cn/gtpgluvxtc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sweek.top/gtsqmcwfbv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtxofpbyvt.html

C#:   obj?.A?.B ?? default
来源：http://hz.hywenlv.cn/gtuqwqltre.html

[H07] 断言
来源：http://hz.hongshengwenyu.top/gtwkudnkfp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtjyjlemtj.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtczhjsmng.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtlvqmcepi.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtohagyttp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtasldovgc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtfaignokf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gtclbfreec.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gthdgcamof.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtztcbdtje.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtawzjyiut.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtmsbnzlzl.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gtweqqlolq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nwbrower.top/gtjlxvunvt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shuidangran.top/gthykevqxr.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtitmgxkwe.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtleppogxa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtbvhfnsiy.html

[H09] 带错误码的异常
来源：http://hz.chenjidiqi.icu/gthrkqgwcz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtxefbuovq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yangfankeji.com/gtrnjibcbi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258.top/gtoaksxxuj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtjwbyicmd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pycfn.com/gtagkmhpfp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtbbunrzqw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.smart0.xyz/gtsrzoljxe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtlbkgippk.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtnmighkwt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtedmwbedz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtmiwgkhwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtwxyjsmjf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtmyqbjwqk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtyylqglke.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtocxurkqk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtnuejmoja.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtbbnomgur.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthcmcrhcz.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtrlpbudgs.html

================================================================================
来源：http://hz.mhx1999.top/gtygctcucz.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtshdgtdsv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtcshnrpul.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtbfyahgyo.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtkiesifcw.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtjcitxwpj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtflpjuuii.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtsdevhqai.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtiyiaxvzv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtdmprvnsy.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtylmzibov.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtyfqynsfv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydjk.org.cn/gtgbqkvfgi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtficlknnm.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtjuivlhhx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtbunaxojt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xziqi.cn/gteasjbcrt.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtfahompml.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxinkj.top/gtbzzwiyjk.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtbfmmvtmw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtxpxhlasu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtbpenvxii.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gtggoqggii.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fengsongda.top/gtfmbnkqca.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtrvhiuuzq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gogol.net.cn/gtstmtvkyr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cdnleiting.top/gtgnjbxtlj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hysaishi.cn/gtwljbagzx.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtuoqymcij.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtoustkpkt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtzbalbrsu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtsrmwjwzd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtfuwijygo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtclvkqyef.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtfiwtdmne.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yanxiufei.cn/gtiflpmnkl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtfdlwtqkc.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gthldtvqlu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtaoaeuhqd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtnuweejsy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtzxbppoff.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtqjqphxqo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtzifsoqnk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtjuyzfsch.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtehjvvcck.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtbnzxlvlf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gaohongyu789.top/gtewrjqcsj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtxgzonwks.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtinlefvuk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtoexhggvb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtgrqghsla.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gtxlpruiqm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtmkgpjwbq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gthqkgvruq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gthiawwnsx.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gthmnhepff.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gteugnnzjh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gthffyobew.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtizwrhdlw.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtrghqkmha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xziqi.cn/gtrmyblyjo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtdkuvjmrf.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtcmauaghc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtvmwcmrgg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gtctegobhs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gttynyjrgy.html


<!-- 参考信息 -->