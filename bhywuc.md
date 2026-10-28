代发 wailian999

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtpotrrvjo.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtspyjqhbj.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtsecasypb.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gttnserdvt.html

Java: class User {}
来源：http://hz.zhoulong.xyz/gtiamgclcc.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gtkfweuder.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtsomyzoxa.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtpyahowwl.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtfxacujzn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.c1oappe.top/gttqzueimi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtogccecnj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtqzqaujwi.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtblsjnbyf.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtaemfjbpg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtwtxrsvhf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gtprfcixjd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtufyfkrpc.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtomprhpci.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gttysaufss.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtizocpism.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gthxaevtfj.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtqfnqtxkg.html

Java: private String name;
来源：http://hz.cqqwz.cn/gtflebmehc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtuuwxycnr.html

Ruby: @name = "x"
来源：http://hz.shangyingyoupin.top/gtwuptbmls.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgfzy.top/gtmwdzbtpk.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtaqqchrdt.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtgnmocavz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtqoihcydu.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtheyxjimk.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtjfnatfww.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtuewykuzw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtbfqgjjtj.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gttpmeyoyd.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtwhlzqpck.html

[G05] 继承
来源：http://hz.316326.xyz/gtsippxyzo.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gteimxlmlb.html

PHP:  class Admin extends User {}
来源：http://hz.snrcjt.cn/gtyoawmqdv.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtohkibboq.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtwfzgjdhh.html

Java: class Admin extends User {}
来源：http://hz.iojbl.cn/gtxwunzvhl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pengpengdd.cyou/gtstbvuvhq.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtnvpjpije.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gtzfyywckr.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gtincwuujq.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtophgvmne.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtmjtphkin.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtxogcnuzy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtpsmiwveb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtcqpzopuk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gtyyoinxxp.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtypafnrwv.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtpwcherhr.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gteqveijju.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtjhbcbxxv.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gtfuwbwtuu.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtugljudzq.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtjimmnctp.html

Java: super.greet();
来源：http://hz.shzxlz.cn/gtjpgunukk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtoplddafj.html

Ruby: super
来源：http://hz.fzhhl.top/gthvygsyat.html

C#:   base.Greet();
来源：http://hz.tianlin.xyz/gtegsegxej.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gttfroxzqa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtukyavgko.html

PHP:  public static function f() {}
来源：http://hz.wangdashe.top/gtalilhsqp.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtiizyjtdl.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gttfavrabx.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtjzwljeds.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtfqxzmszq.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtbagxnokf.html

C#:   public static void F() {}
来源：http://hz.cashguo.top/gtdfpsnqpj.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtdggxhlvl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtttyytvcq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gttlpxsfep.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtsmpkkuzv.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtkijqxgph.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtvikdrnit.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xziqi.cn/gtgmiuserd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yvedp.cn/gtabvtetfa.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gtlrztjero.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtdjctjzny.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtobmqtiya.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtcwmzdgdf.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtyrseysan.html

TS:   public / protected / private
来源：http://hz.xziqi.cn/gttwlnvcrw.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtsymbqbnh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gthwxwgtkm.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtcquwrevu.html

C#:   public / protected / private / internal
来源：http://hz.yj202588.top/gtpsgaesux.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtjmqetwzv.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gticnfwqww.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtbkrrynfb.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtdqmteqss.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtlvwocxdu.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtrhzvoskp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtviljrncj.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtmobruriw.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtitseohlh.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtshpobptl.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gthgxddcxm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cheryme.top/gtuggztfzk.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtavflzhnr.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtuucvswgv.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtfcidwpfw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gttortlrrt.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtpvoshyiy.html

C#:   public override string ToString() => Name;
来源：http://hz.daxiang520.top/gtmfvptcpd.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtgxwgxxab.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtfjffagpx.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtgftydoiw.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtjkcscqrn.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gthwomndqd.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtaxkzvmaq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtuyybbijy.html

Ruby: u.is_a?(User)
来源：http://hz.quarkkingdee.top/gtsxsqbpja.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtlfpkdlun.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtyosuxmmf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtywywland.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.0kj1m.cn/gtbapafccf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtvgobmgew.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gtwqknsbbj.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtqcaiehqz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gtrcxicrmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtuabsvkue.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gttbqrbmkz.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtsptndxfw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtiuqktpdo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtorukspzn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtgleafwzo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtfuiwbrel.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtvrlmwtac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtmkyzobhd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtuaojcyqz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtcjnltqku.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtovmfboqx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtzhxhwdyi.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtvnmvamcf.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtntefheho.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtcbbtqtcc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtaavtykao.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtiaccwnvo.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gtxdeljrly.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtqoehrtze.html

================================================================================
来源：http://hz.meibo888.top/gtndizxjdd.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtaaujapsq.html

================================================================================
来源：http://hz.svipenyu.cn/gtpjjhjrsp.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtbnbgsxmt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigfzy.top/gtgjssfmcc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtmpcymuew.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtsuuhiguy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yangfankeji.com/gtekwzcqsg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtuspkroap.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtpnhonagb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtirwzsrcu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtivfsnefd.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtlpgnojtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtgdfvsren.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gttmzxfeqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtyiuwyqah.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtpjjowrca.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gthhbijize.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yanxiufei.cn/gtkhsaafix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.kuanghao11.cn/gtbsvrpigd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenzaomai.com/gthbcsutkf.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtippozqot.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtqaayvplt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtzrliktss.html

JS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtktbkbdwy.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtwwptytko.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtoftsxweh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtawrztqte.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtyzyxlxqx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtmohtstzw.html

[H04] 自定义异常类型
来源：http://hz.zhixingplan.top/gtgiwwcdly.html

Py:   class MyError(Exception): pass
来源：http://hz.yuxming.cn/gttlqvtmpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtoibthwpz.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtkiyqgtea.html

TS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtvkzzqbeo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gttqkeivaq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xinyue.icu/gtnthaziwz.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gtlzyurntn.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtxzwqmeic.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtmdslyyzi.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtduxndslb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gthypmvjam.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtbaninzeg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtxiskzggv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtcgyyixtk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtfjyqyoyg.html

Ruby: rescue ArgumentError => e
来源：http://hz.gzhubu.top/gtyberjbcg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtnrubfekm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtuzcquffw.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtyovuoarj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gttiyhtxff.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gthawwjago.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gttbmobrma.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtbgophuqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gteuuisgot.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtbzzebobu.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gtedbxofde.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtijblnkrw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtbruabidd.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtxmfoxfpz.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtbzarxptx.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtkdiqnzco.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zdqjudy.top/gtcjffucsa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gtsabgoezl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtpdubdokr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gteaqfnxwm.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtvubblggd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtomfrriyj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtvlihgaxz.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gthunecfdd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtyuyxusql.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtezivarxk.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtnnzkdvar.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gttxwdylws.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gttpxxpsmt.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtmahprksz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gthzjhsnks.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gthutsndfq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gttcemambp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtqtsvvfmj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.c1oappe.top/gtdeujfrmt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuetiantiany.cn/gtgurtzvwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtaemqtjax.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gthyxtjnmj.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtuedysemc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtkjzwakzf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtymdyqheg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtigewrrru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtahmzaspe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gttvybhrwm.html

Go:   defer f.Close()
来源：http://hz.snrcjt.cn/gtrlxuqoxv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guowangkeji.top/gthjvghjjr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jiagoushi.top/gtsbtfqygi.html

================================================================================
来源：http://hz.wangdashe.top/gtyqmjiaqa.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtmukyhrjm.html

================================================================================
来源：http://hz.ehwqpu.com/gtdbifgcxf.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtxmgpiljq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtexitayme.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtbxacbgdq.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtgqjwcvnf.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtihukdgtw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gthtcatgat.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtnfhqkgos.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtszkizkfs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtqzzuziat.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtvmmgvdkq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtcnpkqajz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtxwiwnyqo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tian-w.cn/gtmhrbundz.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtyhsulpgz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gttwtochqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtxtgkiqud.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtjjucufmp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtsrgwdmrb.html

[I03] 提取捕获分组
来源：http://hz.jyoumei.cn/gtnuybnawy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.feifeiyinyue.top/gtytfanewo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtjxcguidk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtbweylecy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtwvjmheoh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dianchejie.cn/gtlruqahkc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtfdeljebu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gttrxwupca.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtuupiehxb.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gttopfoogd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtgcxumssd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gttcppabtc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtsmxujydh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtitoseivv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtfcpcetgr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuanzhike.top/gttluxldxa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtmxsvcpgc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtuwnoucnb.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtyggaehqn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtbpgvjvii.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtrdrddjra.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gthcbdwabj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtcllzjhkb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtqleyovtb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtjvhiodta.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtuyjlvpiw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gotoacloud.top/gtpjilovqj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gthnxlbshr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtilhceewa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtbesarcpt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtwzohjwdc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtmvefgkjt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtmabifokp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtlkxvtrcr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtmlgdcybv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtkafaawqi.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtyjtsmplr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtwjpjdbkn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtpzfttakg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtkavyktld.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gtcvfcjhrp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtbeacqlaf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtbudliaby.html


<!-- 参考信息 -->