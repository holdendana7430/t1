代发 wailian999

JS:   this.name = "x";
来源：http://hz.pycfn.com/gtbixmfbvi.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtenjgnlbw.html

Java: private String name;
来源：http://hz.cashguo.top/gttpeulzcv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtfocjiumm.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtykludnhk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gtlpuzgblu.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtaydfgomb.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtixwbdxtd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtehtwqcnj.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtedaknlyv.html

TS:   greet(): string { return this.name; }
来源：http://hz.fengsongda.top/gttllxrmfh.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gtsmbtmpuh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtvabgfnkx.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtoljzrqnd.html

C#:   public string Greet() => Name;
来源：http://hz.yongpay.top/gtwovkkwuw.html

[G05] 继承
来源：http://hz.cqqwz.cn/gtcsoojris.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtuiexkfyg.html

PHP:  class Admin extends User {}
来源：http://hz.zdqjudy.top/gtdnxstnfa.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtvzfoodbl.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtbehfgejt.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtyqdgcbhj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhiwuduotai.top/gtdlvvzhya.html

Ruby: class Admin < User; end
来源：http://hz.fzhhl.top/gtrhhvsmxj.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtexgejbga.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtbfyiyazp.html

Py:   def greet(self): return "admin"
来源：http://hz.guannengcc.top/gtxdimyemu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gthogfuokd.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtanfqtnby.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtdfluhfmt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtqxymukxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtqanarmpr.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gtqseyzgrz.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtabraswvm.html

[G07] 调用父类方法
来源：http://hz.hywenlv.cn/gtaoabhvsu.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtbuvawlvo.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtsablitby.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtrbdfulcx.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtbbmnqlcz.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtxtttaeln.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtihzqtvwp.html

Ruby: super
来源：http://hz.daria6918.cn/gtvthsnvrw.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtzywtxcha.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtxmbzokxk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtaeufkxah.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtwshzirzs.html

JS:   static f() {}
来源：http://hz.zhixingplan.top/gteggrsbjz.html

TS:   static f(): void {}
来源：http://hz.zhengqikj.top/gtiterseyt.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gtznzznxhf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtcjuepqoh.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtivovvylh.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtvicbrlql.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtrqhbhhro.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtlceyemow.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtnghqtymu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cucudq.cn/gtdevoqovw.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtcmfqykno.html

Java: interface Shape { double area(); }
来源：http://hz.jiagoushi.top/gtzuttnfzk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtitxqiryj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ywan-chungtsiang.top/gtsgzeyqja.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtufakkpgm.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtzqgwwnqw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gttveytuec.html

PHP:  public / protected / private
来源：http://hz.daria6918.cn/gtivbkxtya.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtafjqojqg.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gtkttpqhhn.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtjvnvrbxd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtmdyhrzha.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtnqhcpdkb.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtihyikcox.html

[G11] getter / setter
来源：http://hz.jinqigfzy.top/gtsshokrgf.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtanuwoqai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gthnpxnvut.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtrvynvsdc.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gthsvykeig.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtimztoedc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtfucfcrib.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtwbbniccx.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtnbkgdocl.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtsuytuvvg.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtiexvismu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtxnuhjrmh.html

JS:   toString() { return this.name; }
来源：http://hz.sufxvd.cn/gtougbdiji.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtufybdgxl.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtxmzjerhs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtghchbfix.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtkyuscyjf.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gttusnypbq.html

[G13] 判断对象类型
来源：http://hz.jinyuanbaomall.cn/gtsaegvjcz.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtvzgmyjkx.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtiilxvthy.html

JS:   u instanceof User
来源：http://hz.xziqi.cn/gtckypeiar.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtjojfmdgg.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtkntucwbw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtqmqdsqcz.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtrauvllqf.html

C#:   u is User
来源：http://hz.iojbl.cn/gtgxuvrjdl.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtrijdlqvx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sxryk.cn/gtweatnjgc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtpboctqlj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtngxbbhxy.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gttpsvuske.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtnnoggdnm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gthxmljnia.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gthzvmenuy.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtotalyjoz.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtoktqnkka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gthtcdmtxm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtlaoaqwte.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtnculexve.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtjrbclxvv.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtequxrgav.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtpowsbfpx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtulakxsmd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtopidwpvc.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtsmfbhwvp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhaomingkeji.xyz/gtarjsejsz.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtcyfojzmh.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gthunbrmff.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtaesfczfx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtsspmxsdg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtsbnqznmr.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtxvvfujbn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yvedp.cn/gttfhjwiba.html

================================================================================
来源：http://hz.tian-w.cn/gthrdtbogq.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtqdlpydzw.html

================================================================================
来源：http://hz.zhengqikj.top/gtipzllxtm.html

[H01] try / catch 基础
来源：http://hz.sxryk.cn/gtvvjznlmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtwsavxugm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtrcunlfff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtrrnidaih.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtbjclqlme.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.havefunace.top/gtzsavcekf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtmgnnbouf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtaspxtlhe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gthntaldzy.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gteshbyhcv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtfjlzyyls.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtnyjraupo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtwzajqiee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtamirnkiz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtaifgavcb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtgneoieey.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gtcgeeoryz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtirqypwll.html

[H03] 主动抛出异常
来源：http://hz.snrcjt.cn/gtqywodsqs.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtsdpnqjih.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gtzzopxmkk.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtpvwemqfo.html

TS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtybxnhbek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtrubxddmj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtipnxaivi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gttrneehdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtzwidtcls.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtwzgbclus.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtsezgeajs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtclpeezip.html

JS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtqqrqjhwg.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtmfafobok.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtenvxgbht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtytqfamax.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenlongwang.top/gtdldojmbg.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtvuxsgmht.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtjgmthqng.html

Py:   except ValueError as e:
来源：http://hz.zhoulong.xyz/gttrdpemvu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtzzwosuri.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtlyqtzztj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gteaculhec.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtvqlexfpo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.havefunace.top/gtjfgqsxky.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhaomingkeji.xyz/gtmqlqjpuk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tian-w.cn/gtuxdmwxtc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gteesulmee.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtdbflsila.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gttwkzgifu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtumrbqfpa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gttlzetyen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtpxsegmsq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtsvgtlson.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gteglwvlhx.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtfbiotnrf.html

[H07] 断言
来源：http://hz.xylfe.cn/gtdjalwgfm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtuuojvhjy.html

PHP:  assert($x > 0);
来源：http://hz.c1oappe.top/gteouqbssd.html

JS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtvriligxv.html

TS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtotqdgjpj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ppjwa.cn/gtyldkpipf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtrbitbwbx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtlxzcvkbf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtwcehddkv.html

[H08] 获取错误信息与堆栈
来源：http://hz.aibaodan.cn/gtofrwplut.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtyrbfyqxa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cqqwz.cn/gttgppbnyt.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtdzhrmoqi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtfqhrietc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtvfjfvlzm.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtjnxqpcjp.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtttphptje.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtkpfidhsb.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtvrvfivcv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtriloujem.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtxfsjkkzm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cucudq.cn/gtrmarflgy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gticnoongc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gtlkeedynx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtekafsonf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yonumen.top/gtcowkbxpw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gthjiyslct.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtakthfneh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cucudq.cn/gtpbstgizs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtediybrua.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtynhxjhmk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtwiwzfpdh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhengqikj.top/gtyiwtlshi.html

Go:   defer f.Close()
来源：http://hz.fengsongda.top/gtenjdpbcj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtdobteses.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtmrelqoot.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbrtppqda.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtwfgnxirq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrbkcdfod.html

[I01] 判断是否匹配
来源：http://hz.meibo888.top/gtsmwlfswk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtymwfigpy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtmysmzdfq.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtrwrgigpv.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtbdgqsmko.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtlstxoodh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtnkvvqonn.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gtdyknzups.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtayhbizsv.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtgdfgnvgo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtqwuumsck.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtkbuytkor.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ivvv.top/gtwylhubzl.html

TS:   s.match(/\d+/g)
来源：http://hz.hnqzz.top/gtrhvnoeek.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yueranfly.top/gtxhebynvu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtmdrgfjau.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtoyigtraf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtojqsjfyu.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtaqetackd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtchevnirx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtoywpezkw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtqhjcpiss.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtoinvumaa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtxshfyqig.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtokuudkcv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aibaodan.cn/gtwdcwigwa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtxfowttjh.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtegfmfkwe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cucudq.cn/gtsbwzclyl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtyfyxnovb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtuzuqvnof.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtourbihqt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shzxlz.cn/gtvxzcpqma.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtgqccwtdl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtuhyieoua.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtveqfqosm.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtdvpckvtx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gogol.net.cn/gtocrpfyun.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtuxmfvsta.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtjroymxcf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtpwtsyfey.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gtudbrxvpl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtcxdzcfak.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtsixiwcti.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgufenzy.top/gtcqxuxmhf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gtjcmahccz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtpvkgqofu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtuhahkydj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtixugvjav.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtxdtmelfj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtdllhaimx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtuzpiuhjl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtreglmcey.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtolcruvuq.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gttapyrppz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtvhvtkwca.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtlueiqjgr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shuidangran.top/gtnrevlluc.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtpndysnag.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtqijdbtdp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtilagzlug.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtkmxnqwmq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtktxysfie.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.birdmap.top/gtjqlfghtm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtmuibcjvt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtyszwgpmq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtitaynjlv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtwyhprioz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtnuwobujy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtlwjaldqo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gthjasqfwa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtswcscfaj.html

================================================================================
来源：http://hz.hywenlv.cn/gtvnbqeosl.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gthngfxhjd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjcadzzhx.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtemfjrsnu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtecblcjpo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gttxtmqkwr.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtgwwzersr.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtoiiyxqkl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gthtotgdce.html


<!-- 参考信息 -->