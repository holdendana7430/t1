代发 wailian999

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtqcqqsdhk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.snrcjt.cn/gtuuvczsjl.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtpowwpeld.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtxdxozsmr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtbvdssffa.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gttpvukmfz.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtewavdgjr.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtvqqfnsnp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtjpfxgkjf.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtglajmcvz.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtkedysenw.html

[G05] 继承
来源：http://hz.dianchejie.cn/gtsrwqduvo.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtwqyieedn.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtlicziouk.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtftlvahzh.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtveaofcqq.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gthgspamkn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtlrueyikh.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangkeji.top/gtcrqwtkwo.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtjbxxgsup.html

[G06] 重写方法
来源：http://hz.shanyushiyangkeji.top/gtinyvmwsa.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtxqmjsxwq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtbqduwqby.html

JS:   greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtrwdhozfh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtwmkmbqel.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtspvdzczd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jiagoushi.top/gtahjtctya.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtndtyxkgy.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtifngcprs.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtbbdqxsyz.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtwxgehvam.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtdxaxrkgd.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtuahujahk.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gthxfcvxnv.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtsrmbwycf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtzwtgavtu.html

Ruby: super
来源：http://hz.yanxiufei.cn/gtbvpjajra.html

C#:   base.Greet();
来源：http://hz.yangfankeji.com/gtjejnllzo.html

[G08] 静态方法与属性
来源：http://hz.xylfe.cn/gthfzrziif.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ywan-chungtsiang.top/gtzawndyka.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtogjehwxf.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtuohzuben.html

TS:   static f(): void {}
来源：http://hz.feifeiyinyue.top/gtmksfoejm.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtgyreciym.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtrobjvrry.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gtmqmxxmkv.html

C#:   public static void F() {}
来源：http://hz.mhx1999.top/gtzxrexawc.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtvekfzdyy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtzvwhdlvq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtcoivtgbo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhongyouzk.top/gtaobrqjpo.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtxmipbdiq.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtzrlrvdzh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtbovlgkwy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtagawvluk.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtuptpsziy.html

[G10] 访问控制
来源：http://hz.zhoulong.xyz/gtatvcaskt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gtusxwolin.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtyfabrtry.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtrjppjwpp.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtuyidxtao.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtkdcymkzr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtxwjszsjl.html

Ruby: public / protected / private
来源：http://hz.zdqjudy.top/gtgvsnpvtk.html

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gtrofquxol.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtibrjyyer.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtkpekvxue.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gthloiiccw.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtndtkwbzj.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxuanxn.top/gtsnptwiwa.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtyqthlzkl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtgkkaufjy.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtlhfrrtfj.html

C#:   public string Name { get; set; }
来源：http://hz.nanxinkj.top/gtbfnpegku.html

[G12] 对象转字符串
来源：http://hz.ydzc1.top/gtzatxtbzh.html

Py:   def __str__(self): return self.name
来源：http://hz.haohaochexian.top/gtselitimf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtyljjuwoo.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtcdmxillj.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtdbzsnxzf.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtkztvjfrh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gttsbnakrr.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtxoirgmng.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtasqgongl.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtjwgtxodq.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtrhsamlhd.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtzlvhtrvm.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtjzhohbcd.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtqzycnhwm.html

Java: u instanceof User
来源：http://hz.birdmap.top/gtkwtzxymd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtaselkjvm.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtshrasjnl.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtbhcyzret.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtqrccwivq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtipfnjvlh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnxiangtu.top/gtxlvdgmjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtkbjpotyr.html

TS:   type User = { name: string; age: number };
来源：http://hz.cheryme.top/gtsbhstsio.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtusppemjb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtsnwnrxof.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gthyjytpjg.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtsqwqymkr.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gterpdgffo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gtvkkmyjul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hywenlv.cn/gtdgjpcymr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtajgteguz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtkutbuyza.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtotljogth.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gotoacloud.top/gtecywypui.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtcuopwtxw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtndeffsmt.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtznctiudc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtiofcficg.html

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gttokbjbcz.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtjytwaznw.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gthdurnzqn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gtyrmqxdgv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtwehrdrup.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtpgkkweak.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gtglcsklix.html

================================================================================
来源：http://hz.mhx1999.top/gtqbtqmwkf.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtuqpjkecm.html

================================================================================
来源：http://hz.andypj.xyz/gtpajgegig.html

[H01] try / catch 基础
来源：http://hz.gzhubu.top/gtlxrfpajl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gthfnmrppw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtyjlvmbjn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtkhovqhne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtbjsarwmf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gogol.net.cn/gtpvhvxguj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtwmsuthca.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtxrspqvae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtnvoqeyis.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtdnxutcjj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gthzayfxix.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtktcrrjpr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtuocqwklu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gttkoqlxvk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gttwbqezaw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtmooxchrh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gtzsweemlt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtjfelibuj.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtuylcnijg.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gtkweesvoi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtuizksorr.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtwrhwciko.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtikdwznnx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtbhloeglv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jiagoushi.top/gtnwsxyrql.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gttcxslesg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gthddalakr.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtamyembok.html

Py:   class MyError(Exception): pass
来源：http://hz.zhiwuduotai.top/gttnkrnwbp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtazbayurp.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtgdmgpqbv.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtbgerdhqa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtdwctwzrc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtyttmdqen.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtyeilvybh.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtjfjwzcav.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gtuaxosowv.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtvbzjufvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtnfjhawbp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gttgstrclq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtokcnvazj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtowgfcsyk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtynynckkf.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtgukindrc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gtviesqlwa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtofmagzat.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtlavqygat.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtmtnkaxnd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtknfnhsty.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtfwolrgqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtpvhjejar.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gthgenostf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtoempnner.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtfwiyhhpb.html

[H07] 断言
来源：http://hz.chenzaomai.com/gthpqrdfol.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gtqdmsxadh.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gthrudlgus.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtkkiknfdn.html

TS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtduaqjyvw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtozcjmdkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtthjjjulj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtmunlchrq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gttqqhgiog.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtfddihfet.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gttkftugag.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtqlduylfk.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtskctzctt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtwwibrbrl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gtzocxeqea.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtjdxufvnl.html

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtejjqmlfc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtelvqwnwx.html

[H09] 带错误码的异常
来源：http://hz.jinyuanbaomall.cn/gtzttugtpx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtjplmyjxu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtkfqlueac.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtpamqkmqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtlmjtacls.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtbxkzdekx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtzftwnzau.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtvuzykjeo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtczsbhxoa.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtxwoklxed.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtjnorcsqx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtgzsxeult.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtkyzijykx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtecnsswkc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtixyabskt.html

Go:   defer f.Close()
来源：http://hz.zhengqikj.top/gtmuwvpbdj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuanzhike.top/gthrwlmveu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtordntnit.html

================================================================================
来源：http://hz.havefunace.top/gtevbanynd.html

I. 正则表达式
来源：http://hz.cashguo.top/gttuvtepda.html

================================================================================
来源：http://hz.chenzaomai.com/gtykpdbdup.html

[I01] 判断是否匹配
来源：http://hz.aibaodan.cn/gtacoiaolj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtafzsbhqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gtxwpabppf.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtinoowtzf.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtabhjcbwv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gtpiaaiool.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtitxbvpeg.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtjdxrhsxf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtqpdofkyl.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gtdshimrxi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gtxnhbctbc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtvsajmhak.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gtbegzjuyb.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtpvojexlx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtjthtiihl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gthobmvocs.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtnnjnsksd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fengsongda.top/gthrfvuvit.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtrwdzcexi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtfcyntutm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtrpzglken.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtalerkhws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtbmtssgul.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hysaishi.cn/gthqischlf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtwndzofmy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yvedp.cn/gtfitytfvp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gteckdiadc.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtanpafzwx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gthpclrgpl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtuqnwhlsp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtwxeiozyk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtlvddcyqz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtigzzqccl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtfzcgwrqj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gttnfwokam.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtsxidxbtu.html

[I05] 按正则拆分
来源：http://hz.jinghuilouyu.cn/gtvwnkequc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gaohongyu789.top/gtdotkmgxy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gthrpfowko.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtoootkeow.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtpdilxqhh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtcmjielga.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtefolhhrm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtyewegkfp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtdcnhjfyk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtplgfuwme.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtikzivgzc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtmwhmaqmk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gthbztyzkv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtmmeegviw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtkhcpbovv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtxfsjfumr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gttbmfzxmw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtrpikxzfg.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gtzqopioqw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gtkeuvrziv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.meibo888.top/gtzzmmcxlk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jyoumei.cn/gtqudhkjzw.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gttiyhodyw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtetlnbabv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtgfqsljdi.html

Ruby: s.scan(/error/i)
来源：http://hz.9152youxi.cn/gtbpqwrlvq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangkeji.top/gtepckcekb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtzuxdczbt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtfcivgwyj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtyadirzkh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtpdernhtw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtuflqrwea.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtwipitwrm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtdjdfphxs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhoulong.xyz/gtsbwjjihy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtphkcppkq.html

================================================================================
来源：http://hz.mhx1999.top/gtnpbeiwve.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtmgjuvszi.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthuzwhhxp.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtqzmnnspi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtxcqonfed.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gttdfrymqg.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtlbrnjzuo.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtiipthhhj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yonumen.top/gtftqxkpdn.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtncwidzra.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtuqdkxyri.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtpeyqgkkr.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gthlyvombo.html


<!-- 参考信息 -->