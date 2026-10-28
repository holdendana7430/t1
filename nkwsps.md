代发 wailian999

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtwkfixeie.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtnfmrnhga.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtvauhsqes.html

TS:   class User { name: string = ""; }
来源：http://hz.havefunace.top/gtyvlrzhpj.html

Java: class User {}
来源：http://hz.yj20258888.top/gtclvzdtmu.html

Go:   type User struct { Name string }
来源：http://hz.pengpengdd.cyou/gtrmderyrj.html

Ruby: class User; end
来源：http://hz.jyoumei.cn/gtvvdqdgkf.html

C#:   class User {}
来源：http://hz.fzhhl.top/gtekorspef.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtdlttytpa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtsdoetdxr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtcmstnawp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtttpqtgjx.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtbxwnncku.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtzwnyvtqm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtyfhkqlqd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtvsjmlapb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xinyue.icu/gtmggmleru.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtnfccbqwt.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtwtndyqoe.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtptxyouwq.html

JS:   this.name = "x";
来源：http://hz.nanxuanxn.top/gtkyaqkywn.html

TS:   name: string = "x";
来源：http://hz.jinghuilouyu.cn/gtliczvgtt.html

Java: private String name;
来源：http://hz.yj20258888.top/gtjginjhrh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtnwdyebcb.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gthlaikyuh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtyokcrhgz.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gtbcdnkdrt.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtfmkiaxgj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtvfglhodr.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtiedytnwq.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtuladhsjn.html

Java: String greet() { return name; }
来源：http://hz.chenlongwang.top/gtfzdpdnsx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtyfpiogcz.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtyokcsonc.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtifemjivp.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtqoutprpb.html

Py:   class Admin(User): pass
来源：http://hz.hywenlv.cn/gtdochjtqa.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtvyqtynbo.html

JS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtdbhqouhe.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtuhrgvibt.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtaprfxzat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtqdwlljgk.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtougdjqgr.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtwtqjulzp.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gttmlnbyuh.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtigwrjsii.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtduneltur.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtwiyobijt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtjjgosuyv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtdonludsn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtwemnxias.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtterdkxwc.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtjpygskxz.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtnbdmzori.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtlkzelmlc.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtrmjafayo.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtycjhoezj.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtblwtjuxg.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtkrcvbtlg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.andypj.xyz/gtcslebeoz.html

Ruby: super
来源：http://hz.xinyue.icu/gtshlnvpin.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtxevujgtz.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gtgsdawyxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtwqwnakpk.html

PHP:  public static function f() {}
来源：http://hz.haohaochexian.top/gtkrerutio.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtayglrhdb.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtdjbdreej.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gttyhocwya.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtnglpkkfx.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtywhqlwgn.html

C#:   public static void F() {}
来源：http://hz.ywan-chungtsiang.top/gtmusjugcu.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtonpailhz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gteqjxxdpt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangtech.top/gtxthjkaqa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daxiang520.top/gtnpffabfc.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtmduedjjn.html

Java: interface Shape { double area(); }
来源：http://hz.52xcode.cn/gtwrcclumb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gtitpgrwiq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gthxlfzdaa.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gtmkhktbdp.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gtvsxylshn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydzc1.top/gtnulzuszv.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtxwqlqzdy.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gthajvrntl.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gthuoqqeky.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtqcvecske.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtqbeihwym.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtwbmseswj.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtkmqupqku.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtghnzuvby.html

Py:   @property 与 @x.setter
来源：http://hz.yvedp.cn/gtklfxsdnv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtusayflah.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtjuutapmt.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhixingplan.top/gtlukwlzfa.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtpcasqvfy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hysaishi.cn/gtivqhuqjj.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gtadtgfvhf.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtjobkuatf.html

[G12] 对象转字符串
来源：http://hz.wangdashe.top/gtrrrnujkn.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtycfipkhf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gttzcijngk.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtwbvagnlb.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtamibstyd.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtoltxxjaz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hysaishi.cn/gtijyrihwi.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtweprmikn.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gtjvzcgkjn.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtxdtdvjvc.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtuvzkujke.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtihyauuhk.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtmglwfitk.html

TS:   u instanceof User
来源：http://hz.sxryk.cn/gteluajvgu.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gthjhdvbxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtuayfkfpm.html

Ruby: u.is_a?(User)
来源：http://hz.fzhhl.top/gtdhruuopv.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtlwuphtpx.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtyupbrmfx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtdovsppue.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtrgtikvcp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtagtukwnk.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtcghoeuvg.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtcakhfvzm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtdvhvhsvi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtpswbhnnm.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtowihbtom.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtnobxisjp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhixingplan.top/gtepgqbcqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtfiyioaqr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.0kj1m.cn/gtybtpawlf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtvffyzsek.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtwmsycwbi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtnooqhnlk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtczzfsgvz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtiaqovrrx.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtczcvmmns.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtwlzsflku.html

PHP:  get_object_vars($obj);
来源：http://hz.gaohongyu789.top/gtntvxyalj.html

JS:   Object.entries(obj)
来源：http://hz.shuidangran.top/gtyoihwpob.html

TS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtykrydmwi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtycosmrki.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtomtecjzd.html

Ruby: obj.instance_variables
来源：http://hz.shangyingyoupin.top/gtdbzgoywo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cqqwz.cn/gtxykbttqy.html

================================================================================
来源：http://hz.xziqi.cn/gtizbzbqfo.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtymdzagiu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxcfxynus.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtvbdzimof.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtzviovuiz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtdjdflrvh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtwrmdqvbu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtwokqgzqh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtkncweqif.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtlzgntner.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gthsqwsgsd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtoccueuub.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtymkalvzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtadnbunlc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtwlnfwyyd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtgdahjxar.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtqihpcnag.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gttxluvmmm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtzdbyqxrz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtqzgvzmvc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtbmdfhfor.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gthzilvsun.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtdlvacbzk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtojjtxdgu.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtpwgrqjmw.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtzjmhpvlw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtkxciiwrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtmbzrapqg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtcqwesjbk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtykgonpdb.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gtabwcavkx.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gthfqggdxt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtxovrowau.html

JS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtwijpbjzi.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtbayctuel.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtpffhmhta.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtuzkwbzyy.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtfjakmhjz.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtmwotjine.html

[H05] 捕获特定类型
来源：http://hz.ydzc1.top/gtovmvxvxs.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtxoimmedj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtfxexhbqp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtbibeaalm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gttnoyiyop.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gthnnmmgzq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtsaoqiwsn.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtweoxnfbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtqrcndqko.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinyuanbaomall.cn/gtrzucczsy.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gtlmegpfyw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.redwolf501.top/gtaormknos.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtwpkljxod.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtszdkfpry.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtbnnmpofk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtrsyqbiei.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aibaodan.cn/gtynwueexa.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnqzz.top/gtmvrrfbjt.html

[H07] 断言
来源：http://hz.snrcjt.cn/gtglpuruhw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtdntbjngf.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtabbagtye.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtpkixdvod.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtjstsjxpo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtdfgcyott.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gtshscuwyl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtdspzeher.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtwwhbvafy.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtxvwnqlga.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtjeftkymd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtisnechdk.html

JS:   e.message;  e.stack
来源：http://hz.iojbl.cn/gtlzulxemt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtfyzohaxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtroudtjhb.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtlygfbysg.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtsnellkmf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtbhzckcmf.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtfqubdlik.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtvnvlrglh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtqyxdzuzb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zycfv.cn/gtpqbnbiiq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtkilcwnup.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtulivykfe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtnamljjng.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtlexvbtoo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtcuxjdppl.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtwhqyxwzq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtqlcpeafw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guowangkeji.top/gttodbmjom.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtrevolgde.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtfwqgkuzc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtkqwtyeeo.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gtufgrqkpv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtugiaupyv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtabtlzsdm.html

================================================================================
来源：http://hz.xziqi.cn/gtxwkjhuov.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtnqkdlegb.html

================================================================================
来源：http://hz.cqqwz.cn/gtgtqzkbgy.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gthlmgoyzy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtbjgeusuc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtvdnrkbxm.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtdtoeyhrk.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gterzirtxh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtfmyriytq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtshxxqono.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtzavogdpo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtoqdqskli.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtvepethna.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtymvopeet.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtdotaaiba.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gttnmpwowf.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gtjuqswghs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gzhubu.top/gtjxipibdd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtwlywfnqa.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gtaodvcyst.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtoyxpkerk.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtmxuazzhm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtousodphe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtmkmazfeh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangkeji.top/gtocrzfkne.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtmwrjkfga.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gtfcrekryu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtjuvbixib.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtpujzexyz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gttmopcgte.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtrvhiaxdt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtnedvxxur.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtawmpgoeo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtwfftkeka.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtbsythssi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gttriexnma.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtcudoeszc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtvqujhtnr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtyqbjhbzi.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtroqpfnfd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtzuwltgsa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtuamanjsu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtouwyqbde.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtvznvzamw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtscgibqtu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtidvhsjub.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtujykfogy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtqrfqfbqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtmaraxynf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtxnttgclh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtgcrnreov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gthroauuka.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtsebuaaug.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.vqdsnc.cn/gtfrtqyvkt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtsqqmdtqf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtprbvacos.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtgnyuktxd.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtocsrnitx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtldrmpwkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgfzy.top/gtjgnqvtrm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtsffwxzbs.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtjuliwgkb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtqrfrnijc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gtgqrnbxmp.html


<!-- 参考信息 -->