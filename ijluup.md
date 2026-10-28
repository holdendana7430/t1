代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtkdlpkhwp.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtxkqeiymj.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtnjtuocos.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtyubnghyf.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtbjtyzoob.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtzrjknkwq.html

Java: private String name;
来源：http://hz.ydzc1.top/gtzqhnzomu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtsaxvimwu.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gtqfdrtqaf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtbqmexmqo.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtvzkjrmzm.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtafctmdmk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtawwptfbc.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtghuyjfsg.html

TS:   greet(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtaqzfjssc.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtkvnopfzn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtmhuouuen.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtyrjplgac.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtjzrpgbtc.html

[G05] 继承
来源：http://hz.pycfn.com/gthdmzusns.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtygpuhzyo.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtexrenkje.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtsfwefccb.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtsvqujiek.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtlwlculzw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtnijzzcys.html

Ruby: class Admin < User; end
来源：http://hz.jianghu66.top/gtjmihazmf.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtfdbnqqjb.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtxvafpeen.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtccvzsbeq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gttuiljgoq.html

JS:   greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gttljcwmup.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtgztqnqvl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtcarnsbyk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtcdumsrxi.html

Ruby: def greet; "admin"; end
来源：http://hz.hywenlv.cn/gtjdmhwtol.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gtmhltvrgv.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtqmycypsf.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gtbszczctr.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtrhnbhnwh.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtjfovwvko.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtychvzzru.html

Java: super.greet();
来源：http://hz.yj20258.top/gtcaimdvid.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtbyjqgohw.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtmxgyuexa.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtzvgowgyf.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtyydlbwmi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtvowmvlae.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtghkokjjm.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtauvahzkg.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtftenipgb.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtgfiyewbl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtyzfoqaww.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtbrdyaqau.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gtboduibet.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtifwmyfby.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtgfvfnlqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtthfxlamw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gtbpsqspet.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangdashe.top/gtxopdicoc.html

Java: interface Shape { double area(); }
来源：http://hz.havefunace.top/gttxarpztb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gzhubu.top/gtosjljwam.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtjfacnljz.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtvkhlnsco.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtelutbxrn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gttiqqhzrw.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtdgbowrvv.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtsusomgbm.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtelglbvio.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gtdhigdiyt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtfdeqpxyh.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtvzrfdhig.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtopldlruo.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtyhswadli.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtszsxpiam.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtzvxloedg.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtwjgafrun.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtlrikikdv.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtbjjvtavr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtcyoovecx.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtcgvnpjny.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gthrxasvjq.html

[G12] 对象转字符串
来源：http://hz.vqdsnc.cn/gtvljzthsg.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtvmvvxpuu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtfpoeyrxk.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtefrfftjz.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtnayigzfz.html

Java: @Override public String toString() { return name; }
来源：http://hz.guowangkeji.top/gtvzxxiboh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtpkmtsusn.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtjpdxerap.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtbvzchbqu.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtinieumre.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtgnysurao.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gthzrplzab.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtdssiirsx.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtmwokhykj.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtpzqurofq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtmflbazim.html

Ruby: u.is_a?(User)
来源：http://hz.xziqi.cn/gtiqfkqfir.html

C#:   u is User
来源：http://hz.hnxiangtu.top/gtqjtbnrvw.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtzymaywbh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtfuaivcha.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtirpbczvf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.bjfxy.top/gteffgmgzh.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtxisumnyg.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtilqqjrxh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gttrpztzrk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtbfkvylcx.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtlsxxhsha.html

[G15] 枚举
来源：http://hz.ivvv.top/gtqnvysnvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gtauvfrcgu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtegtbjarl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtbguzsunu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtiuapqgbk.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtxomokebs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gtjoxlrppz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtphzbuguj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtbekntbjx.html

[G16] 对象转数组 / 字典
来源：http://hz.dashuyun.cn/gtgqkleyex.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gotoacloud.top/gtsvfnzdms.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtscayammk.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtopsapznz.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtttdkzpnm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtdkybwlla.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtdcxwsbnf.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtvatzrkft.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtrsnkaulq.html

================================================================================
来源：http://hz.0kj1m.cn/gtkufsirom.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtgavyecxw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvzrqenty.html

[H01] try / catch 基础
来源：http://hz.hongshengwenyu.top/gtxvucvjeq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.bjfxy.top/gtmzkfxedx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gtvhswchbu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtvupvrzst.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gotoacloud.top/gtiknimwdd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ehwqpu.com/gtzzbjokik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydjk.org.cn/gtbkoakflu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtsmxdyrbc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtuswceajl.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gthumedwan.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtrcfnkhdp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtegwhejnc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtknozhhrv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtygzfgsbj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtgmvycida.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtchjwddot.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtyduibgsx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtxdjmsfsy.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtbjvywzaz.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtbhtwadkk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtexlcnhet.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtvkzfsybq.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtaxghpfuc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtjwcrsqoy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtnqbkypio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtfnjsdarj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtezcxylwp.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtxkddlzwg.html

Py:   class MyError(Exception): pass
来源：http://hz.hfpthk.cn/gtczwoaloe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtyjkbvadx.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtetcyqiwm.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtiqeowmgt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtjzcfiniy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtzixcbydk.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtnngqzcme.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtxwxlucys.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtwqpnvrmo.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtounmoacu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtnjodsvdq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtgyigrfmm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtwmmkukhs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtgugbpikk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuanzhike.top/gtkljqdgrt.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtwhjuerze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtqqmefmiq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtuivnlzei.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtebwjkymg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtvlfnkqvs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtfnuvbrhz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtcfxnhdnf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtlyhevotm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtnqqadiue.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtdgkyeilx.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gtwpkymgay.html

[H07] 断言
来源：http://hz.yj20258888.top/gtmvlvsvat.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tanke756.top/gtjydnypbc.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtcpqguets.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtbpdnxbda.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtcjwhxnhq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.bjfxy.top/gtsneshmve.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.9152youxi.cn/gttaatikds.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtzdthvrmk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtwhyjyrjc.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtzplcwogt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtaujfbjzh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtbthokyti.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtcctqwtgl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtbnibwuch.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtbjiqmudd.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtyteunpzs.html

Ruby: e.message;  e.backtrace
来源：http://hz.dashuyun.cn/gtzypcdbel.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtroyshthl.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtkgvmernv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtnyullkmx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gtfyibdcbc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtbxuzeyjs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtpzpqftsn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtwdfbtwtm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ivvv.top/gtxrkhrpnj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtnzosgazk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtpmyiwsks.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtlmbegkqy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtkxqissfs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtnhzulesy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtqydxxdtv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtnrlorzke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtfrfugrfr.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtihbhusqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jlsjyb.cn/gtnfwqqebg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtquvsplav.html

================================================================================
来源：http://hz.aizwys.cn/gtaifpvwef.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtlhgvfxpp.html

================================================================================
来源：http://hz.zhengqikj.top/gtulknlico.html

[I01] 判断是否匹配
来源：http://hz.chenjidiqi.icu/gtajiuhnkn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yongpay.top/gtrpotokco.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtxptomsan.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtgwccfyks.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gttlwtngkd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtniuoaipd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj202588.top/gtgbviiann.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gttdmiwgld.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtuggkoavu.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtdmuevldm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtcmkkbmuk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtbblwqdsf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cqqwz.cn/gtyeywbxxn.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtrxlkskvv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtimsofmmy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtjhagnvsu.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtjsquskwm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gttsefvocz.html

[I03] 提取捕获分组
来源：http://hz.snrcjt.cn/gtfyzjjeho.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtlsxdswqf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtxvdpjtim.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtgvamiter.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtvbzbgtyk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtqgetcyeh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtelaflpqz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtervpyyzn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.c1oappe.top/gthvyxphuu.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtgcemgakb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cucudq.cn/gtttkczern.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtatxxayla.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtzhugsbsm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtvbqzfxpm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgufenzy.top/gtosrhfyqn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gtjamtwplj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gtpuaboquu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtoixlrrme.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtscuuvjxh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtseachqkc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sweek.top/gtrlvdysjk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtallhprno.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtmfuugzcw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtiyywjpci.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtdaeafxcw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtkmmdswtp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtamwzyebt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtlcydoxrc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtdskwryff.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtoksxmrab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gthiuihbxo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtligkgmfh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtptbjtzbu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtkaqagqpb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtyrlzzcqc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gttdyocvce.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtmsunqwyk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtvopudagi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtmeeobnsl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenjidiqi.icu/gtyfaqpztu.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtqqxprexa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dashuyun.cn/gtgkdvafda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtscogfdsm.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gthitchvna.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtdcmxfaem.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtsglqeeii.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtxbvnjbgj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtnwqrzwrr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtfdiiiilj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtszhavgjc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pycfn.com/gtmzbjpeei.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gthqcefqfb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtdpadvfhy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtzrqagidk.html

================================================================================
来源：http://hz.fzhhl.top/gtzgcnjlms.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtdepccheb.html

================================================================================
来源：http://hz.sweek.top/gtivmehfat.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtlcewfzms.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtugsecytz.html


<!-- 参考信息 -->