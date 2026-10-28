代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtftpxjnxp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gthanklwzk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtvrdahpyb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtpcokxryt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaknbcecy.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtqvlqdare.html

================================================================================
来源：http://hz.ybcxt.top/gtotgqvqqa.html

[G01] 定义类
来源：http://hz.zhiwuduotai.top/gtnttcrbbl.html

Py:   class User: pass
来源：http://hz.sxryk.cn/gtgbktfqgb.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtdibdrhax.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtncspxtqe.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtsdrecpsc.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtgwacqsgw.html

Go:   type User struct { Name string }
来源：http://hz.wangdashe.top/gtdogjwyie.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtyszagccp.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtexnknkld.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtfbhnqfml.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtqxwilzkc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ehwqpu.com/gtkczlxtvn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtopvxbiyr.html

TS:   constructor(public name: string) {}
来源：http://hz.cqqwz.cn/gtefnymvrf.html

Java: User(String name) { this.name = name; }
来源：http://hz.yueranfly.top/gtlourpufp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtknniqwjv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtcpstczet.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtyejpipou.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtdfvdjwcr.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtvcsfamfl.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gttxbndgmr.html

JS:   this.name = "x";
来源：http://hz.jianghu66.top/gtqsegzyda.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gthnlcmlgi.html

Java: private String name;
来源：http://hz.52xcode.cn/gtrgbqiwwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtdpjkxszr.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gthqzeghsk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtxgqghzku.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtueloadby.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtwfxdjoow.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtajszzsyi.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtcxxymooy.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtqurxtswt.html

Java: String greet() { return name; }
来源：http://hz.tian-w.cn/gtzpoueltp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtnxqvqexv.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gtgeurcfxn.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtjzptjwod.html

[G05] 继承
来源：http://hz.cheryme.top/gtvfbvydio.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gtgadyoifu.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gttjingnqh.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtbbzrlxsv.html

TS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gthrwupoav.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtyuzfigbl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtuptbfdxy.html

Ruby: class Admin < User; end
来源：http://hz.zdqjudy.top/gtcptprppn.html

C#:   class Admin : User {}
来源：http://hz.zhixingplan.top/gtarisjqzt.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gttdquubjy.html

Py:   def greet(self): return "admin"
来源：http://hz.vqdsnc.cn/gtjhhirxje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtrixuuyvg.html

JS:   greet() { return "admin"; }
来源：http://hz.ydzc1.top/gthidwgehx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtdklukfnx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtrtebaxgy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtviwpqsmu.html

Ruby: def greet; "admin"; end
来源：http://hz.ehwqpu.com/gtwhzlgcxx.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtvesqlnny.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gtwrrtruwb.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtleuyffqo.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gttmgrjjpr.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtqqndogjf.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtahjmwiqt.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtidnopybt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtquklmipu.html

Ruby: super
来源：http://hz.zhengqikj.top/gtealywsaw.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gtqvsasfzt.html

[G08] 静态方法与属性
来源：http://hz.jinqigufen.top/gtlvxkkxjv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtghlqlnmf.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtxzfqajmw.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtvzwxcbmk.html

TS:   static f(): void {}
来源：http://hz.yongpay.top/gtquatulim.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gtpmzaxcwr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtumqaprnv.html

Ruby: def self.f; end
来源：http://hz.cashguo.top/gtamzupegx.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtllcwrqqd.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gtbntwpbpf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtqytnxovd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtfgarewzf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtsrhvceap.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtysxtxoco.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtnptfbcmo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtvbidphat.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtelbnzwbn.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtmsueimml.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtrstfselh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtnsgfrsxs.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtxtubvbee.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtecbgtbrj.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtjognpsas.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtjipakpdv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtaunvnbss.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtcrrmycue.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gtfxjtepgl.html

[G11] getter / setter
来源：http://hz.cucudq.cn/gttrwxanzz.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtghdlrpqm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtdmjyylib.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtakgtkbvp.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gttnmdlikv.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtpdkbrmfp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtnweepfei.html

Ruby: attr_accessor :name
来源：http://hz.nanxuanxn.top/gtnetmgarb.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gtgdthqsuc.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtjbhpmcrv.html

Py:   def __str__(self): return self.name
来源：http://hz.chenlongwang.top/gtppwwmtly.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.52xcode.cn/gthzmgdlrh.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtapwukngv.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtbzgnoyix.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtqbdtznov.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtymoyqcia.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtjsjzjpqn.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtkozcgccv.html

[G13] 判断对象类型
来源：http://hz.daria6918.cn/gtrbhqbkua.html

Py:   isinstance(u, User)
来源：http://hz.daxiang520.top/gtlxbrjlpp.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gtchzjglli.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtbwmkdhdi.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtzchvqjzx.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtbnblzezv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtyprspeuw.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtolozpuhf.html

C#:   u is User
来源：http://hz.zycfv.cn/gtkfyqduyz.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtrpkakwec.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtluxpkxou.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gttojyydbf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtwemlrokc.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtguzzfenc.html

Java: record User(String name, int age) {}
来源：http://hz.0kj1m.cn/gtgmatatzc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pycfn.com/gtjbpshmyt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtbnvfcjuj.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtfpmkpdev.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtdwmwtjdo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gtvqomepex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtytotbvbj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtgnzrcrjk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtkgxcyojx.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtrcdpmqci.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gteeacofev.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtuuaubach.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtvyqraiyy.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gtbxbzlasr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtppxbzaki.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtegqbdhws.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtzuajfdnq.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtimzpbynn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtgnpjisxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtvetwgwxg.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtbetfchlm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtixnsszce.html

================================================================================
来源：http://hz.jqgfzy.top/gtjlmijidk.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtnqsnosqw.html

================================================================================
来源：http://hz.shzxlz.cn/gtqebkdubp.html

[H01] try / catch 基础
来源：http://hz.zhijiandao.cn/gtujmtntgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtagffcnfb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtoqctxmwo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtlyodjgrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gthwlrymwr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtpdgqirhi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtvfodahfv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tanke756.top/gtxgusnmpi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gtantzgcsx.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtngygdidv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ywan-chungtsiang.top/gtbfqqsawh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtraigvtdc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtsildsitb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtgviwsdwm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtebegdhcg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zycfv.cn/gtsxzojrla.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.haohaochexian.top/gttjznjlnm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gtwkbrzhau.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtpecupflh.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtzkcqrsoo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtsuvnuhuf.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtnrusvqsv.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtitapcfjw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtafizrtdz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtmkrfiwzq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtlictpomf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtsmkanwrh.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtqhtundyh.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtjlvfycui.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtqeqxcbiw.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gttdpjcoax.html

TS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtpsryplqf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtcmvpyoei.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtoozlikdl.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtnefjfndq.html

C#:   class MyException : Exception {}
来源：http://hz.andypj.xyz/gtzuqjuedi.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtjbxcuznj.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtkaymvkqz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtaekuokrl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtoclhxhch.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtxpferlwt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtlkdrimqf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gttxxeaaqz.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtvhhvngxe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtkgudhhnv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gtujobuiuy.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtzwggbkkx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fengsongda.top/gtjrkjerur.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtfgvmgqol.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtggxrgenr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gthzaaolqs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hammf.cn/gtzoahbfhl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtltqpjlln.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtolknjcqz.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtdxdqmbue.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtrhcbxpnx.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gttudokktb.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtzosmglde.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtodtbzfis.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtasruwlmz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gttcanwaqp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtsxkwypkh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gttkvbsoeh.html

[H08] 获取错误信息与堆栈
来源：http://hz.cashguo.top/gthjbfrsds.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtjoeuwybn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtijqehxjm.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtfiewbyvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtddfkbuck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.quarkkingdee.top/gtitvjmkxb.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtjvpoaduc.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtdznhthcr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtuhcdxopp.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtpmvftxpi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gtkhfmsgjz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gthhdzsnlf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtjvmmcndq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gtbsedaxon.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gotoacloud.top/gtfacwbklv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinyuanbaomall.cn/gtsyqforxm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtkmcpgyns.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gttpaflzbd.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtgayqnznb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtjkehhmmh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtmnclraif.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtjmkqrzuw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtkolfcdkv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cdnleiting.top/gtlmdzonmj.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtehxrwkbe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtluyjdkgy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtquyrzmya.html

================================================================================
来源：http://hz.jinqigufen.top/gthsharfus.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtqcampbzf.html

================================================================================
来源：http://hz.cheryme.top/gtdlugalvw.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtdqifrxdi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aizwys.cn/gtzlldohao.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtyuedlxye.html

JS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtwnvbtzvm.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtkrtpmijv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtatzlfltf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtpdtqaexj.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtxkudmpfw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtoakjwbvm.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtglfcgemh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenzaomai.com/gtvlsngafn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtlkfxmcpp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtcyfzezil.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtvbrvncxb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtbxpqwbrj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtjkpuyuqk.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtflvkwhof.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtpyqtblwl.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtjidwykxc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtvtvumnez.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtjnzmkhjj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtjtnkztnn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtdbpygbzw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangdashe.top/gtnsbivzfy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gthzxlrbdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtmbdqmiee.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtiwbknjky.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtnxcdjvmo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtcovmnhcd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtlvmzvqna.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtommxyvri.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtznttnqpv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gteitmytln.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cqqwz.cn/gtzxhqaqag.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gthvwxwqvh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtdcepidiq.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gtoofauogq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtutkrbvvs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gthityldny.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtmybwxuff.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtevpjpuxe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cdnleiting.top/gtdhhuqaym.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtjovrubbf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gteotoebck.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yvedp.cn/gtyerjozuq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtjbwpnvss.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtzmknhmur.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sysykeji.top/gtibduyncq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtdzdaddbv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtgdgpddsl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gthqxzhuqh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtozhppckx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtxutoviig.html


<!-- 参考信息 -->