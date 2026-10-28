代发 wailian999

Py:   class User: pass
来源：http://hz.yongpay.top/gtswbijnok.html

PHP:  class User {}
来源：http://hz.xylfe.cn/gtkevnxntl.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtpxaxcqwr.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gtkulurvun.html

Java: class User {}
来源：http://hz.pycfn.com/gtcdvolrlt.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtwbxwbveu.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtxpbmggjv.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtywcupwld.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtleujslyo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtknysubxc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtlhbowjkm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.birdmap.top/gtckdqvjie.html

TS:   constructor(public name: string) {}
来源：http://hz.mhx1999.top/gtvcxzmmji.html

Java: User(String name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtuvqbonbf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sufxvd.cn/gttrxzxpcf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gthzzkjnkj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jlsjyb.cn/gtyuduuarv.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtjihjtpbn.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtcqbvrhnv.html

PHP:  public string $name = "x";
来源：http://hz.snrcjt.cn/gtgcngkivs.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtfdhyhwks.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gteobznagw.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtstasdvrs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtryqfrihp.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtzpbzvokp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtqntpoqsb.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtqlyudlqc.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gthznwgqbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtdqiypqdp.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtnmkruqqz.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtpwqcsxnc.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtgmtvcwne.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtabmmebiu.html

Ruby: def greet; @name; end
来源：http://hz.wangshuangyany.cn/gtykmtgzke.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtyvulseuk.html

[G05] 继承
来源：http://hz.iojbl.cn/gtunhitrqj.html

Py:   class Admin(User): pass
来源：http://hz.wangdashe.top/gthwsyrxmz.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtvgetcjdz.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtqxxxtfjp.html

TS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtqrimyjfx.html

Java: class Admin extends User {}
来源：http://hz.ppjwa.cn/gtbesmglhs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gtdmxjawha.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtrepnduen.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtarvzfsbq.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtzifdpsjj.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtpqszfzmt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtolukfkzz.html

JS:   greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtblufjzue.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gturhqbgjz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtvsijhshs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtgbbauaqk.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtoxgttkux.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtbyqgwutf.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtpgzoqcaz.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtqwfhutat.html

PHP:  parent::greet();
来源：http://hz.sweek.top/gtptcmlonj.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtqnpypahn.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gttuswvlik.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtpozruxjy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.bjfxy.top/gtadjyckjm.html

Ruby: super
来源：http://hz.jiagoushi.top/gtibhybmis.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtfdgnlyfa.html

[G08] 静态方法与属性
来源：http://hz.iojbl.cn/gtommlqymv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtefxaqqye.html

PHP:  public static function f() {}
来源：http://hz.hnqzz.top/gtbhzvdvbw.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gtmyudyltz.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gtcncwjcfv.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtioahqyjy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuanzx.com/gthnmfccnj.html

Ruby: def self.f; end
来源：http://hz.jqgfzy.top/gtfykekygs.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtchmjcfib.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtkbwqzopb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtsgtbpbfy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gteeimjxfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtmjidkkqi.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gttkloufcx.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtdtcsdikf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxuanxn.top/gtmrbmihid.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gtakbsxvyy.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtbmjmqdyi.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtkjszleuu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.meibo888.top/gtjbjkilso.html

PHP:  public / protected / private
来源：http://hz.nwbrower.top/gtiaftbeyg.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtknwjbify.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtqoihrqbx.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtjzqoffxx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgfzy.top/gtbstszhrl.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtgkvvzahi.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtxtcfsngv.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtwrmbexuf.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtrryaszzs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtdadpxorx.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtfsidvtvm.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuetiantiany.cn/gtxjexouhi.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtmvfjugdd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtodvrgmgd.html

Ruby: attr_accessor :name
来源：http://hz.zhoulong.xyz/gtcfjmwnyo.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtzvuhugqk.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtvfrlwcxo.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtaedbuuxx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtkkoicyqs.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtqnggqtvq.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtcggmedhi.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtgvcivbxb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtcaojgzkq.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtexnlrabp.html

C#:   public override string ToString() => Name;
来源：http://hz.daxiang520.top/gtsxpsnuct.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtksmnvxfs.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtfcvzityo.html

PHP:  $u instanceof User
来源：http://hz.tanke756.top/gtsiiegeak.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtledrknzr.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gttmeryqys.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtqbkbfftz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtfiycwvwh.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtpigiwzhh.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtvdlnesii.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtukfuksoe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yueranfly.top/gtzphqthki.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtaesgkqnn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gttgtnmsck.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtubtksibr.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtsuxcqxeo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtvpbcgsrn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtviyqcpdn.html

C#:   record User(string Name, int Age);
来源：http://hz.gaohongyu789.top/gtfsgaspna.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtdagwxufb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gthzzxupzy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtczhslstv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sweek.top/gtlxjytejp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtjcjjtzpp.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtvnbvpghs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtliecvgee.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtljgwmxeo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtborrhozv.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtmohkaoyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtjofqkyyk.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtjijucyhf.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtfqwhabxe.html

TS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtxxylasjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtxdtfjlnt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtaiycjfzq.html

Ruby: obj.instance_variables
来源：http://hz.dashuyun.cn/gtknpxhonc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtqcsbotii.html

================================================================================
来源：http://hz.yonumen.top/gtseqsbatq.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtaescomqt.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmmtbmypk.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtezrdgbrv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtavnpmckf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtfgbzdeyl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtjmfovubb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj202588.top/gtsdghzytf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtwmegwchz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtchgmnrit.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtdzdplata.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtqiegsibs.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtoukqzyyn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtmuukuuvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtjamacraz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gthtlhrorc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtqvurotrl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtndzgdvoa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhixingplan.top/gthfothwsi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtaubcvwap.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtimbkqddm.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtstbkwpab.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtoitxckef.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtjucfqjqg.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtfzgxmyao.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtujlgzasb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gthantoqfx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtdejqlxuj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtfykvmryt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtiotwqxjw.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gthbxijxqn.html

Py:   class MyError(Exception): pass
来源：http://hz.hongshengwenyu.top/gtigpjilad.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cucudq.cn/gtpmlsmgeu.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtpzrniyvh.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtborikvuw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtfblvthmf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gtieuarztw.html

Ruby: class MyError < StandardError; end
来源：http://hz.guowangkeji.top/gtowaberyg.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gttbwcghhg.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtgkmrymwa.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtmovngbhm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtcpqulgwx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtttbrbint.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtewxfudll.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gogol.net.cn/gthnvhmuhi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtxylmkmrp.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtmgznbqis.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtdcpxtsid.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtzjlhjvde.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtafrrymmq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtnvryzpyf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtwfjjdoxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtkyopgadp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.andypj.xyz/gtvsbbkuxr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hammf.cn/gtpfrjbvsg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtwqqlyfyj.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtqvpnoxxm.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtqqnvwxwi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gtcyflhomw.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtfzmcmkuk.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtrodtdkln.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtvltusejh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtwochckjd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtgzhoacqm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtnjdfzrcm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtkxahtvpn.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtrhdkgrgq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gttfhanjzp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnxiangtu.top/gtfxvjbvbc.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtlbiexkww.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sufxvd.cn/gtyacjkflg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtbdpgkric.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gtflzmlhoy.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtrnqtdkft.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gttrrqtmhw.html

[H09] 带错误码的异常
来源：http://hz.fengsongda.top/gtcufvaukf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yvedp.cn/gttaiyvsyu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtdlgqglcm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtobqzfcay.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtqbgnqpsr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gttkumtium.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtgsnooqvp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtcnskrdtu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gttovkmgda.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtrhhgnxph.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtnjcuvcgh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtidbymjuy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtfusyyvzl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtidshkagr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtgqwcsthq.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gteswntvxj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.havefunace.top/gtioyphlna.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtmqajolqr.html

================================================================================
来源：http://hz.shzxlz.cn/gtgcmmjgkz.html

I. 正则表达式
来源：http://hz.sweek.top/gtcwudnowx.html

================================================================================
来源：http://hz.daria6918.cn/gtthyjtvxm.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gthmxpeayb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtfdrhnbqy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gthmramhlw.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtwjkwbjpn.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtzhvygpnq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cdnleiting.top/gtxazwvwxs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtjsuialjd.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtmnqkwhhd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtyaazzmru.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtcuepfztb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yueranfly.top/gtwpsouzlo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtipjmzbbh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenlongwang.top/gtsidjklhi.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtfunogkua.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtucskezpw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtakgbpfde.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtwykgekdt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ppjwa.cn/gtwrngsjpc.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtrhlmepag.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtigzsxyax.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtrvicfeyd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtrsnoetzn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gtducvlves.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gttsrudhsg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gtsrccjlcc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtdjqaswls.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtqttarqpa.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtbbxrgkkc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258888.top/gtaxvtzmov.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtynnqssdj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtibshavhl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtuhfmvoxk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gzhubu.top/gtvtqwzzbl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtnhlqupwt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtjfmuwxkh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cheryme.top/gtyvbaaplu.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtkdhsodbn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtjohkafur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtfjfkcchy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtyvtalpih.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gttkkcfucy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtxanfmqpn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtocthqcwb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtjzxojhnl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtbbaxrvsm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yanxiufei.cn/gtnfdnfmkk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtheyddicq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gtxjaasjrb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtowjeirgs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtawmxskeg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtzkcesmhq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtoeifihqc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jyoumei.cn/gtewchaobm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtkaevdsob.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhoulong.xyz/gtpdbsrorf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtpmctpztq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gttsrtcrhn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gteoevpfwy.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtgofluoud.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtdhrjllom.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtcdjejhxr.html


<!-- 参考信息 -->