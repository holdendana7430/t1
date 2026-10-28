代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtlbrgebkn.html

Java: User(String name) { this.name = name; }
来源：http://hz.aizwys.cn/gtpqyvrdak.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtamvclbhg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gtzwbuyhqt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtzdracuzk.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtmhiyqnnu.html

Py:   self.name = "x"
来源：http://hz.yuxming.cn/gtxyorklce.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtkjmctmcb.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtnlgehlkw.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtxgcmmrhj.html

Java: private String name;
来源：http://hz.andypj.xyz/gtuohzbdhc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cucudq.cn/gtvqixfgva.html

Ruby: @name = "x"
来源：http://hz.zhoulong.xyz/gtepnlqhsm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtyqdznkml.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtyowyvsaz.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtznmovjsb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtclyvpfaw.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtntqurxat.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtqarypfnt.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtuwkwsmsz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gttsauxdpa.html

Ruby: def greet; @name; end
来源：http://hz.ehwqpu.com/gtaskpnffc.html

C#:   public string Greet() => Name;
来源：http://hz.redwolf501.top/gtjszphedn.html

[G05] 继承
来源：http://hz.hammf.cn/gtbvhkksqx.html

Py:   class Admin(User): pass
来源：http://hz.0kj1m.cn/gttkaboczj.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtktdbbiir.html

JS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtmgsopqbf.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtmynbptvj.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtkpsdnozs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pengpengdd.cyou/gtwymjcjlm.html

Ruby: class Admin < User; end
来源：http://hz.andypj.xyz/gtftttrtiy.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtlidbpdvf.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtccluginz.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gtzhvtpohc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtnzvphwqk.html

JS:   greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtfxxkycni.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtdaijlafz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtymabrili.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtlpklxgrt.html

Ruby: def greet; "admin"; end
来源：http://hz.xuetiantiany.cn/gtnhvcvtbq.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtzrosopam.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtkaxwcsyr.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gteoodmvym.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtzxgwwuhh.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtuqbbhobj.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtsmgmmkwk.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtymfdtgvl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtyfsdusql.html

Ruby: super
来源：http://hz.cqqwz.cn/gtfvttughg.html

C#:   base.Greet();
来源：http://hz.jqgufenzy.top/gtcvbgohkz.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtcrcfsqvd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtupgrzwwk.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtftsynnwz.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtxcpwqnem.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtnpsbipav.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtqjjqbdqr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtdgdfsxix.html

Ruby: def self.f; end
来源：http://hz.yueranfly.top/gtbxtpholb.html

C#:   public static void F() {}
来源：http://hz.shangyingyoupin.top/gtarxquygi.html

[G09] 接口 / 抽象类
来源：http://hz.dianchejie.cn/gtdcfuwthp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtynnugcol.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gthnvugxqr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtenjwxuvw.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtlglxepxb.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtskpiaeab.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhijiandao.cn/gtgihbekjq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtgkgbcjrx.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtsupkfwhq.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gtvmmrosjv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtlscaxxqa.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtnanauune.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtyiieahdz.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtxuzfcjyl.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtpfemrddd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtysdfbune.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtcbziirwh.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtlkofxbdx.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtghtyuaam.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtokfkxlpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtdmiyedas.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtagksvvot.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtjgkzeejv.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtywrpkkjm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtiriyybap.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtwumdryod.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtkhhdpmbz.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gthzsnepye.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtzrqumput.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtcedfzaau.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtktclgdoe.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtlzztmpyv.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtlpfpqqsu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtqtqletao.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtaumvxyqn.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gttmxnmoia.html

[G13] 判断对象类型
来源：http://hz.ydjk.org.cn/gthfjtfrnv.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtkwfbgpta.html

PHP:  $u instanceof User
来源：http://hz.wangdashe.top/gtnsyjqdsr.html

JS:   u instanceof User
来源：http://hz.tanke756.top/gtpsebtbvv.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtjlamyzan.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtodvragti.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtngamivby.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtmbdaklfi.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtdeabchil.html

[G14] 数据类 / record
来源：http://hz.iojbl.cn/gtyhjgizjd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtysbxamxm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtnysklngv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtmcsrrhpt.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtustrxhwt.html

Java: record User(String name, int age) {}
来源：http://hz.xuanzx.com/gtdlqimxoi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtuiawrtzb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtbxvhfrwv.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtnbosamjg.html

[G15] 枚举
来源：http://hz.316326.xyz/gtdqrhzkxx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cucudq.cn/gtrelxoinv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gtrykeafwo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtnixeqzmx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtdbzcopga.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtubibkkjh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtxkjvslqv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtdcpycczg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtuqlptmqz.html

[G16] 对象转数组 / 字典
来源：http://hz.dianchejie.cn/gtaswvjqxh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cashguo.top/gtxzngmuff.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtvjxrygty.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtpmykkzsc.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtcisloomh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtlvprremn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtzqdkeugl.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtujcglakl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtkkcqsawt.html

================================================================================
来源：http://hz.jyoumei.cn/gtqhptvxnx.html

H. 异常与错误处理
来源：http://hz.yuanzhike.top/gtxjaatldd.html

================================================================================
来源：http://hz.hnqzz.top/gtabpwtxss.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtxzzltjer.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtxttnrzmf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtereeykzk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtcmxvlikx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gttnsoggga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtzyjawupa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ywan-chungtsiang.top/gtowywohjj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtjhrgfzjy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtfoeckdop.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtspocumtt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtxlifluvk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtpnezcwtu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtnqmfiqvt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtynniyfxr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtyqfklfww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenzaomai.com/gthhyblvsz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gttdlgqjxe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtrcczarie.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtyxwwtdmj.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtipoovpvq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtobtdiiux.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtjysgjmcq.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gthlfpslbz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtfardijph.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtzasditkc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gticjxjtvx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtcdhgieyf.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtfgzaeqdl.html

Py:   class MyError(Exception): pass
来源：http://hz.yuxming.cn/gtekcxekyl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gthbyxjggx.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtccihpyyv.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtsqmmbnmk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtqmsaniwa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gtadwxtewj.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtbbernoum.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtfyudvwda.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtzqqtayek.html

Py:   except ValueError as e:
来源：http://hz.hnqzz.top/gtqnodsrcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtyyamtwmj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtcxwqenfo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtbazxtmxq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtwazqdgsw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtuhwoopsi.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtmlriaykj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtbixtbmde.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gtbipeswkm.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gthfjwxzfs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.smart0.xyz/gtmjylvhdg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtvbyqcfxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtcbdlteck.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtitrqmvqh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtturormkp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtcixnayhv.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj202588.top/gtpppvhijf.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtamhudxsq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtnpgkiapk.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtvogcezgh.html

JS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtzcqgcozt.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gttjqwncca.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtnrkneivw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gteooijsru.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtzddtawfg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtwdbkzdsy.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtipjclbpk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtnavkbkkn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtepailmco.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtkdlyepkq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jyoumei.cn/gtpfgoqskp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtksvbybcp.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtxqejssuo.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtbdncanqf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gzhubu.top/gtcyqxwsof.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtaatxfdre.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtkwmaskqu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtsjmdlwtm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.316326.xyz/gtiqecoyam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtawykozob.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtlkpmdxjl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtpwvfooni.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtnqciutvc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtzrfayaxo.html

[H10] 资源自动释放
来源：http://hz.ivvv.top/gtqyrwylsx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gtncmcpmwr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtmpgiulrp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtekujryfa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gthvyhesdp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtkchrofvg.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gtjysxivbg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtcpewubbx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shzxlz.cn/gtvfttzghq.html

================================================================================
来源：http://hz.daxiang520.top/gtxcvefaay.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtijasxwtp.html

================================================================================
来源：http://hz.haohaochexian.top/gtayupeahm.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtrjrvegib.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gttffejury.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtckziqvvu.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtknznorbv.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gthciwwteu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtypxfvaot.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cqqwz.cn/gtoxguchjx.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtbrimonep.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtlpiqcvmm.html

[I02] 提取所有匹配
来源：http://hz.zdqjudy.top/gtbvwgsfwd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ppjwa.cn/gtxmckmsvq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yanxiufei.cn/gtaypmxjxw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtkucitgvk.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gthinpjgow.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtalpdvtrh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gtefnjvhjy.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtqtgbkwar.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtixogzdrb.html

[I03] 提取捕获分组
来源：http://hz.cqqwz.cn/gtxigmycmq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tianlin.xyz/gtdbjztdzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtxymjjdmn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtfgflraod.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gthiyacofc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtiyagvijk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtpdvtqfyz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.bjfxy.top/gtlcrqlaxr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtwfhkcalj.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtfbizctjr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtxehjsjol.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtbqitsnoy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtbnyjiqmc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtjhfwkzae.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gtnjfvizgw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtanhptbek.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gteeagxbjy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gtqmpfhfei.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtzstrpwwy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtpgivpeza.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gtmhmjjeqm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtslpvtirj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtksnqbtcn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtpqaghnwn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtmbvitdcx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtcilgqslo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtrmknexgr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gttslfmorx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtkmbsxsty.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtetgaeybr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtfrvztdgd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gttytwkvqz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtdbcmhxeg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtogszczxx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ppjwa.cn/gtznjdaklg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtacvqmamj.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtcmsyygjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtzosbrbtv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ybcxt.top/gtiyfcqdyq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtjurvqoue.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtehjksbzz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtccskjgys.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtrhohsbvv.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtyaplsdyj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtbunldoxz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtdqxkzngw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gteuonvcqj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtacazgwfd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtbkhfvckj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtvjphxgvi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtrqolvuww.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gticbcdbcc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtelkhcqmc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258.top/gtixufnrhm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtinpmyghd.html


<!-- 参考信息 -->