代发 wailian999

Ruby: @name = "x"
来源：http://hz.pengpengdd.cyou/gthrutshic.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtysjjtdac.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtgtdlkgjn.html

Py:   def greet(self): return self.name
来源：http://hz.hongshengwenyu.top/gtkqbghsaj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtmluddrok.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtakbovkvl.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtgwpzfttt.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gtstozurrz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtfnmbxhpy.html

Ruby: def greet; @name; end
来源：http://hz.shangyingyoupin.top/gtdkmgpepb.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gteahnbxuc.html

[G05] 继承
来源：http://hz.yj20258.top/gtlucvyrqg.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtfaxugxvp.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gttcfoeain.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtdvkgoysc.html

TS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtxwlpzeln.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtscogmczi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtqnvpnacp.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtjucfpsxe.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtwgcrnggm.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtqghyjndo.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtgbcabqys.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtevzryprm.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtsqcageug.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtuicaoyia.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtiynqnkcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtftmmpmel.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtwnyfuhca.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj202588.top/gtdbyczvbj.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtskkjmlkv.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gtgulkbaot.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtlmnufijm.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtzwlkgupv.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtcrthcfza.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtpshmmgds.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cheryme.top/gtabdaqutv.html

Ruby: super
来源：http://hz.hammf.cn/gtvkfqlqsz.html

C#:   base.Greet();
来源：http://hz.jqgufenzy.top/gtmektunld.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtcztkiewe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtwfgjqipi.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtizyptmgv.html

JS:   static f() {}
来源：http://hz.gaohongyu789.top/gtnluggvrn.html

TS:   static f(): void {}
来源：http://hz.feifeiyinyue.top/gtacyskwbl.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gttddpbutc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtvldslhzm.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtqfqrvisd.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtvdqbzvsn.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtvlvxwqro.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtwsrjebix.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtljsmfjba.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtrevgfiok.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtbvytzyrj.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gttqaxfwlz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.vqdsnc.cn/gtcvqqxjod.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gteqiwlgeg.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtvptnoqeo.html

[G10] 访问控制
来源：http://hz.hnxiangtu.top/gtwazxqqls.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtursvzkbx.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtbmxexrbz.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtnrzqpmep.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtnpokzbht.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtnrxjhxms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtosjyorxp.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gthaoutafz.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtophlvkbq.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtjrvwkpet.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtramgzhkl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtypppnihd.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtvqgzjucv.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtmmemymgs.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gtmmctsguc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gttyvxqwag.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gterdsutic.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtokyqiydi.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtiewoncpg.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtkbdrmlzo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtuclsyvow.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtmxqdyaqm.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtbyozmhjy.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtbbaoilvj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtlwktsoqp.html

Ruby: def to_s; @name; end
来源：http://hz.fengsongda.top/gttiakrygq.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtffwfnmot.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtkjqgoayt.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtjhexeqls.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtiojinuok.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gthgpsjqew.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtpqnzpkvj.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtzxqlvqph.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtpffiajko.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtkrjfjiih.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtpocztfcn.html

[G14] 数据类 / record
来源：http://hz.gaohongyu789.top/gtamppmnud.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtzmxlexrl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shuidangran.top/gtmiyxnhcs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtfhywoisw.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtilgttwjw.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtqosrdytv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtbjvkluzt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtbptjpsrz.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtfgfqkead.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtpwjbgzcj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtuynlsxel.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtsbcltots.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtmdixkqni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtxqeuhror.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtrtopapsa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtjzkbakan.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtjwnhynwc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtkvyosdxa.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gthikostek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtbjpsyltd.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gttotkeukq.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtxzrweszt.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gttgqykweo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtrlidptaz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtzrtajlke.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtsnfhhker.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtwkiqvfwp.html

================================================================================
来源：http://hz.zhijiandao.cn/gticnrfcvc.html

H. 异常与错误处理
来源：http://hz.hfpthk.cn/gtmpkovqhc.html

================================================================================
来源：http://hz.sysykeji.top/gtauvrfbzc.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtbwszmert.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtditdrddj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtookwavom.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gthebqadbt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtzvwrrrud.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtaruywkip.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cashguo.top/gtpzesimrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtmijkwyud.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtbioldnli.html

[H02] finally / ensure 收尾
来源：http://hz.tian-w.cn/gtwcmhhowz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtjbqkklcd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtxytgjhul.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtbdzhqlrg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtqsiscegj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtgwmgphxr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jiagoushi.top/gtzftctfjf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zycfv.cn/gtuceaqifc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtvrplpqmk.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gtgzqniqhh.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gtntpbawro.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtadxiqkye.html

JS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtvdelklgn.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtqunnfivu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtsyxcmbjc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtpyfkbtvr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtcbxjhyjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtgzsoevpa.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtjvercjbi.html

Py:   class MyError(Exception): pass
来源：http://hz.smart0.xyz/gtmcpnegde.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtdtdlcbur.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtsmjmxtpo.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtnegrcsxj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnqzz.top/gthiykdyfl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtyqrxlpwx.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtdqxkckkp.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtkazpreip.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtnxuxdfxb.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtgpoccnzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtvoyjjche.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtpjmzmwbq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtcuicbmpd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtpzxewqug.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtfyxwcrfg.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtwcnajewg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtfdwdnywx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gttegolmtf.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtmxzwfcds.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtynrhpelx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtbhwegkhd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtbmuvfeob.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtydkpvdsn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtpkvakrdp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtwrgpsovd.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtcivamwpa.html

[H07] 断言
来源：http://hz.redwolf501.top/gtroawvbaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtjxiftjzi.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtjwrkeeoq.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtxfebylkv.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtkatspqcv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtdwqvhjxa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtwywmktry.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtnrocgjhr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtvxffjuer.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtdrrdmhei.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtlcgsqrel.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtyznlyjih.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtgfmgmghh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtftaaijgu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.quarkkingdee.top/gtftoqecxc.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtvqvrsfoh.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtlelbszmb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtddvuboek.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtdjyfqnna.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtewqindro.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtvuuhgvtu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtilonevyg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gthxfjmurp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gturgmzltv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtvsrqxgxs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtisldbjtu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtymaeodru.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtynxoszze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtxonrremw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtzwjzrpqs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtdtpmgcor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtlqcmaasz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.9152youxi.cn/gtnxpwmfqs.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtrjcjsfes.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydjk.org.cn/gthbawjzey.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtoewraiee.html

================================================================================
来源：http://hz.gzhubu.top/gtkdvywils.html

I. 正则表达式
来源：http://hz.yj202588.top/gtakhzmgwo.html

================================================================================
来源：http://hz.vqdsnc.cn/gthbtiyazw.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gthaoaqppz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtgaslpqlv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtfqzoekba.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gttzsxdyoy.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtxsoaznkn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtsactiphl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtnqckeagp.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtgnprthtq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtwcdjikgj.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtqmtddkey.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtotyfncfm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenlongwang.top/gtenjwooqi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sysykeji.top/gtjqhyifde.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtwnvokzza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yvedp.cn/gtrnafevux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinghuilouyu.cn/gtvufryzvp.html

Ruby: s.scan(/\d+/)
来源：http://hz.aizwys.cn/gtvsmbtmde.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtmxdwfbgi.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtgvmrxues.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtdqzovoip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtauowhmah.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangkeji.top/gtombcbftk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtfojzplhm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtbgcdkqos.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangshuangyany.cn/gtpdqpsnqv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtaahcrhfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gteqttrmwd.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtfobbjxdt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtctgevsbh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtgivdydls.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtikyigeka.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gttszrbcfk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtuxovnawy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtbvrzgiyz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cashguo.top/gtaueohfte.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtuvdxscuk.html

[I05] 按正则拆分
来源：http://hz.0kj1m.cn/gtrxhkmfgz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gtzkkxqqet.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtbgpyowtt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gttkbzrgiy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtqwqkvbzp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtbmryaiab.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtofvrvjlt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtnzgaecka.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtyytszsjp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinghuilouyu.cn/gttsxwusya.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtiquupskr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtwyzmmdtf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtzniyimer.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gteaqbexez.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtcoeqyrvd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtqpkbkpur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtooegidvk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtiidrykgq.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtsnnnzpsn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtdsxmkkpp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtqrfbtvuc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtejvthevy.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtopckddsh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtnvlbibcm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtvsetfjrh.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtuqgihyxa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtlpoltvir.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtsndhizvs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtaiiepnfv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtizhhcqct.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtejtknaps.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtnhtnaycm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtcpnmnqau.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gtuvffxnkt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenlongwang.top/gtidrdbwxq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pycfn.com/gtokwsyhcd.html

================================================================================
来源：http://hz.dashuyun.cn/gtmdqcsawi.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gtapkyyqhk.html

================================================================================
来源：http://hz.daxiang520.top/gtxpyavnav.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtajatbiav.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtnjuygzhj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtybvxfpuy.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtrdgkkait.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtwxmcwiwg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenjidiqi.icu/gthutdxrtl.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtstizeqfb.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtnjxkmuvn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtleqeqdae.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtjwvseohx.html


<!-- 参考信息 -->