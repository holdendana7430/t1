代发 wailian999

Java: class User {}
来源：http://hz.guannengcc.top/gtgcfczwtg.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtnkxjwyit.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtrfnddzrp.html

C#:   class User {}
来源：http://hz.cashguo.top/gthbzpwcrv.html

[G02] 构造函数
来源：http://hz.sxryk.cn/gturquotqn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gttdddkbwe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtnbetzzly.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtwjbqyeyw.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtbbsccqge.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtoiagdhgg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtjmwumkcr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtzjrjqgtl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ehwqpu.com/gtvkxzbotp.html

[G03] 实例属性
来源：http://hz.hfpthk.cn/gtzltnnqel.html

Py:   self.name = "x"
来源：http://hz.nanxuanxn.top/gtuaiaunpc.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtrpntrriw.html

JS:   this.name = "x";
来源：http://hz.sweek.top/gtgopivizu.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtbptoxikp.html

Java: private String name;
来源：http://hz.birdmap.top/gtysnhpdes.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtliizkeqc.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtdoddtnbl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtilmeujbo.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtcoupwkae.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtexmqbmtk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtrdblkcoc.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtptgkashq.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtrdvhzqgs.html

Java: String greet() { return name; }
来源：http://hz.yuxming.cn/gtarxbadzm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtmaixoxab.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gtmettdkky.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gthlcbkgfc.html

[G05] 继承
来源：http://hz.daria6918.cn/gtkavyeoos.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtjmlucgcp.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtyhyspssb.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtdsznqjjp.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtuggbpfbv.html

Java: class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtympokczm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.0kj1m.cn/gttpuofvyb.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtepetubmu.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtkincgpte.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtfddxwvmf.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gthkfsiofe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtmavgkxju.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtzlbffefw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtmgtahesz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtosjbpruu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gtayvkqjhl.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gtiklepqfb.html

C#:   public override string Greet() => "admin";
来源：http://hz.fzhhl.top/gtpsatnyyn.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtrqrmrxwl.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gtuskexjvc.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtnmzgglgl.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtdqcsvhxx.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtmkueephi.html

Java: super.greet();
来源：http://hz.hywenlv.cn/gtbsoiiqbl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtpdvojoux.html

Ruby: super
来源：http://hz.xziqi.cn/gtbiymqhil.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtvqqcqrau.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gtlaauxguk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtjnphkgrb.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtnhknpbuw.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtilmiyrcf.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtptqvqfoa.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtpwvxtthi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtiyzrfopy.html

Ruby: def self.f; end
来源：http://hz.yongpay.top/gtwabfikfa.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtjqomjrae.html

[G09] 接口 / 抽象类
来源：http://hz.hammf.cn/gtljvmdsdj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtrzzuoqce.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtabzrnjru.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gttyqzvupv.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhaomingkeji.xyz/gtblsdciel.html

Java: interface Shape { double area(); }
来源：http://hz.hammf.cn/gtnnsrmpad.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhoulong.xyz/gtqrubkvyk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtekvhawkn.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtwlmcuoca.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gttuidcdtz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtzqzxotvm.html

PHP:  public / protected / private
来源：http://hz.daria6918.cn/gtzmvusklx.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtybhwklnf.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtyctosgcc.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtnudqsmqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jianghu66.top/gtzhvdyaly.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gtzwwpjoxb.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtxgphqunp.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtvklwukwv.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gtbtuucgbg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtlmvpghij.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtzohjxxqi.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gtigwndvfv.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtkvzuwilk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gttbhvvcog.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtxrmuhxmc.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gtbwlwjigo.html

[G12] 对象转字符串
来源：http://hz.chenjidiqi.icu/gtoyeaapai.html

Py:   def __str__(self): return self.name
来源：http://hz.yuxming.cn/gtsjuqmczj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtxrewwpai.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtnhvdgpjx.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtrogxpano.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtlvnwguap.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtufoatjce.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtxcoinehf.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtexbjbpks.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtujmupxwi.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtclnofwwe.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtioboijfg.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtczefnfyb.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtjcloegzb.html

Java: u instanceof User
来源：http://hz.sweek.top/gthnltqcjb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtruaqzldd.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtexdnqrhd.html

C#:   u is User
来源：http://hz.ydzc1.top/gtmglylxdw.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gtmwwybwuv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gteqiwgvsp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtvnuvmkeh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtvlktbykj.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtgtccdzye.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtnejrqyfe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtjfwmaaho.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtviewcshf.html

C#:   record User(string Name, int Age);
来源：http://hz.andypj.xyz/gtfvgbpsbu.html

[G15] 枚举
来源：http://hz.jianghu66.top/gtjonfamiv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtcrkpyltf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtfnsrytai.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.andypj.xyz/gtckclmvxw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtadwaiacw.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gteopxdbrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtunolmsts.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinyuanbaomall.cn/gtiadvvywg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtpkhacmda.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtqeynhztc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtxvyhxjvx.html

PHP:  get_object_vars($obj);
来源：http://hz.gotoacloud.top/gtibmbhaap.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtsqhrwghv.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtdjoegesh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtupyknnjb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtpkszqupg.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtuteodkfb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtwzrmoxid.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbkaepemy.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtbunbyzmc.html

================================================================================
来源：http://hz.guannengcc.top/gtprlpsmsw.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtyxkjsebm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtcthjutxm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gthdpraxty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtosbkghti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gttectextv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtvksqbubx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtmuwhflzn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtukvmgvfc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtpkfowupj.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtllaajqsu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtiwyvtkwk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjtvecrtz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtfssrbakj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtjwgrovhw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtroamfqrx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtugsujxjg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtuwffsucq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtknpcbedq.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtcnuzojeu.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gttvwfkmtd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtlakcyqgq.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtnqtzdjhb.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtqvsukfdp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtihpztvei.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtjkilxajp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtfqzhuycw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gteenosbqk.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtvsztcwts.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtkkhtcdjg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtzfzwdejk.html

JS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gticzwopfw.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtykzlewyu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gttyculgec.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gttgqewdsn.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinyuanbaomall.cn/gtmpnwjugj.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtitofpptm.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gtaxafeioq.html

Py:   except ValueError as e:
来源：http://hz.hammf.cn/gtfknaiecp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gtrdepvwso.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtdrznlhjm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtueifwink.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.iojbl.cn/gtrhubnzlx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtszozrxgs.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gthvltwbmf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtnkmeotmb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtxhoyyisl.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtazzohefv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtjzntzeva.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtvmsoccbf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtkcwjzwwk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gtffwyofpb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtbrkkcywc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtmsejvfiz.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gttrtilmqp.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gtpyhajwmq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtatgilnjv.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtuktvfoky.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtfinojdwi.html

TS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtuyonpkbf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gzhubu.top/gtwrgvhbqt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gterbndncd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtwifmsakh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtpgdctfac.html

[H08] 获取错误信息与堆栈
来源：http://hz.kuanghao11.cn/gtoejaqyse.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sysykeji.top/gtvvlhvlda.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtmhsqmtfs.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtysnbqudr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenlongwang.top/gtukrjkhqz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnxiangtu.top/gtauwdrrqh.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtwydttzxc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtnkjwhcni.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtfenbildo.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtuabotjrc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gttdcyotdf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtuhsbnjie.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nwbrower.top/gtzepbinqq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtqunltzbm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtiecpzbsq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gttxhkpytq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtcqdqspwg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtjuewpklq.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtnpqogakc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gtkbuknccu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtvfbuqdsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtwvfpemrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtbmmzqzks.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.smart0.xyz/gtlwcexdfp.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtybljanox.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtbbvsdodv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tianlin.xyz/gtsktirpgz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtycoynbzg.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtvyvzunhb.html

================================================================================
来源：http://hz.meibo888.top/gtbjjeryxo.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtfesljnjg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtlfoalxtt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gttrbhvqsh.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtdnyoradq.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gthttnwryo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gthbwxujgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gthzjcjhtf.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gtrrrymecn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shangyingyoupin.top/gttcxjuqwp.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtdcnxwhri.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gturxogbfx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cashguo.top/gtewldttgj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtdxvghhcf.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtewcprdqi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pycfn.com/gtkrecdprc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtgqlhkipf.html

Ruby: s.scan(/\d+/)
来源：http://hz.tanke756.top/gtcbecxhzu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinghuilouyu.cn/gtvhlpgscj.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtlywhhspa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtkstcymeo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtltygepap.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtmlcsoeez.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtyunwbhww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtshwengzz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtvdskijuf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtktqpevyb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtylakteet.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtgsgghriq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtkbawlrau.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtszrgrbsj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtygalzaau.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtbljkpuvw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtxecnrxah.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtyhtswoxs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigufen.top/gtojyasxgc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtwhnkkcpe.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtwgphsltm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtxmmkpqnw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtwhtdunnc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtirorahee.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtwkkoqfky.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtdhxdrtph.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jianghu66.top/gtpslmfvpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtxztiefnb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtdbfqjuba.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gtophawueg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtjswqbgig.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtjmuweflx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtgbihryxb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtbvoxyone.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtaipbofbh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtsprqkvgw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtcmiyqpua.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtpudtetsy.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtwzpyrvjb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtbbbxeqbj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtcsbkfegd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtohkavnay.html

TS:   /error/gim
来源：http://hz.sysykeji.top/gtlotpjlrw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtyiouxhok.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtjfthpfqi.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtjvgramot.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gtekuhdvss.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.birdmap.top/gtepmdyonn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtbgztcail.html


<!-- 参考信息 -->