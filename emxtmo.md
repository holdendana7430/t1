代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtvflzffdu.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gtaqbscahb.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtciixzrrc.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtdwzacptw.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtvxcdpqto.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtdwwyfdcz.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gteecbaloe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.birdmap.top/gtfrllfaqx.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtprllkgaj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hongshengwenyu.top/gtgqynwnug.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtrqsxotvk.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gthgnepani.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtwereppju.html

JS:   greet() { return this.name; }
来源：http://hz.dianchejie.cn/gtgsxusozc.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtjvqynbej.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtqdbigcoj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtycosnnfz.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtotqrluid.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gtibtkrfbo.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtwxsxclcm.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtvwzazeqk.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtrzqycywm.html

JS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtswpvtecj.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtgcatvyhx.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtpusqensl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtdacwlpny.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtnglrfush.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtryjqfrwu.html

[G06] 重写方法
来源：http://hz.pycfn.com/gtteksvpnk.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtevzcdgyi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtouinscon.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtwkxdoyjw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtnfbonxyl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtptvtzvon.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtefdhwipt.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtonyeigyo.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtgocxwhlu.html

[G07] 调用父类方法
来源：http://hz.iojbl.cn/gtnsqxszsb.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtdecfulis.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtanuoxqqa.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtxejadihg.html

TS:   super.greet();
来源：http://hz.yonumen.top/gttrjocacn.html

Java: super.greet();
来源：http://hz.yj202588.top/gtmktzvbuv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtmtejtpkn.html

Ruby: super
来源：http://hz.guowangkeji.top/gtfbhuikon.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtpouugfab.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gttswqhebb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gtxduclptc.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gtfczaqaok.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtfytjkygp.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtotrammsg.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtruocomcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtemhrbion.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gteaxbblov.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtehehkxuz.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtcplyfpwr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtdjnnaqhu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtwjbzdefw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gogol.net.cn/gtygcrvirf.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtmfqfdpze.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtdlryfabh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gttojlmsgu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtfbkfnveq.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtaumqnouv.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtbcvaezzu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtcqpssyyv.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtfjrhpuxp.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtjkmsiflo.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtronhivyj.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtlhxncjgf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtkvrujdan.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtzjqzcmub.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtrcjhxkxj.html

[G11] getter / setter
来源：http://hz.guowangkeji.top/gtuzzmxhlf.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtlfwltenu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtqfesrtyz.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtawmighyf.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxinkj.top/gtumsngisa.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gthsdmoppp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtwrmtlyih.html

Ruby: attr_accessor :name
来源：http://hz.ydzc1.top/gtpiahcszf.html

C#:   public string Name { get; set; }
来源：http://hz.nanxinkj.top/gtqgqixach.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtrbpdewfa.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtzpfjyxxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cheryme.top/gtmlvccyuc.html

JS:   toString() { return this.name; }
来源：http://hz.chenlongwang.top/gthydnssfj.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gtrbsysajp.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtjyrrnurb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtrdzxmkjt.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtwjekqocv.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gtyefaedhp.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtjdjttzko.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtfrkcumfx.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtlfruvmpt.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtsvuerfes.html

TS:   u instanceof User
来源：http://hz.daria6918.cn/gtstsuuxus.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtggtlrshf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtdrhyhcml.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtaberfizq.html

C#:   u is User
来源：http://hz.cucudq.cn/gtsdpkdbro.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtnbjgaavs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtbaxkttjs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtsygqwyjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtgjqurqvs.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtuynmddzz.html

Java: record User(String name, int age) {}
来源：http://hz.dashuyun.cn/gtgdvsrynn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtgqdrpmdn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxinkj.top/gtrfxkrqnk.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtvvozhhsx.html

[G15] 枚举
来源：http://hz.hammf.cn/gtgjjywxql.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtlnhgsuzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtgqnjdsnc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtglopayai.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtqkkiocfo.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtdlmnjvch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtcglikmye.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtnmzirkxl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtrvdauinx.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtqlpjzypl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtxyqijbpc.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtxshdrfhc.html

JS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtungqlksu.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtunfijhqk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zdqjudy.top/gtaqfltocz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtsfxfmtyt.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gthkqdibot.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtvdiksbwg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcbhlrajp.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtfuczcidc.html

================================================================================
来源：http://hz.xuanzx.com/gtwlejnvbx.html

[H01] try / catch 基础
来源：http://hz.xingfuxueyuan.xyz/gtzoozliwr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtmmifxdvu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtasspygcg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtfpqhacem.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gtcpqizpbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtayraxacx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtxxihajyb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cqqwz.cn/gtxifatans.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtzehtvkap.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtgrptlian.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtpbxgpubh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtgubiyfcl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtkyjfhmzj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtbetfyuvf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtooeqiufv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtllpnjzhj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtttyrimew.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cashguo.top/gtphapesex.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtditactkt.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gteomggojm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtgjashhio.html

JS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gtaecpfqqh.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtlypephzi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtjqtwowsm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtjkgaguyk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtkuzcgjdl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtmsmzkofs.html

[H04] 自定义异常类型
来源：http://hz.iojbl.cn/gtkkcfjtky.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtjpaktsqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ivvv.top/gtigmlouxy.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtuwrrbuup.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtxorjoaph.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gthqrmjkjx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtxzvogsof.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtjveesqhc.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtyykewtid.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtqxwusydo.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtcduzeqgf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtgddsemfu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtcsjxnhev.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtqbikkjwp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cqqwz.cn/gtptgplrjh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtoglrloer.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gtqjvqjnbt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gttvdqhbwx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtdylsczwt.html

Py:   value = d.get("k") or default
来源：http://hz.gzhubu.top/gtegbjjoga.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtgvzeogom.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtercexglo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtljdkipzx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtyjmynjth.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtcjaymqpa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtzcvmemnq.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gturqbynxo.html

[H07] 断言
来源：http://hz.jianghu66.top/gtewfasfpd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtkhkankmy.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtqqhfvzcy.html

JS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtwxkfffhf.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtzjgvrroj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtllwvmidm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gthwscjiyn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtcyjhctyg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtextpcqdz.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtybqlhckf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnqzz.top/gtbjdonkwx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtncxhacio.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gtmywsztzq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtdjycilkr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtcbfznbez.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtmmgxhvnf.html

Ruby: e.message;  e.backtrace
来源：http://hz.redwolf501.top/gtubroanuk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtnjmduyxo.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtaecovblu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtceppnbxd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtyjzrxdxs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxinkj.top/gtycecsmlq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtkqputzpo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtdcsaecwz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtavisrsrm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtvpwnosfv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.havefunace.top/gtalpbivns.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtmeyasxhm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gtsrkjqjom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtpsnswafw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtjcduyvkc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtxsxwuyrl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtyzunmefk.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtjatopooy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtrwvkyqkm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtauhzyihp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfihectzm.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtfvdedarm.html

================================================================================
来源：http://hz.hammf.cn/gtrmeocqxa.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtzxdpgdca.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtsauwkwzg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtiqnxwvdo.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtnchcdczj.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtvtwfjjiw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhongyouzk.top/gtguqefwwb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtthxhpsnx.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gtbkgbfkes.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtsvajmjmb.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtimojtphm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtkjufjeyu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtgwazgxjw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtnvvjsqbn.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtstntrack.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.bjfxy.top/gtzrvgbkje.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258.top/gtpdhbqrau.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtizrgwhxy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sxryk.cn/gtvelhhbfh.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtxlxnfkwe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtqmwnfvai.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtiwuwxyrz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtuzyuyppf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtitcnfeob.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtuztgmuuw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtpipoargb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.vqdsnc.cn/gtmtcsjvwo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yangfankeji.com/gtjlcppbse.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtknhtjdru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtbvmhwmpg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gttgfcoziv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtoogpefhm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtyywdpfhz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gtxdymcrqt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtqwisuxkq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gtmqdwgzio.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtbuaxgkkp.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtakwfrcyb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtylecdufw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtyarcofue.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtbaywvazv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtistfvrmw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtrjblsycm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gthyhayvcu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtxsrcbrza.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtjxttvwmk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtoliubwdw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtrhrxdzuy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtkwscuzek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtotglmhvt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gttkkplric.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtsdsnrgvi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtlsufaeei.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtpwvaugia.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtdjocdxkc.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtryzaclkp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtcmkssvnp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtomwcwtxw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtbdepduuo.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtexosbddh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtcuichmry.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dianchejie.cn/gtoaxawydx.html

Ruby: s.scan(/error/i)
来源：http://hz.hysaishi.cn/gtyickagym.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gtxmzdekna.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gtrfrwxvbg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenlongwang.top/gtniwdvojw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtqrcxnuyi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtovglcvch.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtjckihggt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtacyzhycd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxinkj.top/gtxtsncdcv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hysaishi.cn/gtufmrlalx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtegaojmre.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqdonjygl.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtjzcfgzba.html

================================================================================
来源：http://hz.aibaodan.cn/gtvknoydan.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtehnsduou.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtsflvqhsp.html


<!-- 参考信息 -->