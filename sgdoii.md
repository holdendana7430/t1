代发 wailian999

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtxcvtjnnv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtfuinrxio.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtnyghzgsx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pycfn.com/gttdzxycnn.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gttkunkswq.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtgenlsxjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtdlxlqmze.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtswdfiwbc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gthzfcbsex.html

[G03] 实例属性
来源：http://hz.smart0.xyz/gtmitlmkkc.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtmkevxzuj.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtdxlrrnww.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtimblvnsm.html

TS:   name: string = "x";
来源：http://hz.yvedp.cn/gtdonqmjla.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtswrzmjte.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtudmpcenm.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtiompqbyr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gttikpdllh.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtawtpavar.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtxappkxws.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtjbjresum.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtkwheakhp.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtwzgglrtt.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtoxtvgmwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtbdkxoybv.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtugxxoond.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gtppaeljzx.html

[G05] 继承
来源：http://hz.cdnleiting.top/gtbkzqvnrs.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtllnhiktl.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigufen.top/gtzfhegrfu.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtogzyereq.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtbesqkhcz.html

Java: class Admin extends User {}
来源：http://hz.iojbl.cn/gttxjnkmso.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtweghepiq.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtixrnevon.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangkeji.top/gtvhxidicj.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtjhkbrdxo.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtborowylc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtyxwbxpbq.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtlrcpipra.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtyfwdpjdn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtjmyoywsg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtqxugcmjo.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtnbjrhvez.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtjjmgmxqt.html

[G07] 调用父类方法
来源：http://hz.zhongyouzk.top/gtxmdclnjj.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtwpvrlqlg.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gtperwjtzt.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtkqirbtdj.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtgmvnhxem.html

Java: super.greet();
来源：http://hz.daria6918.cn/gtanqbwipp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ivvv.top/gtcjnjbddd.html

Ruby: super
来源：http://hz.aibaodan.cn/gtoliwxwis.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtlouiufqn.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtapsbxdya.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtncgznhrq.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gtbyqsddhc.html

JS:   static f() {}
来源：http://hz.52xcode.cn/gtkrxmyxng.html

TS:   static f(): void {}
来源：http://hz.fzhhl.top/gtrnycixuh.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtumclcisa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtjiiwvpzl.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtgonfdhad.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtdczenisd.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtbawuiehe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtshaqgbmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtxdztezdk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtecizaiav.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtvbenxpsp.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gttavanbad.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhijiandao.cn/gtmkscyvpl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aibaodan.cn/gtkaphymsw.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhijiandao.cn/gtmokmwdqd.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtdzmwxdwg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtufrpwbjg.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtfqrxecru.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtomtchkfo.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtlzvjfxcp.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gthcfdpqvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtsoagndkh.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtdnmjjrgh.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gteqthhxwr.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtxwlafkdh.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtlojsxlfg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtwzaomirn.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtcuzjvokc.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtxevuuvqw.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gtmjzzfvzh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtaxxutkqv.html

Ruby: attr_accessor :name
来源：http://hz.daxiang520.top/gtrssskuin.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtjsonpzgo.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtedabfzbs.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtojeyyuig.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtumnczqiz.html

JS:   toString() { return this.name; }
来源：http://hz.c1oappe.top/gtpjczoxnu.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gttlbxmogh.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtkiupzfrq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tian-w.cn/gtzlfmstnl.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtbgbpcige.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gttursjgas.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtymdrugev.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gttmunyvej.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gttxyhtnxi.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtbyuiujxh.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gterggdker.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gtnbafyvfd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuanzhike.top/gtrdkajkqj.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtzkeqhksc.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtidkrlocx.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtnejmhbaa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtwjiqzlrk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtnezzyjfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pycfn.com/gtnvtxgmwr.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtvnsnfqcm.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtnjkmvczo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtdughdbjd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtcqotkrwp.html

C#:   record User(string Name, int Age);
来源：http://hz.xinyue.icu/gtwdrqryqy.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtsszfkzjj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtdexyemci.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtedohechy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gtapeluikp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtlycbtcsw.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtrzcqcmof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtallzhskj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zdqjudy.top/gtdwwipazr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtjenmpsoq.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtoniqjkpw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtmqozowks.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtwngfqggd.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtownlntko.html

TS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtybravpzy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gtuvxfposd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gtymrsusfa.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtofavbjix.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gthqdlpaqq.html

================================================================================
来源：http://hz.316326.xyz/gtipllwyub.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gtxmqdefri.html

================================================================================
来源：http://hz.gotoacloud.top/gtgyctmzgv.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtdvuzhxgx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtsxhsnlzv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtimkdqpry.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtveyoaukc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtrmizkodc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gtwksthwhg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtgbezhljw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtrpbbxvdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtaqxqbyde.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtlhatihch.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtiblqdrob.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtfedgrqsf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtgdivngho.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtmbqutfts.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtbsfzlkeq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtdvivicef.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtruymthxw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtieswnkct.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtkznmbdcy.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtmbvkauuw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtqtopyhdq.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtgculalym.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtbjtpefwc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gthuusmaxl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ehwqpu.com/gtojihclit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtjuloucoq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtsxlxnqep.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtihewpmdw.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtmrkqumbu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gttwishdst.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtejxzpuea.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtsddyvcux.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gtflolceyt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtfkdypbgc.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gteeqobxng.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtbepkaqup.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gttihyuqpi.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtxthgexbb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtcybntkln.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtoaznlpqg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtlphrfqos.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtdpuhfdzl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtszsvtdug.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtdorrstba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtwiekedcj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtrmeycdyp.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtkwmqhhrx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxinkj.top/gtcpizfnas.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtguwqngca.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtrqrbyefv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.mhx1999.top/gtzticddfw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtcbkzdrlw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtdwnbcjcg.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtzvfnuxta.html

[H07] 断言
来源：http://hz.bjfxy.top/gtdwzwakpx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtxsaskzaf.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtrclauupe.html

JS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtymnhfqgd.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtcpwtrskb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtepoksaep.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cashguo.top/gtmjaizmyc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtnbgkemek.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtvzjxgktn.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtdtkmjsav.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gthwsfwjng.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yanxiufei.cn/gtgiymjaur.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtbbzylitl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ppjwa.cn/gtklgwwdwy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gtuxeuewwj.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtiradldkj.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtqdrgqnvu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtpyfrbaiv.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtgxqntnzj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtdnmojdly.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtgkoetsql.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gteuakunwp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtfsywtaer.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gttyiuzugj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtksnrcllh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtpqjvvmzg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.svipenyu.cn/gtezsfnayr.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gtpddjpuxh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj202588.top/gtbyboizon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtikcdjakn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtjdhefftd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtzdramion.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gthgdiijmg.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gtodlnbrvq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtgdsxxzjj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtsdnbqpds.html

================================================================================
来源：http://hz.zdqjudy.top/gthwzvgtez.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtqnbsqaub.html

================================================================================
来源：http://hz.ybcxt.top/gtcqytxmxn.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtchgaeuyt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtnvwdmobv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtiyzcvknq.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtwxugzeyd.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtwoaphwev.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangtech.top/gtrjdjnndy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtxquhoisk.html

Ruby: s.match?(/\d+/)
来源：http://hz.cucudq.cn/gtoeexfldj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtcopfeuqw.html

[I02] 提取所有匹配
来源：http://hz.gzhubu.top/gtennizqrc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtdrkazhhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtqotaljec.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtbkaxqahw.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtzmtphewv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gthgynfwuv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtcijporul.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtiwxauabo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtnigecnfz.html

[I03] 提取捕获分组
来源：http://hz.jqgufenzy.top/gtwyiotvrn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtckfrtukz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtpuptokhs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtaakzruke.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtlvuaputx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtsegpsihm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtefancwdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gthairgerg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtwaaszmht.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtdvekyjzj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtonwcotbw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtssrrmyqr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtnpxkzxry.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtdcvnjbiw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sysykeji.top/gtqeohubhf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pycfn.com/gtxxopjulk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtvilqwrui.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtapijxcto.html

[I05] 按正则拆分
来源：http://hz.wangshuangyany.cn/gtrfvmzzut.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtixkvpaip.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtbuldxidt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtimhcmpkr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtmzpwqqyh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gthrdeurzc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258888.top/gtnemmiywl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtmeyubgyk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.haohaochexian.top/gtewzameqx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtrumrbghx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtrlhzanvn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtnrcfvzeb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtejxwgusv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtcxdqqiiy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtzujegzql.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gteyugprce.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtkfzadflq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtezswbzjs.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtazpxkkfn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gteyjouxvf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fengsongda.top/gtxvdrajkm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtaentrogh.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtwoekmdun.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtqbvraocb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtkeihbdtc.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gtwomhasdf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gttseiyfub.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtjyjiagkh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtqtrtjchi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtlugaheaz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtmtzmvuyo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtklsoyret.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtyjkfosxk.html


<!-- 参考信息 -->