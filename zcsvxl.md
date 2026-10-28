代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gtalucyncv.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtualltcbi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtysoylrah.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.andypj.xyz/gtuxtcijmr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtrfypicwn.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtfelhjwft.html

Py:   self.name = "x"
来源：http://hz.zhongyouzk.top/gtmudisnvu.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtlfjmfkvg.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtuzjhlebl.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtlrrtrcda.html

Java: private String name;
来源：http://hz.fzhhl.top/gtmwtbdzne.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtezixyrcl.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtwmnyzaln.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtlxcwrrkd.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtqjwruqym.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtduybkvbb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtgvvkkrgc.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtvlbhftmm.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtdyhqtwll.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtzuielsjk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtzniifebl.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtnzxjpotf.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtzlknenku.html

[G05] 继承
来源：http://hz.fzhhl.top/gttdehepyq.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtdwtvdfyv.html

PHP:  class Admin extends User {}
来源：http://hz.shzxlz.cn/gtbatyqqmy.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtatapjejy.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtpkyeeqla.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtavxqgnkv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gttlharsba.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtgnprxslc.html

C#:   class Admin : User {}
来源：http://hz.zhongyouzk.top/gtlhczozjs.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtohwsdvdx.html

Py:   def greet(self): return "admin"
来源：http://hz.pengpengdd.cyou/gtzhupgtwe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtnkgpdhiz.html

JS:   greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtzefiqbsu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtoompjgeh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtwlrcbnps.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtkktxzlli.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtxpxunmtc.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtbeglfzcq.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtkcttchvb.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtesexdccv.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtmucinlij.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gtpdpxsyws.html

TS:   super.greet();
来源：http://hz.tianlin.xyz/gtgjlcrwtn.html

Java: super.greet();
来源：http://hz.svipenyu.cn/gtrpuswkbm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtvvtbrxsl.html

Ruby: super
来源：http://hz.ppjwa.cn/gtfuzspdzr.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtdspnqjps.html

[G08] 静态方法与属性
来源：http://hz.yangfankeji.com/gthlfnmzbc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gttqspnhfb.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtpptfrnyx.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtsfihmrqu.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtrtgqzics.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtmemelakt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtyreeavnf.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gttwsqoqjd.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtvvuydzby.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtdfyyxtco.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gtzcfmacvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtyrmhafhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sysykeji.top/gtqfbwfnjn.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gthjpsywbz.html

Java: interface Shape { double area(); }
来源：http://hz.andypj.xyz/gtqnyvxmpt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtqanmjqfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtnuhvnuxz.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtnmajbwde.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtiivjqhgs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtdfggxhxx.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtnprykiny.html

JS:   #private 字段；其余公开
来源：http://hz.yueranfly.top/gtpluimczw.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtmtsplhqq.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtwwppajdj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtcxtvitas.html

Ruby: public / protected / private
来源：http://hz.vqdsnc.cn/gtmjhogwef.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtbdpjpzcn.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtrtxqfqzd.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtlaoymypw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtwtioluji.html

JS:   get name() { return this._name; }
来源：http://hz.jiagoushi.top/gtfljtckbf.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtqzccaxxs.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtcyhmfvrn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuanzx.com/gtqncjnwfk.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtoesfebye.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gtmbraeyop.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtqxdjlsdq.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtgkmshjiq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gteqhelwjm.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtxdyghdqq.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtogggztyy.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtgobnsjhj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtvfbspgkh.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtbqputwhg.html

C#:   public override string ToString() => Name;
来源：http://hz.yvedp.cn/gtfbmkbpml.html

[G13] 判断对象类型
来源：http://hz.quarkkingdee.top/gtureazbay.html

Py:   isinstance(u, User)
来源：http://hz.yanxiufei.cn/gtogeuttju.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gthujxolxh.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtpmfeocnn.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtwnbomepu.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtqbygvwvc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtheldexah.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtprwbejvc.html

C#:   u is User
来源：http://hz.cashguo.top/gttimkbhga.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtcexgpskk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtgfqguqtp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtfouzhcii.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gtwynkjtmk.html

TS:   type User = { name: string; age: number };
来源：http://hz.gzhubu.top/gtebtrwwie.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtjxnipfxl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtvanklwej.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.vqdsnc.cn/gtuknuapao.html

C#:   record User(string Name, int Age);
来源：http://hz.haohaochexian.top/gtilkzuuly.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtsvbjffox.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtgljlqkyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtbhtajkvm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtlrugmefy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtmusayeut.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtmrfkxqub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.meibo888.top/gtwlepopno.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtitcqrgts.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtiuznqoyd.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtzcdkxnnj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtyrcipsju.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtswxmjefg.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gthtqqgumz.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtozhvkqzi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtyzrzscdx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtkhbbkosl.html

Ruby: obj.instance_variables
来源：http://hz.wangdashe.top/gtpractrxi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtwhjqqdjm.html

================================================================================
来源：http://hz.zycfv.cn/gtwptdwjwv.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtyhqcqjau.html

================================================================================
来源：http://hz.chenlongwang.top/gtfcseclii.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtxttcpkyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtymdwdzqt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gthchlnopk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtxkxbfvbh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gthwblpcgm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtzygjyzrq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtevcvczdq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gzhubu.top/gtiewbbwgv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtpifvuink.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtsjnlaztf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhengqikj.top/gtdfieljfk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtlmzmpvik.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtpznynfim.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtwetbeicw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtpsoobvnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yueranfly.top/gtoykcourb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtxukmyjpi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtertylrtu.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtxmonkwjk.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangkeji.top/gtsfnskqka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.havefunace.top/gtctwtpkok.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtxrlxnkzs.html

TS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gttpukmkru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtruglgewz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtbgkwwmxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtdlcwhcli.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtkfhtfays.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtumnckwkf.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtbbkjtamc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtbokteidb.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtjgeqwjtu.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtrqvfhkug.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtnuzbjgiy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtjltrhhld.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj20258888.top/gtzcgxextd.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtoydkfcbh.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gthgwgehyh.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtvgcathch.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtbqbmvqyx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtfvlyksym.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtejgkcrvx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenlongwang.top/gtfkrexzyy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtxogozpce.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtydbmltyv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gtaminvdfv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydzc1.top/gtzcbihhim.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gtkqfhwjfb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtpemyzkxr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtxyoxwtfb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gttbzhrbhu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gttbcdjrsk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gtivzfdsja.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dianchejie.cn/gtxgksveym.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuanzhike.top/gtxtpmwdla.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtjoyvfkeu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydzc1.top/gtsizejtjc.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtufxoedgv.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtkuamjqlq.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtdriqpaam.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gtytdwoghw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhixingplan.top/gthptzceqf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtyeefqwvq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jyoumei.cn/gtbhmicpgs.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gtwugxloxo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gtrfnljllz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtvbnwwwam.html

JS:   e.message;  e.stack
来源：http://hz.ywan-chungtsiang.top/gtfhyyfbtm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtiifbqojz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258888.top/gtudzirqur.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtslxzgqhu.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtfmaylwjx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gtmsrahqqg.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtjvymumbn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtfvkaxfeo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangtech.top/gtkesquqtn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtdcjtpnvy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtzaofpwvz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gttfghicgv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtwutdoont.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtoxpgdnom.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.svipenyu.cn/gtfsgdcqba.html

[H10] 资源自动释放
来源：http://hz.jiagoushi.top/gtlhsoflmx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtnocxhzpf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtfktwugxr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtwahfnqzk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtoscliihs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtdicznfpa.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtznorowvi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtjadljuuv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cashguo.top/gtvvraigjh.html

================================================================================
来源：http://hz.cucudq.cn/gtedjielzj.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtecsuqqlx.html

================================================================================
来源：http://hz.jiagoushi.top/gtipaynmcy.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtkicwcnku.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtpqkoltqd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtinyctnax.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtiyaiwwad.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtidwvpzns.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtplavnmsz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtcxgwiwwu.html

Ruby: s.match?(/\d+/)
来源：http://hz.cucudq.cn/gtnehmrdxs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenlongwang.top/gtjjrpvokd.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtunbfrrwp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtfelotwss.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtyrwnihlp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gthofcqese.html

TS:   s.match(/\d+/g)
来源：http://hz.nwbrower.top/gttjdgpxfs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hammf.cn/gtejicdfry.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtoruvffin.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtazvmhubw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtcdmnabgg.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtrprznkoa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gthruygeup.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtobttcuqj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtfomhcofc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gttakeyudv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtjjhuxoao.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtguqebqqr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cucudq.cn/gtzxzaegsq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtjhbklvqs.html

[I04] 正则替换
来源：http://hz.jqgfzy.top/gtvwbvwmwl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtzgmfhduy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtibeqytgy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtlhhuugas.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtacfrdsml.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gthguuzvhq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtjebvrcmr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gthcyugaqm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gthqhnnsnp.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtpyhndzgw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigufen.top/gtesazcpph.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtnfgmcjnv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtppybeihd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtzwaffkri.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gtfoevnncl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtqldmdydl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtqadbcrks.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gthaquhuun.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtqlwbdfmf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtzdfpwqor.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gttwkkoxfp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtuamrbcfk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtycixnlin.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yvedp.cn/gttuqrfquc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtiltnbhxk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shangyingyoupin.top/gtkwukzbqn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtjetqonzh.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydjk.org.cn/gttovdzlss.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jiagoushi.top/gtvqvtzlpr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gthdxvxwwb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gthesjjcfc.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtxzsgypuw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtkztkjwxv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtdssitcva.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtkxcgpcee.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtkwxswoen.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtlaxmyeue.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gttemgarzf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtwnqxgzgo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtlychxpvn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtqowttnto.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtujqzvmsx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pengpengdd.cyou/gtbwusdqnw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtjwlfadxt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtizpyyewb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbwetiwjn.html


<!-- 参考信息 -->