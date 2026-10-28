代发 wailian999

Java: class User {}
来源：http://hz.ywan-chungtsiang.top/gtkvxcfvgj.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gtkzrnvyka.html

Ruby: class User; end
来源：http://hz.ywan-chungtsiang.top/gthmeiydkb.html

C#:   class User {}
来源：http://hz.ivvv.top/gtdttzcqdw.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtxjjotane.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gttifbfnqt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtqizxkupb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gttibtzczd.html

TS:   constructor(public name: string) {}
来源：http://hz.gotoacloud.top/gteccvbjmc.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtwxeaehjh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhengqikj.top/gtiyazmosm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yangfankeji.com/gtrgkekkeu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aibaodan.cn/gthdfomfeg.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtwzrujstg.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtlvucywjf.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtfdewlvxa.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtbfqnsmvd.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtuuiywyjp.html

Java: private String name;
来源：http://hz.gzhubu.top/gttykszldf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtlhcaamyy.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gttquagvqt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtmmymkvwq.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtrqsqisdp.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtffeqguhs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtgexgimgr.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gtearihmcq.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gthqhckcfi.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtoshhvqym.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtmbmewpuu.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtxdpqjpql.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gtpienkdpn.html

[G05] 继承
来源：http://hz.mhx1999.top/gtmfmssmom.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtlthsobli.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtdrqregeb.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtmtgebgcl.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtqnyhjuuy.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtsibdzktp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtnggldlok.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtfcyedecg.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtebijfbpo.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtfaqrusmj.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtxoepxcze.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtpiyjvpya.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtbqxekdjz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtextpigry.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtpjauhvce.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtoigrkwjm.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtnpkalsbe.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gtplawqrix.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gtmvjyndid.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gtrdniepuk.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtzxlmxwsy.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtqnioagse.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtbhenljfj.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtfptcchok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yvedp.cn/gttvwgrlsb.html

Ruby: super
来源：http://hz.nanxinkj.top/gtjyhoyton.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtouskeuta.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtywczhmts.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtyvtmhafa.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtcdzfaopx.html

JS:   static f() {}
来源：http://hz.316326.xyz/gteixocpvz.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtyrybltqr.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtgygwydjg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtkoeekzxe.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtnvamvvsl.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtjlvfuoyv.html

[G09] 接口 / 抽象类
来源：http://hz.gaohongyu789.top/gtpaxwvwmk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtolpgopnj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtgwebdzib.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gteqmgqofl.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtpvhdpjom.html

Java: interface Shape { double area(); }
来源：http://hz.yueranfly.top/gtgsoycduf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtizjpymmk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gthyaqxkkx.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtshswilbx.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtytozdmso.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtlgyzowxu.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtlmqychoe.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtxtqfkcfp.html

TS:   public / protected / private
来源：http://hz.tianlin.xyz/gtlbjxujdo.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtrzkeiepq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtbrivmdsb.html

Ruby: public / protected / private
来源：http://hz.zdqjudy.top/gtbfgcyddo.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gtjllhhbhh.html

[G11] getter / setter
来源：http://hz.ybcxt.top/gtgfgnfmsj.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtimmhpyyo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtsobsuosd.html

JS:   get name() { return this._name; }
来源：http://hz.zhiwuduotai.top/gtxeqrppxa.html

TS:   get name(): string { return this._name; }
来源：http://hz.cqqwz.cn/gtctdabjve.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtzuuspjwp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtddlhtzbh.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtgoxtghjg.html

C#:   public string Name { get; set; }
来源：http://hz.haohaochexian.top/gtaqouauyh.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtfpuysyrv.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtymtazvrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.meibo888.top/gtosytluyb.html

JS:   toString() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtykjxwpso.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtlxnidoaq.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtpnihecxq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtscpakeyd.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtlumzdmkk.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gtetrspfxm.html

[G13] 判断对象类型
来源：http://hz.sufxvd.cn/gtlnlbkapa.html

Py:   isinstance(u, User)
来源：http://hz.yanxiufei.cn/gtupzhytxw.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gthtaxxgex.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtlvzvuaqb.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtdgjzsowe.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gtturhfsjk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtzfbmhxov.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtypyczeuk.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtqmtjfiif.html

[G14] 数据类 / record
来源：http://hz.iojbl.cn/gtdtzfnyfc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtaqwawida.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtbacbnbny.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtzyswnhws.html

TS:   type User = { name: string; age: number };
来源：http://hz.gaohongyu789.top/gtfbsawmzi.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtloxzcncs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gthcmzvsau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gttqqrvzrg.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtzvgunpyq.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtzmownyki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yongpay.top/gtgegvrdwk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtrudrpflp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtlevhgfzr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtatunpicc.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtoovebbhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtpcksqsjy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fengsongda.top/gtzwpbcsae.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtihaholzo.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gthyktsxhu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.snrcjt.cn/gtofoftcok.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtfwlppeti.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtrtogshnu.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtrfzmgpol.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangshuangyany.cn/gtdbfjkidp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtulrohtru.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtrrurpifj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gtzynaafss.html

================================================================================
来源：http://hz.haohaochexian.top/gtijrifbhy.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtlkxlvcel.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtyyaodqhi.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtnrsanoiz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtfkjjytcr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtikmluilc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gttejyhfqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtjgjxotyq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gtgcfgbull.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtbksiewin.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtrutdhslz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guannengcc.top/gtzgfgyqbo.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gttervbpmb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtqhmpboxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtzuldykmj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtrxgsyqkx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtozjxviiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtqaesfchk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtaorhrzam.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gtfvhqjjkc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtfzjddrfj.html

[H03] 主动抛出异常
来源：http://hz.hnxiangtu.top/gtyzpsizma.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gtcwdvlmqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtmrwzhinx.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtypavsrps.html

TS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtztxqzkdh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtbvqomejz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jiagoushi.top/gtkqyrcmvy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhaomingkeji.xyz/gtfjvncrpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gticyhghal.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtpcvffahk.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtxxivcptr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtagiskesq.html

JS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtulgptavu.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtkudsnbvo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtdwfhwqnp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtlmmorcpc.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gttneygswo.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtscesuytk.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtubrceluf.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gttmzzghhr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtekpfyuli.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtgwwwqoxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtzflppppb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gogol.net.cn/gtvedqgxip.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.birdmap.top/gticzqvkoi.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtxerhsqyq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtseiiapsl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ivvv.top/gtfysfbxeu.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigfzy.top/gtamlrfoac.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtocpeykpa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtdwjqxqvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtbubkhmtg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtztrxxjew.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtxekyskpu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nwbrower.top/gtimhjycgm.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtnhfnlrwk.html

[H07] 断言
来源：http://hz.ivvv.top/gtydbbeorf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtacwtbrnq.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtsjxsmwtt.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtphyjcvsq.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtesvpfjlh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtnwctbpvw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gtgrfkedte.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtoxtysbwj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yangfankeji.com/gtqawjzlfr.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtzfbhdimh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yonumen.top/gtnrhnilci.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuxming.cn/gtvrfvadfr.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtksikqiii.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtyvvyzppt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gtlqejjqys.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtgnjpgstb.html

Ruby: e.message;  e.backtrace
来源：http://hz.fzhhl.top/gtntfnblve.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtzgwdkofe.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtuxjcnrpj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gttknnuqef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cheryme.top/gtmranegob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtyqtskypa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtwutpbiwy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtempjrttj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtomgjgtya.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtibwvtiok.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtncutyirt.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gtegmaojjc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtyctbxxwt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtuhicould.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtawuoueoz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtrgakxjyd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gthtcyymnd.html

Go:   defer f.Close()
来源：http://hz.pycfn.com/gtpmdehjje.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtfmgxablw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtczoqycnq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbfwdfaqn.html

I. 正则表达式
来源：http://hz.sxryk.cn/gtgbejbxeq.html

================================================================================
来源：http://hz.tianlin.xyz/gtsfhbhrmu.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtockiqzmo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.havefunace.top/gtiecvcnlv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtczywmfgp.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gterfnktpz.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtokqlfqep.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cqqwz.cn/gtrubguwqc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gtdexlbghk.html

Ruby: s.match?(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gttarehknd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtjngrgbws.html

[I02] 提取所有匹配
来源：http://hz.hnxiangtu.top/gtvtvuuahp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtndhqzvbm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtbzrukemi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtcerqzorn.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtpaglygbi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtygcianab.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtohsotmyl.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtlmpooyde.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtukezvugk.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gturlrjqpa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gteihftuke.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtlpkjzpjw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gtuzdgyefw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gturnpbllu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtfqpltfhw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gtyfnapqeg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtkgtiphkm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtthejdjxg.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtfnglkzfv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtfdwypklh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtphrhnerz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtavduzuky.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtgahzeknc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtanwveaid.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gtkhyndaty.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtditavone.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gaohongyu789.top/gtlukbyfdv.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gtxrnyfbdl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtornkfbxi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gthqzjexyy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtgvdwjyzy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtpmeeokks.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtmnmlsdls.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtebybeqwi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtrtmypyxj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtutxqjthe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.mhx1999.top/gtjvkzmuym.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gteokvomdf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gtkxfaetfo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtkusxwnyc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtldeixtit.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gaohongyu789.top/gtgnbagiyx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtrhiwvrqo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gtbcrsrqks.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtynuiooms.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtpqokxjse.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cqqwz.cn/gtlrkwtqlp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtrjiqrnhl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhaomingkeji.xyz/gtdavfgoyy.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtepmszhre.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtoozoipsk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gttdgzglie.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtognowkcm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtxdnqrvki.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtvoziunmm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtrgniopof.html


<!-- 参考信息 -->