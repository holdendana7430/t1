代发 wailian999

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtwvzynkgr.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtdtywioyw.html

Java: private String name;
来源：http://hz.cashguo.top/gtkyacwjwn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtmbovevtl.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtxpxebwio.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtrlaoysrb.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtmpfafwir.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtyeaqqhax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtxaldsanv.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gttyuynajm.html

TS:   greet(): string { return this.name; }
来源：http://hz.sweek.top/gtrtzorcni.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gtzmiazocg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtxujufxuf.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtxsugzxos.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtdsiapdqq.html

[G05] 继承
来源：http://hz.daria6918.cn/gttyplmsrl.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtnxmvznyh.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtxwxkkdoc.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtbquczcji.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gttuchuysg.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtnngypsyy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtjvmtkuet.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gtnbehvxhf.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtuzoiafjs.html

[G06] 重写方法
来源：http://hz.yonumen.top/gtedmsdzld.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gtehbejnll.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtxedscywt.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtgscoverf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtmkwuusry.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtijptgflk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.birdmap.top/gtuipzfzxe.html

Ruby: def greet; "admin"; end
来源：http://hz.havefunace.top/gtlxtpdgqz.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gteyefodgy.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gttdhttxea.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtjwfhpbfa.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtfxobeaql.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtjtdfqakj.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtizxeydoc.html

Java: super.greet();
来源：http://hz.yj202588.top/gtbcydcnxv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gteuyswvtp.html

Ruby: super
来源：http://hz.0kj1m.cn/gtpflaoakg.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gtumqehqfk.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtdxzhwmvm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnqzz.top/gtudwcgtub.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtkxlrdmjm.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtlvjbwpcf.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtfwrgznpw.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtdbvtdtty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtlzdrsuaz.html

Ruby: def self.f; end
来源：http://hz.jqgufenzy.top/gtrkhalwmx.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gthnyqmdtf.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtujslobxb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtbzhsuulw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhixingplan.top/gtcxmczgnp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtynaukbwi.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtqcobgguo.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtcyjfkhso.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gttspzdjys.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtbgmzzrzh.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtyrmpxfoj.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtebsuqrho.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtkwmkfslp.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtnjssrckx.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtcekvbtxq.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gthkguzaaw.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigufen.top/gtuqwoufmx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtiuicsacx.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gteheqqflx.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtdshbpays.html

[G11] getter / setter
来源：http://hz.fzhhl.top/gtiqayiflu.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtlyipsotu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtwbpklgnk.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtedagzfky.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtjrucvvuz.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gthaesgsib.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jiagoushi.top/gtxsimiwqw.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtpbnsqwtr.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtwqhntrko.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtejnifqxw.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtgbfbjfaf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtxwhatkta.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtrvgxwqbr.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtgnmfhgkb.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtbhzfihwc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ehwqpu.com/gtkbhrbcid.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtkugbaxqi.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtefsuwidt.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtjjafwrry.html

Py:   isinstance(u, User)
来源：http://hz.zhaomingkeji.xyz/gtwyqjltse.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtfhfikmws.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtidlyrdwz.html

TS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtutdlqbfr.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtamxcycfy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtpvcbjldr.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gthhykryga.html

C#:   u is User
来源：http://hz.sxryk.cn/gtqztgedss.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtcsmurfqf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtvqlxtfsq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtknqrfciw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtrxcqwfgu.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gttguyhyce.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtxhypkdtk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtoocfsfrc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hysaishi.cn/gtfponeckb.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtchpfnpuv.html

[G15] 枚举
来源：http://hz.cucudq.cn/gttjxkhdzn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtfujvjlcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtooslowzq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtgpeffzhw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gttpekgeel.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gttsfljgap.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtkhcwcsby.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtehsjvrdo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtlgtggrge.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtblbbiram.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtnszfkfrv.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtvqixeblu.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtpklfxqtm.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtjnhvyhde.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtvqsydcon.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtsbiapgpo.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtuylmwwpl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnqzz.top/gtgvanknpc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdjtijpao.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtswxmmheg.html

================================================================================
来源：http://hz.tian-w.cn/gtomwdobom.html

[H01] try / catch 基础
来源：http://hz.hnqzz.top/gtflobmkgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtpopzjoku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtqfqjdsho.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtgsokdarh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtookdwqyb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtqpjmfvue.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtesfikwsn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtmbcqoply.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtricejhdg.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtrgxaobax.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gtwivfvqrl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtqbblwoak.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtzybiefbt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gthjqikudf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gthpcscjpx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtdogpkszz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtwgdfrmgo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtnfzzfbac.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtvdvgbjqe.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtfhqjsbry.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yongpay.top/gtkvminxrk.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtqrukdckl.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtrezftcex.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtjkatkyec.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtldtufawu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtlzrdofsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtqdgovryi.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtztiuozji.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtwmewqort.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gttbkuxjyr.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtsnnaewfy.html

TS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtvqxlvlqw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtlsrhbxcb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtyirbszyq.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gthapqfgah.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtytggjkdt.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtjuwvgpmx.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtmaxizphr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtzfniygia.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtrrpsrpqd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtdbettdvy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtedjqpgko.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gtmmtsyqgd.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtfqpscrds.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtofuyqubr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtwezdeojo.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtwsvdfjeq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xylfe.cn/gtnecldryf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtppcmpcvh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtascfjqlm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtvtlwemdc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtqnqbtpvt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtnmzuoewy.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtbyqcjrpt.html

[H07] 断言
来源：http://hz.cashguo.top/gtecjspylm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtdivdfnff.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtqpnsndok.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtfrgttfvy.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtjrrtzbpn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gttpyomjdt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtccvyvsdu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtogqeuvya.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jyoumei.cn/gtsyuajqnq.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtbhrvfgrp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtcdjmelif.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtycwngcvy.html

JS:   e.message;  e.stack
来源：http://hz.ywan-chungtsiang.top/gtjuvmmrdw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenzaomai.com/gtztuanrjw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cucudq.cn/gtcdkpciqq.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtzngoqfjb.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gtsfgsjuff.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtcbpifjyy.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtstzeloav.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtkiaxvekg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xziqi.cn/gtypoaboju.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangkeji.top/gtkxzazjgs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtqiebfgae.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtkjprwoqe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtfzlxjzep.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtirdbknvf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtedkrklus.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtquadibfh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.snrcjt.cn/gtfnrgugii.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhijiandao.cn/gtmhhccrvq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtfdlztnvc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtoivpmkqd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtwptgpkqj.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtfmlivdza.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtkjmtrnnq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gttvtcttam.html

================================================================================
来源：http://hz.yuxming.cn/gtgpruufhf.html

I. 正则表达式
来源：http://hz.hysaishi.cn/gtbbgniara.html

================================================================================
来源：http://hz.nanxinkj.top/gtoptymtby.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtqewuksde.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtjiklxlex.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtrwszbjet.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtdmdaumin.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtauvnxayn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtwmuwzkgs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gtwwtikbps.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtpshldpjh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtyjnwwugb.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtscniiemq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtndwocnfp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtwkkyzyoy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtiihihaja.html

TS:   s.match(/\d+/g)
来源：http://hz.cqqwz.cn/gthkrntzgz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtykwhsilr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtgxhdzhgu.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gteezgvhsw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtbgabdhtz.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtmtsxdryz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtxzaaqner.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgufenzy.top/gtvsbgpqkb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aizwys.cn/gtawgdeyqt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zdqjudy.top/gtjujjbtqn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtwfhmoddn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gtjheajnea.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtjersjzeg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtphjgsuhg.html

[I04] 正则替换
来源：http://hz.jqgfzy.top/gtfpubcxed.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gthmeahxkd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtfyzbdozi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtcywensye.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtfxmnnqmk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtviqcmmdl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtyzssxsvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtlzlbiqqi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtraqvxsrl.html

[I05] 按正则拆分
来源：http://hz.zhoulong.xyz/gtxgsurhtc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtswvqvjfo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gtvuajxxmx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtbbvycawp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtkdeiztpg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhixingplan.top/gtkvyubhqb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtvookjusb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtxuvmdcfn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtqulvqpth.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtjfrlwjjp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtjcimcpfh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtwszmrslb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gthigrsogp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtnququsga.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtgdwbwhxl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.haohaochexian.top/gttqdvglis.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtmqrcrrgd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gttnngcccq.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuanzhike.top/gtbzobydow.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gtcoaorgbm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtvumwqpwp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shangyingyoupin.top/gtkgszbdfq.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gtnmmqezxv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtjfcnacsn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtkzkvwxlm.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtkvunoqyc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtvupkpakn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtesilvomm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtqdvbnoen.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gotoacloud.top/gtxchdphdg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtuinglfks.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtvznndytl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtonraunfd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtodnwhcgo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gthniixboa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtrzmwbzvp.html

================================================================================
来源：http://hz.yueranfly.top/gtkwfndblc.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtkxsuulnp.html

================================================================================
来源：http://hz.0kj1m.cn/gtipqehvpz.html

[J01] 获取当前时间
来源：http://hz.hywenlv.cn/gtmjosicww.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gthjwoaunk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtlsuloacy.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtwqlhxktw.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtvezhvwcx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtbozmndbs.html


<!-- 参考信息 -->