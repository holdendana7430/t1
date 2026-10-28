代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtfvbyfyaa.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtdutmpmoi.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtfdasaqck.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtxedpzdqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtoddoxxvb.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtwknhsxey.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtmmqvrndo.html

[G05] 继承
来源：http://hz.xinyue.icu/gtwfomjaar.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtninueodt.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtbmqydssn.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtjedzhodw.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtjvjtrach.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtbtzqhbdv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtgwjdxsay.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtkemepjhw.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtcfbuwnbm.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtttwmqarw.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtcirbflom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gttksrzspa.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtrjmrtada.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtxvnwvmxa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtseqdhcsq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtxeknxwnp.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtecdqhxkc.html

C#:   public override string Greet() => "admin";
来源：http://hz.daria6918.cn/gttikfuxcw.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtnmniwxtb.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gttksmxzsq.html

PHP:  parent::greet();
来源：http://hz.sweek.top/gtcsxxpueg.html

JS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtbkyrkdog.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtglbofacj.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtviphtptv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtkjniwjwg.html

Ruby: super
来源：http://hz.sweek.top/gtkrowwddq.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtmrplcoxi.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtfoibtkpc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtpxylzpsv.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtkbjssjal.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtxmqpkvht.html

TS:   static f(): void {}
来源：http://hz.redwolf501.top/gtfazhvbor.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtcuxkzzax.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtapckrrwd.html

Ruby: def self.f; end
来源：http://hz.jqgufenzy.top/gtugwkycge.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtikikchif.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtryipebyc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtjevocnjq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cashguo.top/gtbqfidvsf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtvpbhzwpe.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtwvmcxkjx.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtijphmvtr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gteuyohjcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtpgqaomez.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtfoqrgksx.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gthitonqbh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xingfuxueyuan.xyz/gtwwbbxwfi.html

PHP:  public / protected / private
来源：http://hz.shangyingyoupin.top/gtwxwzlach.html

JS:   #private 字段；其余公开
来源：http://hz.mhx1999.top/gtcbdcnlpr.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtgbbqosqd.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtuhsiwiie.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hongshengwenyu.top/gtevyaslww.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtpbkmwukn.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtsnmsnfml.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtpltodnfj.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtphoroqtv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtjuwewuan.html

JS:   get name() { return this._name; }
来源：http://hz.yuanzhike.top/gtddacyjdk.html

TS:   get name(): string { return this._name; }
来源：http://hz.shangyingyoupin.top/gtpaggfpmr.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtrazdtibo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gttnpcztdh.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtjhzvurvp.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtmbfgwpod.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtbghxshgk.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtkbacluzc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gteiaocbgf.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtgdxspygr.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtqkiyzxsv.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtnjrgiscg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtpoptkqpe.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtygbgjdzh.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtgobfiffc.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtkdaksmfu.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtqoreyufv.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtipllniqm.html

JS:   u instanceof User
来源：http://hz.xylfe.cn/gticcvqeke.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtaxrxakwr.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtkflhgusu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gtzgyxlued.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtqglspbjj.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtcyqfyfpm.html

[G14] 数据类 / record
来源：http://hz.zhoulong.xyz/gtjvbqdrhn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gthsxrhlxh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtzpwbmppv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtybhdifnx.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gtpirqrzkx.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtbqrzrerc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtytyecnkf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtbrmmvvjt.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gthkludxdm.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtuqoystxw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.vqdsnc.cn/gtxtvdnfpo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gttqbghyyg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtblsywway.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtemmfgwbo.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtojnrtsqs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jlsjyb.cn/gtjnrpwnyp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtavyajhar.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtnobubypw.html

[G16] 对象转数组 / 字典
来源：http://hz.yueranfly.top/gtgtcupzfo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.haohaochexian.top/gtstldbysb.html

PHP:  get_object_vars($obj);
来源：http://hz.meibo888.top/gtuvxbifmv.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtoqasacod.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtcsyeduaf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtgsawpxri.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gogol.net.cn/gtjgtznfqx.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtmukdkwlh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtgasuaauf.html

================================================================================
来源：http://hz.yuanzhike.top/gtngzaiqin.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtkneqnzju.html

================================================================================
来源：http://hz.jyoumei.cn/gtezwqteep.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtlmxnvofl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtvdejeicv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtajlmsthm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtlpvmubmx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtjnxltzth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtiaxdewmb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtmjewewsd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xziqi.cn/gtgenaiqcr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aibaodan.cn/gtsvdpeoqv.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtehchljgt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtnlsjupws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtnsiffnyz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtxyjevrow.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtvrlrxysa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtawatuvlm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtoisullbu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtrdtpwjof.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gthbvajoox.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtisciluhj.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtwytboedc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gttyrbgdlb.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtzoyzxlck.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtkownuwek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtenwlyewk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtfljnywrm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtsnbaahid.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtzwochohc.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtfkvrnfvu.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtgcgadtsa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gtkefkfqpe.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtrautbzhw.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtnfphwdfz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtkyxozunu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtgzbuyftv.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gtjbjojqgh.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtjudosjel.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtthxnicin.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtbslpyjeq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtthgmlxtw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtcgclhhae.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtudauthiq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shangyingyoupin.top/gtkqhymfkw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cashguo.top/gtshnxeikm.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtwuqcelbt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sweek.top/gtqdctahmt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jlsjyb.cn/gtcmnxmifx.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtszltudwa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sweek.top/gtosqyjbyo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtiooqjwzm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtjhwmghme.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtmxfhlqyo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtowfezdfx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gthcyuzisr.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtagmmozmf.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtdmuzevcm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtfjanmlmv.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtwhydhdlv.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtdlmlikta.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtihxwfatd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gtckmnsxxv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtpxnapbso.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gtpotlhnka.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtldwxacvv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtqnjmpzrl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gthpvjefpa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtaeetrovc.html

JS:   e.message;  e.stack
来源：http://hz.zdqjudy.top/gtkpbmbjva.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydjk.org.cn/gtusykkjgz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtxgbljouu.html

Go:   err.Error()
来源：http://hz.snrcjt.cn/gtbjrliadn.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtnugirjay.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtrvecfich.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtofbdetyo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtczhwukil.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtcxstvsos.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gthqfhmtpz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtfkzjljyr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtvnllzhky.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtnwhuwknt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtxdsulkoz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tianlin.xyz/gtpsqyelhn.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtnpxmpxkl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hysaishi.cn/gtzuxlmqqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtrccnebrq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtbxsjjmij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtlbonudvv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.c1oappe.top/gtspqljwgn.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gteyecrtkm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtjllajjxz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtuckmwmls.html

================================================================================
来源：http://hz.yongpay.top/gtvgwhodkj.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtqyjnghbf.html

================================================================================
来源：http://hz.gogol.net.cn/gtmohcgnyq.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtsxolfhpw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtysgghkyd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gtjzuonwaz.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtbajjukvj.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtthmyopzp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtnaqxbgqd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtyrstccqq.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtydxfpcax.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtezikabdq.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtwejhxlbo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtdscdltub.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtwwuudsod.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtkbyindln.html

TS:   s.match(/\d+/g)
来源：http://hz.c1oappe.top/gtrnzqhizp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtccpbereu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtlxiyigdx.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtnnpupyke.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gzhubu.top/gtdplwlwca.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtkutmkyqx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gtvjayzjwv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtchqnxeog.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtvavttauz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sweek.top/gtgbqrqweo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xylfe.cn/gtfkuclplk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtgqpuabjq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtjfofsxza.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtrlisfgqk.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtdpqrcnod.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtiphsxrqh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtcqytvhyd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtaoduwwqv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtptfqntkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtznshpces.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtsqhizylm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtoomgkdxo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gttttzlmrt.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gtzbfdfgwf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtfkswdzyx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtjhnbnohk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtkpksmbzr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtrczwsmaf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtrbhshsjc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtuczpshba.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtdgvkqury.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtlbccated.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtksvhdopb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtnykuepwq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtkftxywha.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtialruiic.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gthxideunp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtwxzrrwee.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtvfzjuxap.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtyzwurava.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtsiljroxo.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtsvnfatiw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtbvjaqvao.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtcahnkxtk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtoppusrxt.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtbzlytaoq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtcyowdkxr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtrsfrfqav.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtmtabmoki.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtxdounwwn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xinyue.icu/gtqyujsrap.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtxccbeygz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtiemouuua.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtrpzvqbuk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtnpdghpir.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtlbfedsbu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shzxlz.cn/gtevtnlllk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuanzx.com/gtlfrwoomk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtcemsdcin.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrgdiuabo.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtcrbotbvp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmapbzymn.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gthgtfimqd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtjsoajlil.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtafixcsuj.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gthnwcqdzf.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtusshfelh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtvubswnye.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gthjvbrozw.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtmhkjzcvx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gtrahmcruh.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gthsfdhtjl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gthespuzwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtnzkukczu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.quarkkingdee.top/gtaozljdmd.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtswmmwcfa.html


<!-- 参考信息 -->