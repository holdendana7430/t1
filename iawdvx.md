代发 wailian999

[G02] 构造函数
来源：http://hz.yj20258888.top/gtphsvbsfh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtrclxxkie.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtkgxzcxbx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnqzz.top/gttvcpbvvc.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gthdlznbal.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtfkolzlsh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtcajgwyps.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtvkdosadp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtonrjmhxo.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtgponofau.html

Py:   self.name = "x"
来源：http://hz.cqqwz.cn/gtqgoxtnkl.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gtftzvfovf.html

JS:   this.name = "x";
来源：http://hz.meibo888.top/gtuofrngms.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtghvatxoh.html

Java: private String name;
来源：http://hz.meibo888.top/gtcwwyijix.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtdnmwmevk.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtetubmchv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtvfbxhahv.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtrtnzdeuq.html

Py:   def greet(self): return self.name
来源：http://hz.jyoumei.cn/gtpetbwtsz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtbvejdbqu.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtetfnyyvp.html

TS:   greet(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtercuwcqn.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtdyhnocgg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtipexegho.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gthssqtoyp.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtszclsdxf.html

[G05] 继承
来源：http://hz.bjfxy.top/gtjbpbcqql.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtlyuaewan.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtiaglwfew.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gttgihyvbj.html

TS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtrmpdcgih.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtdrdgplsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtdjqptxcz.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gteqvnbtnx.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtdrdbcnmc.html

[G06] 重写方法
来源：http://hz.nanxinkj.top/gtghvfvcyj.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtsyyzahap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtbijbwdfm.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtfimvrzzv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtnggzgtie.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtysgwjrbr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ybcxt.top/gtkrtuwhbs.html

Ruby: def greet; "admin"; end
来源：http://hz.gaohongyu789.top/gtrisjcani.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtcfqwgxdo.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtwugloplz.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtkuswfofu.html

PHP:  parent::greet();
来源：http://hz.52xcode.cn/gtevgcofrs.html

JS:   super.greet();
来源：http://hz.iojbl.cn/gtbvdcsful.html

TS:   super.greet();
来源：http://hz.dianchejie.cn/gtrlprqhsl.html

Java: super.greet();
来源：http://hz.yonumen.top/gthtsalvdc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.52xcode.cn/gtsbfbxpey.html

Ruby: super
来源：http://hz.meibo888.top/gtvpibpxet.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtgcthuzar.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtkfudmcej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtvmokmmiw.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtrytgfanf.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtstumkerd.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtghwsxwrd.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtevfqlggt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtjerjswzq.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtoamchmrq.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtqikwjfxy.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtykvokshu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtnmfxqpnn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xinyue.icu/gtpztdqfka.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtsirmwmkw.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtqyuornhi.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtbxxardqf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtxwiwonxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtvwuynifz.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtbipiwmam.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtqbrmmlhw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtxgbsmvie.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gtefxczmjj.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtqlxaarhz.html

TS:   public / protected / private
来源：http://hz.yonumen.top/gtrkztzxlv.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtmcupnirf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtkfyttujm.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gtozyucljl.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtclysmxbg.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtcdmqyaor.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtnatoinfj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtmemhdaek.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtpoqonggq.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtyewgyzxy.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtyevgkltl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtpqprjhoo.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtbasexvnc.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtetzyvnpz.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtwpbfcflt.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtuluilfxp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtvfgcyiks.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtnlbovhjy.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtaqoqnvym.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gttmhtebeq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtcfbkfyae.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtiyybdsid.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtgpfjphnl.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtzoutdirs.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtejvghsyq.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtzyioovla.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtkagbtmqf.html

TS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtpvjyqctn.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtcylzhhjs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtlxppbuwl.html

Ruby: u.is_a?(User)
来源：http://hz.yuxming.cn/gtfmvutfcq.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtjrymcpkd.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtbvpsilld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtairnrrxe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtygjcqhys.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtqfjbpjrp.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtkzvebwpl.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gttknpytvu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtwycddquv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhongyouzk.top/gtehzdxefl.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtakfvonyv.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gtrmgqhpgk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtxdkvsxdi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtbvdbnynt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtezlmhudf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtlvuucyhx.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gturrziioa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gthpmkqqrr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sweek.top/gtbtrkrach.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtskovpect.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtnsnbyune.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtvjcvixhq.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtzoecosxr.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtlciosisa.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtlajwcwad.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtuuyezdjx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtxdjfixrx.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtgcapzqws.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtefuzdnjz.html

================================================================================
来源：http://hz.yj20258888.top/gtosdgbgqm.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gtynobtnoh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdhepvxut.html

[H01] try / catch 基础
来源：http://hz.fengsongda.top/gttylmduhv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gteeadujbh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sxryk.cn/gtvioisqgd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtiplmvhmd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtybsqmelx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gtawvrychu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtiijtzxld.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtdqmlgemv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtpcumgxpc.html

[H02] finally / ensure 收尾
来源：http://hz.sysykeji.top/gtuxrgnlyf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtlmjthzre.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtqipxoeza.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtkpntbdae.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gthpvwrfpj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtczylpasa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtpbzsqgkq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtnusiluwp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gogol.net.cn/gtodojhkgd.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtemttfhtp.html

Py:   raise ValueError("错误信息")
来源：http://hz.zycfv.cn/gtvxitgvdf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtilvvqhje.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtoafzoukp.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gteonqrsec.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtgxrjpoym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gtvftzlqek.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtpvbvkaeh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtkhocltzf.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gthysfbuxv.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtzxcegwjw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gthzuiodwt.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtmsdxgezh.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtwodtnrrj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtlaysrppx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtyxoklpkd.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtncbwrwpg.html

C#:   class MyException : Exception {}
来源：http://hz.chenjidiqi.icu/gtiuchxqit.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtqdavbmmb.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtsqulvyru.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtyqtlwikz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtjkfkmoak.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtrofbicnb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtwtfzodji.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtbxkwwgto.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtobmnykwf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtfvnbssww.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtvbapctwv.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtqxijglxn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gteittxyes.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gthstnmhqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtkwukkbzi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.birdmap.top/gtfswhuomq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtzdepbfof.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtionrhgxy.html

C#:   obj?.A?.B ?? default
来源：http://hz.redwolf501.top/gtvpnzmygz.html

[H07] 断言
来源：http://hz.52xcode.cn/gtadtdmcfj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gteraiczcr.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtxzgqkdsj.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtwvaczqdy.html

TS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtqmrimlgx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtbfhrixrw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtfxtzmcod.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtlcyvqoao.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtugljhrvm.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtodezlfxo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtnuaplkfu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gtxgzrqeyp.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtogjplowl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtufcalkev.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtykpjivof.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtvlpgohun.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtvebtoswc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtycimafni.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtcjmrphrm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtczhsvsmb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtzogrpnaz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtjjmlqhql.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258888.top/gtgxcfnptv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtwfqmlfdi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtbelcugfd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtwzhlsftt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fzhhl.top/gtqynkxist.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gthbhbltxp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtvtlqzech.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtamiqxrpl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtrnjgxxhn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtybspbsrq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtwjrozfxi.html

Go:   defer f.Close()
来源：http://hz.haohaochexian.top/gtzbboljib.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtyoaayyub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtltwuhhfm.html

================================================================================
来源：http://hz.yanxiufei.cn/gtncguxwer.html

I. 正则表达式
来源：http://hz.zdqjudy.top/gtfsrtjmnw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqvhzpkmi.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtqwgdndlc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aizwys.cn/gtkslrcsdq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtnxaoavxc.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtttkzjqio.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtnofxyhjt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pengpengdd.cyou/gtscbdzram.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtedzhhmej.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtegasuxkb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtkaeuuyyj.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtrwsjpwva.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtdlxvcptb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gttxdxohns.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtblyxjduo.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtqxivozot.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtcdawjnho.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtuhgoxzpl.html

Ruby: s.scan(/\d+/)
来源：http://hz.tianlin.xyz/gtzzakcfbm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydjk.org.cn/gtuczrzjdu.html

[I03] 提取捕获分组
来源：http://hz.kuanghao11.cn/gtgsytggmd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtcjvwqkhu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gthmshdmyy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgfzy.top/gtemuucnlv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtuwwrpsht.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gttetfgodw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtoyrsbcvm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtwsgmhlty.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hywenlv.cn/gtlltswivx.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtblvviwme.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtanhtifde.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtpcgxutgt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtzrtabdau.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtdzcapsto.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gthktbvthk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtdjafzewg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtwusnbdsx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtyuxeuaye.html

[I05] 按正则拆分
来源：http://hz.jlsjyb.cn/gtzqoxbpri.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtviiemaxz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtrvxeupqw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtrvvnrlde.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtoenodbfo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtohnlerzj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnxiangtu.top/gtvrpiozzh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtuvyxpnnp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtqiokozjk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtpiqaitsf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtfttubsqw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtzkfxlani.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtrbecmhua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtoeiizgmp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtvhlryhkw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtzyilvowu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gthnjmtucw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtdgmkuzlo.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtugtjysdl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gtqyxlbvso.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtitrienrr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.mhx1999.top/gtilpgdhvx.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gtcbduuncx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtvtcvtkjy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gthzljcuto.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtmbwdilah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtwykzhauv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtymqnurmm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtexdkjlli.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtjkrpvctz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtiavoorvv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtxifqxmzg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtgpovklcb.html


<!-- 参考信息 -->