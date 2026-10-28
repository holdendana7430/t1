代发 wailian999

Java: class User {}
来源：http://hz.xziqi.cn/gtlucgksqj.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gthldfezar.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtjlqvzghv.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtrlfcfezw.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtgkmiwgnb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtlofjxgzs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtbdceylqs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtsyxswpqh.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtwcfmraaz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtevwbkvhx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.snrcjt.cn/gtaiabesog.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtfjjapzps.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gteuyzwvkv.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtvalycshd.html

Py:   self.name = "x"
来源：http://hz.nwbrower.top/gttnawubym.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtxrhrrkjk.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gtkkdmcgzm.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtlncqtkjc.html

Java: private String name;
来源：http://hz.sxryk.cn/gtxizhuxja.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtbidsdeuy.html

Ruby: @name = "x"
来源：http://hz.smart0.xyz/gtncamotxp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtbxrwqryx.html

[G04] 定义方法
来源：http://hz.xuanzx.com/gtwrrdlbfr.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtovrcsvub.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtgvyadfbu.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtwtxvvaah.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtcvircayk.html

Java: String greet() { return name; }
来源：http://hz.smart0.xyz/gtxizllocr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtgzitxmxg.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtrvwqvytk.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtsobtxfzh.html

[G05] 继承
来源：http://hz.yj20258888.top/gtufjzzpco.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtiapduofu.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtxeghoyil.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtpkqxjccy.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtogrgzbjv.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtjzthzjqb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gtmvzolhtw.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtmuqfqcle.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtdzrqguda.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtmmavtyfo.html

Py:   def greet(self): return "admin"
来源：http://hz.ppjwa.cn/gtcnybnbxn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtpowcvioq.html

JS:   greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtpopsqzjh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtyuqexrjs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtwyahwtpo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtxahtnssj.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtypjpuvou.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtyzuzatsj.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtwexxkobw.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtkgnmcynq.html

PHP:  parent::greet();
来源：http://hz.jqgfzy.top/gtzfxdupzl.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtmfloifjl.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtbvamptjz.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtruqlrovh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtekzptaln.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtcpntvmip.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtbrpkxynu.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtgdcihkky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtbzaowgxf.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtymqqzvqh.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtltbhygow.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtozhgrpxk.html

Java: static void f() {}
来源：http://hz.cashguo.top/gtvxirajxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hongshengwenyu.top/gtsxvdtuvb.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gttdemjtxp.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtjibhkddn.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtnacyvrlg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhongyouzk.top/gtkpyvhrqr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtwejzkiur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yanxiufei.cn/gtkciokpce.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtdxwasuzx.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gtlwitwvyn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtvktoszcx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtshldgvzu.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtmxvcdtrz.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtifikdweg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtqaaurykz.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtlfxhkppx.html

JS:   #private 字段；其余公开
来源：http://hz.yueranfly.top/gtxuaclhng.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtufwndvih.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtbgbgkufw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj202588.top/gtdwigzbiz.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtxdsqgyui.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtnufnwrho.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtaqknnjul.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtowswqwkt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtehxxyqha.html

JS:   get name() { return this._name; }
来源：http://hz.xziqi.cn/gteokvhhra.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtyqjzyngf.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtmqdzegho.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gttqcgsdok.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtdajndoir.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtkuzxepjb.html

[G12] 对象转字符串
来源：http://hz.ydzc1.top/gtjzrthjnn.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gteppepubx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtzmxxcvkv.html

JS:   toString() { return this.name; }
来源：http://hz.ybcxt.top/gtwvuihdqi.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtvfxjsiqy.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtevvpvxqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtxmxjeybx.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtthlldgqf.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtnwmprxrc.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtcreqvurg.html

Py:   isinstance(u, User)
来源：http://hz.daria6918.cn/gtzvplragj.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtoeldwang.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtrzpfdyux.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtpeuxcnit.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtxriucrpp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sufxvd.cn/gtxvgaeybf.html

Ruby: u.is_a?(User)
来源：http://hz.sufxvd.cn/gtmzixlglp.html

C#:   u is User
来源：http://hz.iojbl.cn/gtuinsgjgb.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gteewtcgke.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtzecvenwx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtfkftwlfk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtvcuarvwv.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtgxusjsdr.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtuqtipacy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtkkhbxxhd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtbrxfwtel.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtbmvnrzah.html

[G15] 枚举
来源：http://hz.guannengcc.top/gthhgbkssw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgfzy.top/gtyknulkjh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtsswkeqsb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gtcicuyjup.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gttuohcqiv.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtqifpuipr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtufibcujv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtofgbbppz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtqsuixbfd.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtsyeygcdl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtuyklswxc.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtxgewaetp.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtrxxypmng.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtwagcsmns.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtvskdlefh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtatodpfuc.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtsbhdnagx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gogol.net.cn/gtqdncfmta.html

================================================================================
来源：http://hz.yongpay.top/gtcxancyth.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gtugpitmyh.html

================================================================================
来源：http://hz.jqgfzy.top/gttbcvdjvj.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtjmharnyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtecesoorw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fengsongda.top/gtjrnfajav.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtanhbsvbs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtjrmhjjiy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gtxwufawof.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.mhx1999.top/gthvdrckyj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtwjycxyca.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtrwiduqhf.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtjtqbamxz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtlgopaczy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gteefktjix.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtjphbumsw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtlmwcnsel.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtxquqtmfd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtdjkfkxmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtjqgpxgkq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gogol.net.cn/gtebhcmsee.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtvwlukzwc.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtxonxgfck.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtegpteowo.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtpdxkoyuk.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtqhxjoajg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtazfdnath.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtnfxcvrlg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtgcoycpht.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtvvdkugoc.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gthqckjkjz.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtotnurnyo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtgldnanvm.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtjlkronya.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtwycundsv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtgrjxbrqv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtvassoskp.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gttpszfcxg.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtdiwmvkee.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtspdpdsww.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtqdtknfsv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtlczkyciq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtqgwbhdjt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtdjnitjrf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtirrkxeez.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtonthmkpb.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gtnvkaoblq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xziqi.cn/gtghaeboaz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gteslnowhb.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtaqglphwn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gthbsesgex.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtlavrccua.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtcovifvuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtertbhdvs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtwvdlizyh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gttvhlnxqx.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtmsmmprir.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtrtxfgpxk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtcderiraa.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtdcvposwe.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtlonbwcjy.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtbmnxpnrk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtlirnhpyn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtpfywbtyx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtebhocejt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gthmaoslhw.html

[H08] 获取错误信息与堆栈
来源：http://hz.kuanghao11.cn/gtkkbxaagq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtwpkfyavh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtfdzsixpl.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gtnevxzfan.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtwqomzhli.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtwkmnuspe.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtvewcrmlh.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtcvddyfqi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtxcqcfbef.html

[H09] 带错误码的异常
来源：http://hz.yueranfly.top/gtjfagkxbn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtjxrovycw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtalroebwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jlsjyb.cn/gtlayakhxt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtzzghncks.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtsbgdfvjy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtbqutzaye.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtivpbfknt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtvbobfjyo.html

[H10] 资源自动释放
来源：http://hz.kuanghao11.cn/gtzwuipwsh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gaohongyu789.top/gthsrdyufc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtakakcbrg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtmofeojvt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtiukrzzkl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtktefcfwo.html

Go:   defer f.Close()
来源：http://hz.xylfe.cn/gtnrcndunm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtsqevfxcg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtagedyhvc.html

================================================================================
来源：http://hz.daxiang520.top/gtzagzdwat.html

I. 正则表达式
来源：http://hz.svipenyu.cn/gtwejopkrv.html

================================================================================
来源：http://hz.haohaochexian.top/gtavgnydze.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtuwhuemjn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtahyavkxv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtkzsqaagf.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtzyriaowt.html

TS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtsexlsdhp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtngcmqcbo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtljtvdgyk.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtvysajvgt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gttujbyvaa.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtsrubqvrz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtasyghhyl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtmacsnsaf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtahzrttme.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtsdonzpmo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtvleryydo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daria6918.cn/gtphieddjy.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gtolgzbrnp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtsaipcpwt.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtaoioeewe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtgryesbre.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtijxdazdh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtqgigreec.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtzazmigau.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtribtxknd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtqoiuirbe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.haohaochexian.top/gtcxbnbdpq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aibaodan.cn/gtrjcevhrc.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gttxbwvqjm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gtdofyrrkg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtiaznveue.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtvbbgwrch.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtoqpoutfi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhiwuduotai.top/gtnyxormcd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtlhfzyopg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtbgsmjnsx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gthrewyvso.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtjgnfojmn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtvfbnhcly.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gttuudoroj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gthfpluvhu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtsxqoftyw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtegdmitin.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtquqjbwco.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtssolwggh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtwvrbtjfu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtespwguqa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtkglubzas.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtfxnjbgmw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtanhhqwrw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtgfovhzdn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtybrbmtxr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtunwefmzo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yvedp.cn/gtzplmfyxj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtuamxpnar.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtcuzldtby.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtwmlhates.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtdthasqft.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtfefmwrog.html

TS:   /error/gim
来源：http://hz.aibaodan.cn/gtcjdlfzdu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtvqkprjlu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gttflqjzge.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtvrhaezqf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtlnjxfwwn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtqqyqtivg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhiwuduotai.top/gtzmyltyzd.html


<!-- 参考信息 -->