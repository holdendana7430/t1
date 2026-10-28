代发 wailian999

================================================================================
来源：http://hz.0kj1m.cn/gtwxhghczk.html

G. 面向对象
来源：http://hz.mhx1999.top/gtntxvvmyq.html

================================================================================
来源：http://hz.chenzaomai.com/gtyfewdrrd.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtyqmlrpty.html

Py:   class User: pass
来源：http://hz.tian-w.cn/gtgdklgnuf.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtbyocitba.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtfengaogl.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtinwgezhc.html

Java: class User {}
来源：http://hz.jyoumei.cn/gtsoxpsgpc.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtnhmvabro.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtaurdilug.html

C#:   class User {}
来源：http://hz.zhiwuduotai.top/gtfezluxli.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtkaldpsgl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtwhztmccm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtceptbnqj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtbnyrpirz.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtnkpssxqq.html

Java: User(String name) { this.name = name; }
来源：http://hz.bjfxy.top/gtboqvtkay.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtkjllemsi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtkptcocbt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtunmkmpjr.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtrgetbhyj.html

Py:   self.name = "x"
来源：http://hz.jiagoushi.top/gtzsijwwlk.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtmstqaxyp.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtdsskolxg.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtpqrpxksy.html

Java: private String name;
来源：http://hz.hammf.cn/gtpndhtcmb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtxekodxnc.html

Ruby: @name = "x"
来源：http://hz.gotoacloud.top/gtacsmlwhz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sufxvd.cn/gtzcnqgpkf.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtjboynwgy.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtktelfvju.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gttwhdkdrm.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigufen.top/gtquoosfjb.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtoucqecgx.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtclmvvghh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtxqcnwajl.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtoxgkhxai.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtwghfcwtj.html

[G05] 继承
来源：http://hz.shangyingyoupin.top/gtxjnnscru.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtinksaobb.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gthuvguqbt.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtuehjdnuu.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtmeluhipo.html

Java: class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtykcqkxch.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gttjxcmavq.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtlbsakfue.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtunenrxed.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtpfpxstri.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtnivtrrcn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtupekbvoq.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gthqenynqh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtlcasmvfp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtvzaumuqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sufxvd.cn/gtmflzqteb.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtuoltewoy.html

C#:   public override string Greet() => "admin";
来源：http://hz.c1oappe.top/gtuupvuyun.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtmuigzlta.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtmzkwyjal.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtylartydn.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtejhihurm.html

TS:   super.greet();
来源：http://hz.ehwqpu.com/gttzhzeywg.html

Java: super.greet();
来源：http://hz.zhongyouzk.top/gtjwopkxxt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtyadwmgmh.html

Ruby: super
来源：http://hz.c1oappe.top/gtipupnqrz.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtebvzorsg.html

[G08] 静态方法与属性
来源：http://hz.svipenyu.cn/gtlyjrhddh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtgyrwnfhg.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtforilkdq.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtexffdbbq.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtusrkumrl.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtoabhnkej.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxuanxn.top/gtejfagbde.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gtaguwyjlc.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtzvdofvsp.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtdbmmhlpv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtlvtffbxj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cashguo.top/gtulyhyxrw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtshmcnzvg.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtpvxkpbpz.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtmwljawym.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtohixxoel.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gtelzwdzln.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtjxwqukxh.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtsrjgqcwh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtumiftfie.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtfsslbrmm.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gttclqerty.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtbyjciqdf.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtflgxymzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tian-w.cn/gtnroxyyht.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gtkxgaafos.html

C#:   public / protected / private / internal
来源：http://hz.fzhhl.top/gtopgfqkib.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtvefyunzk.html

Py:   @property 与 @x.setter
来源：http://hz.jqgufenzy.top/gtlfnxabvf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gthobjxfxm.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtdhhrozym.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtcirxyadb.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtwzldktqt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtjapslohb.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtsttsybuk.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtnizicpst.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtorfacqsm.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gtpwuwxhqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtggyufzvo.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtaxbsgeft.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtgxrpdrbc.html

Java: @Override public String toString() { return name; }
来源：http://hz.cqqwz.cn/gtwlsnvhqj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtrentroei.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtyppigdii.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtcwwlmewf.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtmaojqfxn.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtzhjqbrly.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gthdpvfjyu.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtnayzqysu.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtausjiwzj.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtdpywlyqn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gtkszlyvsw.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtbekpbhuj.html

C#:   u is User
来源：http://hz.yj20258888.top/gtcwxzyztg.html

[G14] 数据类 / record
来源：http://hz.tanke756.top/gtmgcreant.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuxming.cn/gtwnruhxvm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtsxdwpavs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtxwnpqzyo.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtdftuutdg.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtlqazqsty.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gthdzoplwf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtkvmltsmh.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gttzaiglso.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtiwfppgsz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtsgheilvr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gtynfjklau.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtebbctacw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gttbhliosc.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtugkdhpip.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daria6918.cn/gtmxyfxflp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtnrbxfdkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtlvlhfoyv.html

[G16] 对象转数组 / 字典
来源：http://hz.hnqzz.top/gttpmyabbx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtexchhnmr.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtykvgznss.html

JS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtganjbwls.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtdauecdzp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xingfuxueyuan.xyz/gtcoejbede.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtggtmtjrs.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gtvqovpzhp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtsmnowqrq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdqpjghhq.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtfegasvvr.html

================================================================================
来源：http://hz.aibaodan.cn/gtwzomdkcm.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtwipwgpbv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cdnleiting.top/gtfdxcqyxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxuanxn.top/gtiqvhpfnx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtdvmiwkyy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gthkzeqpzr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtetsjcwcr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guannengcc.top/gtwvxeeetz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtdefedfmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gtkrclilzx.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtxvsbebbc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gthqqfzmzb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gthvkvdidg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gttuckalyc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtnukdfmlu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtejmpnqam.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cdnleiting.top/gtryuxdbuc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gtoskavwrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtrmxfarsy.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtozarbnsy.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgufenzy.top/gtcyetmhck.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtmhjnhcwz.html

JS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtxfemojnv.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtoabksmxt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtqiwnzqqb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtwjbmpmvr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtsnxvziad.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtmbkofbdl.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtscnhdwhc.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gthtjpxojf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtwgaqesxr.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtzsogpvuj.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gteieueuwl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtcdcemhri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtbkedrnoc.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtuhwrbtwl.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtnqxjszeu.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtgvqlnuvg.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtijtzkwbh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shzxlz.cn/gtyujsgsxh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtrswvugtw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtittsywjd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtvbltquqo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gteifoanyq.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gteyjwzjhc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yueranfly.top/gtgggsowzv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtnfegvhnw.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtvdjsnqnv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtrewmxnem.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtbbokketx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhixingplan.top/gtvyvvmkls.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtqnsaznjb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtkfybizgf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtuciknecb.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtonyhpwlv.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtsvccnvno.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shuidangran.top/gtfbmvfvup.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtkuthduzr.html

JS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtznfxuiip.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtseijxbta.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtmagdhioa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtvapuoxrm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtmqumefiq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtrufzzdjs.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtibllrsrb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtjevnieiw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtzcuvscpq.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtzgfrwpkt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtwnfchmlg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtmhmoanih.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtxiiwchzo.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gteseozoyh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtqrqkaxae.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtjqxxrrrv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yangfankeji.com/gtkpejcanj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gttopfauyn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtjjwmurep.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gthjnyoniv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtdowgwjeb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daxiang520.top/gtfsqydxzr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gtjlvjxlyo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtsotjgwng.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtphtbffbk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtzdogeebq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtquvoymng.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtquwtbfto.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtknldntyw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtzdbvngok.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtowuwyiup.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgufenzy.top/gtgicbvwxu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtfwomcapo.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwwgwcyvc.html

I. 正则表达式
来源：http://hz.yj20258.top/gtmdrfcbqc.html

================================================================================
来源：http://hz.pycfn.com/gtvmseyden.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gthayzuxae.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtbxakigiy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtkzmtchrl.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtqbessgzo.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtwquxqwwk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtnwusjkfd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtctkdubzw.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gtfgrwecov.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtwxjjldts.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gtacngkpjp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtpdxbntzi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sxryk.cn/gtpcqcgprh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtovibdoru.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtzlcfwrlc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtupzcevkb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtfaduxnrp.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtokbvppkh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtahzwpbrg.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtwbqdzpbe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtvmjpekwp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtpkcqemdp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtrhnmncvz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtxhwbkknl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daxiang520.top/gtazqoxwlf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtdgtujsxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yanxiufei.cn/gtygqbizjw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gtlvjrnmxl.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtahbjtkuz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtagltsqbj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gteoefgino.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gttobnoewa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtqxsdryww.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtqfvjefmn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtojrxnchf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtrlcpusou.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtozwwzuzp.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtbhxepiss.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhengqikj.top/gtdaqkzwvs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtdxsmtttp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtltvifkqx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtxihabjkd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtiboibboq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yonumen.top/gtnskfggjn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtiogvdngg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtlacbvmno.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtdsoixikj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtcfhohyaj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zdqjudy.top/gtuwkphnlh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtjdromtzo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtedhnifqb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtxztssskd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xingfuxueyuan.xyz/gtukrrmyvu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtgxnriyso.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtddflgvvw.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtzwkcrrfu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtxrifckld.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtaodyelxv.html


<!-- 参考信息 -->