代发 wailian999

[G02] 构造函数
来源：http://hz.shuidangran.top/gtauqahndl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtifsxpibr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gtfwpfclrv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtymjdrfqg.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gthaujaand.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtmcxvuehz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtqdeondlf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtarlskjzu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gtdqzkqzfy.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtnyosclxj.html

Py:   self.name = "x"
来源：http://hz.vqdsnc.cn/gtyroqvfcz.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtxnlqzmbv.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtaxpjwwuc.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtenjyonae.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gthbosadfv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtxbkszqqi.html

Ruby: @name = "x"
来源：http://hz.ydjk.org.cn/gtefyxeryq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtdardxwkq.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gthsufgkql.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gthadymort.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtwfkmrkbs.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtbilddgkt.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtieqpgxgq.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtuonhygzq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.haohaochexian.top/gtuzmcciei.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtgpxwzuqu.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtbgluxkvt.html

[G05] 继承
来源：http://hz.iojbl.cn/gtoasaxsfi.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtjwakqbok.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtpdzrdzer.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtieljhnte.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtulhpggxg.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtdsnfwkej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtzemugnqp.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtvvwzpeys.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtwofexdrv.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtpglsivrz.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtdjrsumub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtqrjjcxgt.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtnvjbuabe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gttfcsxaiw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtggfxvbad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtzgltgoto.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtpjzzmvdy.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtijvytbcl.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtfhjftkld.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtdmdfpswx.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtmzpbptmm.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtckvibgye.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtrluqmywp.html

Java: super.greet();
来源：http://hz.c1oappe.top/gtkufwyrds.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtiqkvtqoh.html

Ruby: super
来源：http://hz.jinqigfzy.top/gtamkqtrac.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtzemdpqgz.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtqkzguagj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtjnmvotcl.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtybsejxjt.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gthprqlwci.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gttbohcbvf.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtlpnituks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtqufuzasp.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtmduuvjne.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtijfsomff.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtqhnpqjhd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtzsfdsvpv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gthbjcujhw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangshuangyany.cn/gtvbzbktic.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj202588.top/gtyuroqpum.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtctwjclqm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtzaiyayrj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tanke756.top/gtidhgltix.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtenuxdmog.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gthqjcbzgm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtfhlojovf.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtyekaqsmd.html

JS:   #private 字段；其余公开
来源：http://hz.jlsjyb.cn/gtovlduwuz.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtucaexgjc.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtzvkoavxp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtaykqgdyg.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtwzayxjyh.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtyvbjvugs.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtkpzrbymy.html

Py:   @property 与 @x.setter
来源：http://hz.zhoulong.xyz/gtooqkxxiv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtjqymosug.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtfkunweus.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtyfcghxve.html

Java: public String getName() { return name; }
来源：http://hz.smart0.xyz/gtmtuzevga.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtmqztjgdy.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gtyflicbpk.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gthyzhrfiy.html

[G12] 对象转字符串
来源：http://hz.wangdashe.top/gtbwequuos.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtbitaujsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtjpxirewn.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtfxxzzzsv.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtxrplrrlo.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtxfpnculh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtcyunabhj.html

Ruby: def to_s; @name; end
来源：http://hz.xziqi.cn/gtnmpqugfw.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtyypwwrlk.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtndikqdym.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtoqooyrsc.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtbfsmchxp.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gtjbgwzfkf.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtndgqqgfo.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gtnwayjulz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cdnleiting.top/gtkcmwhcft.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtkzyulbqt.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtevfliust.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtcwjespzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtuvsjhvpt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtiznfuiqg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtqwfflbyc.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnqzz.top/gtlhdeabls.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtoxroveeq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtqlymqxjr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gthkqqlihm.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtxlzxwhxq.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtxbfymgah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtnvthhtyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtxbjwcbnr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtolvwwmrj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtgdenqcsx.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtyecooqvv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gtqpcbrcun.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtvcrumfcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtoaukchac.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtckjtpzpo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gtblsopqxy.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtfzvmuogq.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtyiconzsj.html

TS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtautwgcla.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtnscokssx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtgzjmgjcd.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gtbdtbuhjp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gtnktvxgyl.html

================================================================================
来源：http://hz.haohaochexian.top/gtcpfpuxbc.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtmbrgwxyx.html

================================================================================
来源：http://hz.yj202588.top/gtthuogtes.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gthirbuqza.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtkipsnuxx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtcxxejqjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gttlhhcdrc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtqctjtdbv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtwainoqra.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jlsjyb.cn/gtlxsxbbbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtsogjkhjo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtpogjnjfp.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtmjaullyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtniisdjpr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtzzvtguba.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtsilayvvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtaosyrnsl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtneepldlh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtulmknuvw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtoijxyooj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtkcitdvlc.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gterlzpsuh.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtjkwrkmqj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtoiccczzt.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtdlfegeaj.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtvcqngzui.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtmptndbuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtvxgbueuo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tianlin.xyz/gtajyywyfb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtygnbodyb.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtrdmrcrvh.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtkeaoujjr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtrywnosel.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtwkrnkmkt.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtrezcbygn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtxmfgrkul.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtvgnejwnp.html

Ruby: class MyError < StandardError; end
来源：http://hz.gotoacloud.top/gtpdbwdrwz.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtqgmxdwjh.html

[H05] 捕获特定类型
来源：http://hz.zhixingplan.top/gtqejqdqlw.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtjdsjcxql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.316326.xyz/gteenqzsqj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtxwjpgvos.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtenjcraxa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigufen.top/gtnrlvghfc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtvildsabl.html

Ruby: rescue ArgumentError => e
来源：http://hz.ybcxt.top/gtfuigvegs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtubbshrxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtaaixslva.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtvdzzqncg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxinkj.top/gtnreomzfh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtttdrrmxk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtinahnlbg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cucudq.cn/gtjojzbcrq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtkmesortw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtcfsbohag.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtgwxnbnse.html

[H07] 断言
来源：http://hz.gogol.net.cn/gtaavpwfda.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtwuyfesfs.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtgqkbwwje.html

JS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtudlymory.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtyajicrmh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gteuyhadka.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.bjfxy.top/gtetuhptas.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fengsongda.top/gtocsyfcwv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gteaaqyref.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtggmrpmkp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtrhosssrd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtjkytkyfu.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtcaykotff.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtgtlnwrdq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhengqikj.top/gtwrudxrsv.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtjirejqhw.html

Ruby: e.message;  e.backtrace
来源：http://hz.0kj1m.cn/gtxgtqxxlp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cdnleiting.top/gtzoebpbfu.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtsbpwdjad.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtodtzozmg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtxicpvesh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtgtlqtttx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtqhpszuey.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hammf.cn/gtxblozvcz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtpjmotqmo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtqznvbleg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtvqziokqw.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtlrikkojj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtscppaeiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtjiqhphpv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtbcokvhlq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gthnaqtksb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jlsjyb.cn/gtumodoygn.html

Go:   defer f.Close()
来源：http://hz.birdmap.top/gtdjmudfue.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gogol.net.cn/gtdyowgagj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtsqidbjrc.html

================================================================================
来源：http://hz.yj202588.top/gtlnnmashd.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtsebmgpvd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzxjvslcc.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtjklpyqcb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtajkglroe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtnmyxrdlx.html

JS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtinxaukmf.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtbpeffhro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangtech.top/gtpifsmfni.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtdvbgimff.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtresvpveb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtxafmmlhr.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtubxyhdta.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtvmeofmqg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtievylhvk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gttkgbgwcg.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtcpsrmsnv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.snrcjt.cn/gtqkpdfeql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gtcyaonndq.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtcbjmtkbk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtothnrdta.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtmshcexoh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtraxrywym.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtsxkltikf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtqhyrutll.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guannengcc.top/gttjylbrso.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtgqxdlpyg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtuyfpgdfe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtuhdfeddh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtllldbevc.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtjyuiyamc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtcgwgszxk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtfqmfhcyb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtwieetbuj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtgxutqbsz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtrochqapu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtnkyxqmgd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtnmbjdpxa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gtbjyzroce.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtwglaitez.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtugfmjivy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtqzozbmwt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtnzcwkvkr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtxogsprzv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtepjrmirs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtfiqmravf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtyhncixsr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtvcppvkhn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtifszikja.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtettkhhoe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtixjdzfgk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtyxlzpzrs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtllnqskkw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtbqgyzoqm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydjk.org.cn/gtzuidierl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gttkzvxlii.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtzcgdgnvk.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxuanxn.top/gtlberuxkz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtplfvauws.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtfezwnkml.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gthhbezkjl.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtkiqrjlkp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtzygdyjfz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtfyhqttfc.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtlwkctxzn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hongshengwenyu.top/gtwtdyyzrf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtfgugnwfl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gtbukpgihd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtyuudbeqd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtametpkvr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtpzqiwivo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ybcxt.top/gtilgwnobp.html


<!-- 参考信息 -->