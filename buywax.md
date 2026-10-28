代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtaabortmq.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtvrffharp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtrvvmyhzd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtrvlegwre.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtsepjmibs.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtzdmhaugy.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtdamquxua.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtpmzixdsa.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtkbqlczqr.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gthkfgphro.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtfpjdpjnb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtozonmswj.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gtlnnmammf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gtmlntvqfp.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtzcjfotne.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtlcpgimqy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtpyzddsie.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtmttijfdg.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gttxvdgdcp.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gteqfybrdt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtcsptaowj.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtusmpjwjo.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtfjqcklto.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtkrknvjlr.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtocmhwirh.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtlvsroiyb.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtpdrrteko.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtyfnektpd.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtwbnhsgpq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtdnivivcz.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtvmvkmikq.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtkfuyeiwj.html

[G06] 重写方法
来源：http://hz.zycfv.cn/gtpauttrko.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtgzomlvbi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gthtaqzohm.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtvriiguqx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtmhlbpquq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtbbaaalpc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtilojiere.html

Ruby: def greet; "admin"; end
来源：http://hz.meibo888.top/gtadjlvsjt.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtqubbwcwv.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtgepjvucp.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtvkebdwdk.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gttzymjpoa.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gtyuqddrvt.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gthevikroy.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtieqmamtr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtbbyiomfg.html

Ruby: super
来源：http://hz.yj20258.top/gtynsnkqyh.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtqqdbgvyp.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtmxvircze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtymptbkjw.html

PHP:  public static function f() {}
来源：http://hz.iojbl.cn/gthmllgsnw.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtcsqalyty.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtcegecgau.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtyosnvtui.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtrcxpnhce.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtprpbwaqd.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gttdwfkmpv.html

[G09] 接口 / 抽象类
来源：http://hz.cdnleiting.top/gtfisjlqof.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hysaishi.cn/gtaywjivfx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtohfhhlul.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtwiqqcefk.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtgslwkpyz.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gthsslcdbf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ybcxt.top/gtscvzwksm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtlthalmhp.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtyxsqarbd.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtujhpuaql.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cucudq.cn/gteoqirjzq.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtrqbgkhkx.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtmmklendh.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtfrqimoko.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtguflwnpk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtdrxvidzj.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtppbpjjfm.html

C#:   public / protected / private / internal
来源：http://hz.ywan-chungtsiang.top/gtbksmqizu.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtmydlkwdm.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtqpuswzku.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yueranfly.top/gthviodnuk.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtlgzxwybt.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtjvjheyhc.html

Java: public String getName() { return name; }
来源：http://hz.bjfxy.top/gttdjugovm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtwpmvhnzo.html

Ruby: attr_accessor :name
来源：http://hz.dianchejie.cn/gtoqujrruy.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtshlljxud.html

[G12] 对象转字符串
来源：http://hz.shzxlz.cn/gtywwwtict.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtacncinbc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtdlatylkw.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtrioigxfv.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtvmpmqpea.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgufenzy.top/gtqcgimall.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtynyewtze.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtwjvuafvd.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtwoebdtud.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtllrmwntl.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtcxwmogyn.html

PHP:  $u instanceof User
来源：http://hz.tanke756.top/gtmrmiurle.html

JS:   u instanceof User
来源：http://hz.gaohongyu789.top/gttroncgcc.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtkwtaudfh.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtadtwgcwh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtgriacqew.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtilsrkewc.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtuyvjpzvv.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtsfjqqnkt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuanzx.com/gtiygzxoee.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtoxabdrjl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtxleqibgn.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtgdysfpgo.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtjknfvqxz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gtoyouhsth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gtzbsmbfzj.html

C#:   record User(string Name, int Age);
来源：http://hz.xinyue.icu/gtmuejqwyl.html

[G15] 枚举
来源：http://hz.cheryme.top/gtfehxaayr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtprubzaut.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtlewymwjl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtgaheqphq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtdnoieqhz.html

Java: enum Color { RED, GREEN }
来源：http://hz.zdqjudy.top/gtqhntpaus.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtjstznlvg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtrgduedsi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtfjyftgvc.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtyfffwqln.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtdknzpibd.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtwqevxubl.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtijtwnaon.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtpvosdcyu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtlrtlefrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtndsmxiba.html

Ruby: obj.instance_variables
来源：http://hz.ydjk.org.cn/gtqeffdfym.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtpettnwdb.html

================================================================================
来源：http://hz.fengsongda.top/gtfgdywpks.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtpxalgxch.html

================================================================================
来源：http://hz.jyoumei.cn/gtaiqvkguj.html

[H01] try / catch 基础
来源：http://hz.gzhubu.top/gtapluklgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtnpdjbrva.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gtmunthocb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtklcvzlhk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtczmbdpuk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtgyttkkuz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtxrxopupv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gthnrhaagm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtclbsbnwb.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtyraigwbp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtebzzgxum.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtgzugobks.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtnoiulyxv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtfebolymk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtlpfzsgxe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gotoacloud.top/gthhjxtmxl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtgkyphozy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtsoktyahs.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtgwvcnupf.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtqzagruhr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtfuitkoeh.html

JS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gthpufyhqj.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtycyqyyhb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtevodurra.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtobfkstht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gthfbevbyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtojnhwmyc.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtdwrrmpfi.html

Py:   class MyError(Exception): pass
来源：http://hz.jinyuanbaomall.cn/gtrprtevci.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gttqtzqmdv.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtoybrsrmn.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtgjdgcvku.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtekxqijzl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtxnlhuqbf.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtlujnkuem.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtbzxtruog.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtngnglvcz.html

Py:   except ValueError as e:
来源：http://hz.quarkkingdee.top/gthvowkbuw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtdwjkpfvz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtksezzgec.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtivdfgeex.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtxzolqlsh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtfjcvusil.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtmxwqvbdi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gttbugpobe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtwlbuqykr.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtriimpmod.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yongpay.top/gtbpcocmfm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gttazqpzlk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtbvounhpb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtumjjpgza.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtklybkgzd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtgucucbai.html

C#:   obj?.A?.B ?? default
来源：http://hz.kuanghao11.cn/gttxgdrtzp.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtdtxzzfte.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gttoxkyops.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtpddalnst.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtnnlwjwka.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtgqkdvuhp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtrqctaexd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtqpyapjdy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cashguo.top/gtriyzizvq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtkeoiuado.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtgkmasgiq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gtlwjuzyyq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yongpay.top/gtagmflwuo.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtqbdfhqla.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gteggjpoam.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtuaszmlpy.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtcbwvyaft.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtkwrikecl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dashuyun.cn/gtjribcivw.html

[H09] 带错误码的异常
来源：http://hz.daxiang520.top/gtssxvxdto.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtgzgidsxy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtovujbedd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtrzlqhrrf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtrsnczczn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtjkbtgfrg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtibotsgkn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtduvhgfal.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtpjjivvpk.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtbesscmqn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtyyxxnmye.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shzxlz.cn/gtvulrrste.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtysvlnsyn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gttzkxzzhy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtlqkguley.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtailwbhbe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtocxsinbo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtdptdsxyh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxfodwqhe.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtfokczbxk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzyqpwwou.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtzxpsnojb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtubhfvvia.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtfarxrlal.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtelgjhqro.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gttzlbqlwf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtpfkpxrqb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtabkslbro.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangdashe.top/gtjsdiazou.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtjdauqvnz.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtnfyxikat.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtxhxxvxhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtfczwqdjz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtadntxqep.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtcznyymvb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yueranfly.top/gttwstubql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xziqi.cn/gtlhqhqemj.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtbrdfoeil.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtbziwlynt.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtlpxaeteo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtejdmttrq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtyckoadmg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gteifnwarb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtvuskhnwd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gtkeetwxvs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtdxtllhey.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuanzhike.top/gthobayqgo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fzhhl.top/gtmqbxeujq.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtwpgtbkfg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtaenalese.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtnltsaubb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gttxdolpyx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtaiitlhfi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtuujirxzu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gttmgsqqnw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dashuyun.cn/gtpxylxczr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtcoekiiqr.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gtzbdvdhlb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtyuunjtip.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gaohongyu789.top/gtdxjyuiux.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtexdpgzgq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtqoeubdjc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtucwntlgm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtvksqkgbi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtxtiztgto.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigufen.top/gtksrgzyag.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtejbsbpuv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtorjcabws.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtwhzifbuz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gthxeexyyt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtttchkpzh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gttjblemfv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ywan-chungtsiang.top/gtqfhpygru.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtevdwaymv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtrgjulqws.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtwnogxxau.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gttboffjct.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtposxcngf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtvwwfeclo.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtlvciaoji.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtlepuymok.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gtkcjwdsjn.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtlvutqsys.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtoeydztpw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtvzujxmaw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtobuzudyq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtgjbohfuf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtbqnrvhmw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtserpelvv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtywqwnqva.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtxyntgwsg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtpvvpbssg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtdxakzeet.html

================================================================================
来源：http://hz.guannengcc.top/gtizrgzylb.html


<!-- 参考信息 -->