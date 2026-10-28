代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtnbjhzycw.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtyyhngtkn.html

Py:   self.name = "x"
来源：http://hz.gzhubu.top/gtoepekdhl.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtsyczcbbg.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gthryujawx.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtzllwauvs.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gthsprifhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtcrtkkpwz.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtsrueuebj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtkyodrqmb.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtpgeclhwt.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtlzcajjtq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.havefunace.top/gtgdgyhaii.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtibvcwpzu.html

TS:   greet(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtrsgshctz.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtcmmbwdwb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtayhxvjis.html

Ruby: def greet; @name; end
来源：http://hz.kuanghao11.cn/gtskgirfjp.html

C#:   public string Greet() => Name;
来源：http://hz.jyoumei.cn/gtrcinxbxb.html

[G05] 继承
来源：http://hz.yj20258888.top/gtsewnetip.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtafqrfveo.html

PHP:  class Admin extends User {}
来源：http://hz.bjfxy.top/gthiyhfbmj.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtdzpwlbqg.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtdugaykyc.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gttjgbaznl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtbbczgzbq.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtnospcepm.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtadvfvfoe.html

[G06] 重写方法
来源：http://hz.svipenyu.cn/gtojjpctzr.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtgaynmljj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtimpulmlx.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtrcnpawig.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtvnhldjpo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtuoitowdu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gaohongyu789.top/gtditfrwgr.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtcbwvcmhq.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtpxrwzqjk.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gtswinusho.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtigzkbero.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtezghdrwo.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gteqoosyky.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtzoteayaw.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtxlabejbs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtgrcrvmgf.html

Ruby: super
来源：http://hz.zhoulong.xyz/gthlixvoxt.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtqycqpanb.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtjstnsach.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtjheelkva.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtrrhctiqb.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtcstwpmvh.html

TS:   static f(): void {}
来源：http://hz.zhiwuduotai.top/gtfxwwexvc.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtinwoyeii.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtaiqumozg.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtbgufwtuy.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtafvkndgv.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtkudwbpty.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtqpkdhbbd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenlongwang.top/gtbxiptghx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtknmnexbm.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtfdenbcpd.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gteagoncyx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtqziurmnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gthouxpkrx.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gterxzpbsm.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtijunupom.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtyscjjdkc.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtdiqgiywv.html

JS:   #private 字段；其余公开
来源：http://hz.52xcode.cn/gtahhtiqsj.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtlgwegzar.html

Java: public / protected / private / 默认包级
来源：http://hz.52xcode.cn/gtraypktve.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtoxdrdlwv.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtsisdjuip.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtkfwidmow.html

[G11] getter / setter
来源：http://hz.sweek.top/gtdxmbiize.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtslpinvwn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtyrwmbpir.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gthfubeexl.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtrparjtjd.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gttzqlavvt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtourypzkk.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtsxjvhifb.html

C#:   public string Name { get; set; }
来源：http://hz.wangdashe.top/gtzwemmnml.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtmwsxhmfx.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtucapjrji.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtmijgslvj.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtflbsydtw.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtpaljouoz.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtqfniislx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hysaishi.cn/gtwcnomstj.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gthfuexpik.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtahladmot.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtvwniftjs.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtgnwqtizq.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gthooameco.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtbqjoipqw.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtyzhgrzig.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtxyyoesys.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtictrgupd.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtacpxvwxe.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtmfwhqwbi.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtbumsrfeh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtegfjtfms.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtinmnolhn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.9152youxi.cn/gtcdoedinl.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtixjfjmvk.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtrgdvigea.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtetybclri.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aibaodan.cn/gtloseikdy.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtakhumume.html

[G15] 枚举
来源：http://hz.zhoulong.xyz/gtzqukihyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtuvwvvfla.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtvmpsdukr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtnwjjidtk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtisexolux.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtckdtpokj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtbwogqjnc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuetiantiany.cn/gtazghiszi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gthfifhvso.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtoakixvob.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtsqclblyz.html

PHP:  get_object_vars($obj);
来源：http://hz.tianlin.xyz/gtlahwkzpu.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtszacitdg.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtxdlukkyy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhixingplan.top/gtcmlozzri.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gttmuhvqmg.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtmokurjzz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtbrounasd.html

================================================================================
来源：http://hz.tanke756.top/gtrspfafrk.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtvhaozvwp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbzlssvkr.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtvogxwcjy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.iojbl.cn/gtbwmigdhg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtmhyddfgb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtyinvmkig.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtwtvhpmgq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtkhtifmwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gthnrvadej.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtjbmutwuo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtikzxhvwl.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtfstdxhjx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtnjiziejf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtvvyqryge.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtjlokafaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtzhtrcipt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtkcnawywb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtdvchgnjt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtluinjbna.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gtsvlhcgrd.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gterkztyma.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxinkj.top/gtfxkrbhjj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtrdyhnejr.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gticiahvvu.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtbvxrzdfj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtzduaenbx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhongyouzk.top/gtjwsknbis.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtsoiikorq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtwobgazpf.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtvusgzucu.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtuocgzmfv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtbmgjkeaq.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtzrejxgsi.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtmwhxtglm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtvqhdvazy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtnnmmgvgo.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtsykbwlpt.html

C#:   class MyException : Exception {}
来源：http://hz.vqdsnc.cn/gtvmhtorwf.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtzragohoa.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtjtunykjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtiojqgmwd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtappprhxx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gthbirwtrk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtexjjztwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gthafvkyli.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtpataiywa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtfugkqfye.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtgmoykzoy.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtfmzbpoqt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtdhwariso.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtafjaundz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtzpbailnr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gteiksduad.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtexiypsii.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtrjsdcgjb.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtwjgbpnym.html

[H07] 断言
来源：http://hz.cheryme.top/gtukqokbqj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yonumen.top/gtdxcapppk.html

PHP:  assert($x > 0);
来源：http://hz.andypj.xyz/gtiqgoztyb.html

JS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtssmwueqb.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gttnsgxyfr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtdodnibgq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtimdnzoln.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtxhdmvgqq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtkdhfaern.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtzxmbuesk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nwbrower.top/gtkhjsobcl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtarvossmg.html

JS:   e.message;  e.stack
来源：http://hz.sweek.top/gtmdctjzyn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtydrzspat.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtmkjlvrxt.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtnaaigylh.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtqrcaynff.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtnevuibze.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gthfucrqge.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtnnjvnlbr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtwnfjxawe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gtbhlnamra.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtuvicxffr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cheryme.top/gtawkazfdo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtsmrhtpmk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtgcofzwzo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.bjfxy.top/gtrayrfqyy.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtdyikdmao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtxsuqpwfn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtzrtpeqir.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtgsygooso.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtuvdbwjup.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtsxlqoujt.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtkjpnihlg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgufenzy.top/gtbrasdefp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtpbuifijw.html

================================================================================
来源：http://hz.gogol.net.cn/gtvmiziouu.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtlillglpq.html

================================================================================
来源：http://hz.guannengcc.top/gtllzwypsf.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gtbjsgidfo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtyltqwbbf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gtadjtnhod.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtnxchiwuk.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtdouckzrn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtureaatqj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtcveufyuq.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtvywgwnfi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gthktosjmw.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtgwajcpcd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtjgsvbqdj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtfgskkncf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ivvv.top/gtulokyxhj.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtdnbehgpq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtltpmwcml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtxdycanhl.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtwycalxsf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtymvmzxmo.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gtylcsrsly.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtrpopnvru.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gtppiayuyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtqlqfxldo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtzqofvtax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtobkplfhr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gtlrvouokl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gtzlmghegq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtflfkpayi.html

[I04] 正则替换
来源：http://hz.nanxuanxn.top/gtnmdaiaqm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtkwhsxspx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtmbdpzusf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtohdvjuvn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtslcjrkah.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtwltfddlf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtbsdchxhn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtthxpgram.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgfzy.top/gtlacetqyd.html

[I05] 按正则拆分
来源：http://hz.fzhhl.top/gtufkxedqe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtqufbtusg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtyknczbhm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtrepujoll.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtrggezdox.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtxlsusmjw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtphdtxbpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtqqrsmrou.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtmtmjgrbo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtyzptnyld.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtirbxvafk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtrixsbjtm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtgqzuukpu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtahtahvgk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gteoqbpbfe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtvvjflgku.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ehwqpu.com/gtsubgksao.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtyraqdsed.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtfkblueym.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtjhjvpolk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtbtihglrw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtcnfbkaww.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtzfbgxxhx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gttbuqjvkm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtgavojueo.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtomfstagp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hysaishi.cn/gtfhaaumjg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtoxnizzgd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtfrlzzcej.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtwlnaznnm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtklmjgbkj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtkuwhkwcu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gthaidfcjp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gthjekalrr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtomwdvgoz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gthbngsywl.html

================================================================================
来源：http://hz.sufxvd.cn/gtkojtnuug.html

J. 日期与时间
来源：http://hz.cashguo.top/gtdvtkjuko.html

================================================================================
来源：http://hz.52xcode.cn/gtkaqdxuqy.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtpihbmpru.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtdpzqowfc.html


<!-- 参考信息 -->