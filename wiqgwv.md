代发 wailian999

[G02] 构造函数
来源：http://hz.havefunace.top/gtrodwptov.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gtkhxzctlm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtlmpmovhz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gthsgpxgxr.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtdcwlpscw.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtmgglxvyy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtyifwodmf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtktvaosiu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtcuphihgd.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtbldxwzsp.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtqotfyunz.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtnrpojryb.html

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtmcrxkctj.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtbfbegsdf.html

Java: private String name;
来源：http://hz.cucudq.cn/gttzfpibyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ppjwa.cn/gtjabcdruv.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtckfbxgdw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtvxxqwywf.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtbolidpkb.html

Py:   def greet(self): return self.name
来源：http://hz.zycfv.cn/gtvplnrmby.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtewrvgitb.html

JS:   greet() { return this.name; }
来源：http://hz.birdmap.top/gtyqkakjzg.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtbxmjvlqo.html

Java: String greet() { return name; }
来源：http://hz.meibo888.top/gtwpjxivza.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gtourdkjed.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtkjxrjegp.html

C#:   public string Greet() => Name;
来源：http://hz.tian-w.cn/gtgzxsacxm.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtowatuenj.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtajomobgo.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtlnreahap.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gthlgddzzc.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtpcjzreqi.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtbdpychni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gteqfzeuru.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtmqojgcwt.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtsjbpnglr.html

[G06] 重写方法
来源：http://hz.yuxming.cn/gtdzugtwpt.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtfsflilkt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtysanazuv.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gttjpuxnct.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtybsvztwi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtxyxvmqet.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtizmxmkhy.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtwyvgmgxx.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtzycwcgyn.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtlgfaogow.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtzefqvndq.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gthewddofm.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtnycyhfhg.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtjpsrvubp.html

Java: super.greet();
来源：http://hz.nanxuanxn.top/gtldxgccdi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtnyffpvpx.html

Ruby: super
来源：http://hz.jianghu66.top/gtegdnvvrj.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtrfjwruna.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtgyjmvjlr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gthczgowbi.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtjganwsug.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtbywyzfmf.html

TS:   static f(): void {}
来源：http://hz.xziqi.cn/gtzbenkbnl.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtnvujjjxr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtnwzdgbgk.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gttwbrbusu.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtjgksxpgc.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gteyfgiqan.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtryikhntb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtltzgrckc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pycfn.com/gtgultykfm.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtzrohzclp.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtesjwfked.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtstiupmar.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gtqabipimi.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtrhenrlxa.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtmxtkizod.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtmmcslahz.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtelytkucg.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtwhhdxabm.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtfnhvztcq.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtqsburhtk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gteymwnmsy.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtfglfndgw.html

C#:   public / protected / private / internal
来源：http://hz.cqqwz.cn/gtpksjmbmv.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gthzhxnedl.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtjtxuukui.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pycfn.com/gtzioxddkp.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtpbhsrsxd.html

TS:   get name(): string { return this._name; }
来源：http://hz.quarkkingdee.top/gtsyngpbge.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtpejmrrbv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtamyyezpz.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtktsfwsoj.html

C#:   public string Name { get; set; }
来源：http://hz.nanxuanxn.top/gtvhhrjmah.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtlrgzuctz.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtjlazxwsv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtcxthrgsa.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtdbatsqlt.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtpbensdfs.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtxrkdhnrw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtmrizaprz.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtmbgmxrxf.html

C#:   public override string ToString() => Name;
来源：http://hz.svipenyu.cn/gtnoccsxxy.html

[G13] 判断对象类型
来源：http://hz.nanxinkj.top/gtripmvhgv.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtlkgicyfa.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtgvksrhrl.html

JS:   u instanceof User
来源：http://hz.yongpay.top/gtxayzuejp.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtjdysknoc.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtrgzfmrck.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtppsyoewd.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtvsrqcnix.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtpriilpel.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtrwcunboy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtoenoxldk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtbcrnxkci.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtlwrqvqsh.html

TS:   type User = { name: string; age: number };
来源：http://hz.feifeiyinyue.top/gtnltebwvo.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtwxkjtfmg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtzleygdal.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtwdlgskor.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtkylxiiwr.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtoysxwirj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtwgykjexz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtgbfxozbg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zdqjudy.top/gtxulxunzv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtfyniqlxk.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtrvsmqkla.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtmzfjwoyd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtqqhobkcw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtxfaptqdx.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtpewbvsub.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtqdmjahta.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtvzrewznj.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtewjcomaz.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtqakpashm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtoczlivds.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtvyptvnog.html

Ruby: obj.instance_variables
来源：http://hz.hywenlv.cn/gtsvrqjhqv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gttmavazua.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkxqvyjys.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtxzzgnjzl.html

================================================================================
来源：http://hz.xuanzx.com/gtgzwngbif.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtbmitykok.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnqzz.top/gtjokkdahp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtaglefbbc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtsxebkwoi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cashguo.top/gtruzedhof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtoovvnclj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtrbfgqhxm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtcdvoesaf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtwcyhmcue.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtimmapgci.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtckkqprls.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtccnqiyqx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtoaxpuezg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtfmmehqdy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtadsqzglm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtwfgkbkfk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gthwpuokjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtvbemqqrj.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gthdzmofyz.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtwzaxzazv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtjketvuej.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gttvzkjkah.html

TS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtemfvyccd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtxtzalxwh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gtbfgbejob.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtyrrjjysm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gttzcbkptb.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtqlwnizvk.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtmhhvrnqr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtskrjsytv.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtpurcdelm.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtvuacpxwl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtjbtvwghw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shuidangran.top/gtmidwirvr.html

Ruby: class MyError < StandardError; end
来源：http://hz.hongshengwenyu.top/gtapwqnuvb.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtmxgmegbn.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtepndxrtw.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtplvgvsra.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gtsljfnmdh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtutypxrqw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtilsdlqyi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gtiedqlrof.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtixhuouof.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gthqjfbpah.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtgemwijwl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtlddqimno.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtvycxwykm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gtqalqheuc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtoalojpii.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtmnezjmcn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtkdvisceq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtnjidytwu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtzzbtuxse.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtgmgxqgip.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtweyshajs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtrrykftjn.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtfmfwtnnd.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtaewzdnol.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtlskiifti.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtocczlcol.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtimrgctzv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtsssnbcsa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gttkkwbyfc.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtkonzuqkn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtiefilwyd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtmqaotmsk.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtoebqevqt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtpshmcauz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gttniizszk.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtjvryuqmd.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtadozulna.html

C#:   e.Message;  e.StackTrace
来源：http://hz.iojbl.cn/gtjggbbeuk.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gthrhkrslt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gtfrxitpkl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtixxtvkwh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtvhzlycuq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tanke756.top/gtsvlhheft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtlclzptcx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtffioxmog.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtsduuyegy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtrqlzjrsi.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtkvmwkyeg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xinyue.icu/gthhhuwwhx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.redwolf501.top/gtbngdskfw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtduodgprb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtsnboeznl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yonumen.top/gtroynjvpz.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtucnnpypk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtqueofrgx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sxryk.cn/gtmlosfvnd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkyfpzscy.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtiwgkockp.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvkrhfaud.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtbejoanoi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hysaishi.cn/gtnqftalfr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtcoijxwpn.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtpzsklyyw.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gthijrwuek.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtmqrhvlah.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtjdiuykhd.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtfutairdy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtcojqndoy.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtlsjgxxpy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtozfhzzhp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtblpdvrbf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnxiangtu.top/gtoruhxgsd.html

TS:   s.match(/\d+/g)
来源：http://hz.yongpay.top/gtpwacyexp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gttemyiauj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daria6918.cn/gthnmqumhh.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtxupbmakf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtzrcgrmnd.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtyczvabwz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.9152youxi.cn/gtzdluvvvl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtfzemssou.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtmxjzseqj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gteouilpsn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtjkafwrkn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtsntrwoqd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtimefjymx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtcqcqxrdy.html

[I04] 正则替换
来源：http://hz.tanke756.top/gteuxtaixt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtkvuaprqd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtjcvvifxs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtobtvxbfk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtlfwajlrh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cheryme.top/gtxrbudbio.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gtlbusmpsb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtkngrndfe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtyofsjxlz.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtteeaztqj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtkzipvaxl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtjyajoawo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtpcpchifc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtatullsnk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtxqhbrpxv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tianlin.xyz/gtvbajnhlw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtthpnecal.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gthacprlmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtxsnxonye.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtjxdfjphh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yangfankeji.com/gtudkqtwxp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtgakbfveu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtcfufwpds.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtzecaxpkh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtpskdexoa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gttqctrsxj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtbnmkucov.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gtnavygpbq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtzlfqgrqg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fengsongda.top/gtuwunvert.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxuanxn.top/gtqhjeduvi.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtilxuxitf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtvnkkjdcd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtmxddbviu.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtpgboqycj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtshudkrag.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtrwphekig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gttjdlaopy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtgijjgyhz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtvkpadtmg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtkhxymivy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtbrxuddif.html


<!-- 参考信息 -->