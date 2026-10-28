代发 wailian999

Py:   class User: pass
来源：http://hz.wangdashe.top/gtjnutlmyw.html

PHP:  class User {}
来源：http://hz.xinyue.icu/gtroelffjp.html

JS:   class User {}
来源：http://hz.cheryme.top/gtxpefflgy.html

TS:   class User { name: string = ""; }
来源：http://hz.ehwqpu.com/gtjwmqwcom.html

Java: class User {}
来源：http://hz.ppjwa.cn/gtytekrjlg.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gthcqreqiq.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtxzlogwwe.html

C#:   class User {}
来源：http://hz.birdmap.top/gtekislymm.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtelbpjlvv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dianchejie.cn/gtwarguyza.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtbcizmusw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hywenlv.cn/gteuifrmuf.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gttegyooxl.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtwwihpinp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gthtjivesu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fzhhl.top/gtabygicri.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtsupkwtis.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gthqvdjwkd.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gtgjupmzih.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtjmnboxvz.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtqygskqpi.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtpwuljryr.html

Java: private String name;
来源：http://hz.ehwqpu.com/gttalwtuep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtawlhpuyu.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtmcrqxxzk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtkokqhyyx.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtlpgoifyr.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtxexeydjr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtkulyoexd.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtfrpsegdg.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtsnumdoew.html

Java: String greet() { return name; }
来源：http://hz.jinqigfzy.top/gthufttycx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.snrcjt.cn/gtuvqwisgz.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtqwioorpa.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtcafawqkg.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtnavwvivv.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtwhuegxuh.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtornltmrt.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtcuscxdqd.html

TS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtlvmwtoxk.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtvtfikyhc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgufenzy.top/gtgoxyzwnq.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtbzeaarlw.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gthwknuabv.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtdmedkzkj.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtkjednahd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtphcyyzbq.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtyeibrhya.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtylcxfska.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtfyekxncd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtxebcjrwv.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxinkj.top/gtyjfrwjvi.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtpuoqehkx.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtaeqvfwtj.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtoasbtafb.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtjsvjwrgl.html

JS:   super.greet();
来源：http://hz.iojbl.cn/gtljtwbkyl.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtfgoiscwh.html

Java: super.greet();
来源：http://hz.guannengcc.top/gteakzurcw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtiiwpyxvh.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtcwkbuxkj.html

C#:   base.Greet();
来源：http://hz.quarkkingdee.top/gtwichbbks.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtuxldmfzg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtvngbzqlp.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtjzlgjaxj.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtgjrfxgas.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtjnxtrqeb.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtufwcrdpe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hongshengwenyu.top/gtzyxtwihz.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtsyrsljfc.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gtlgjitphx.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtvvlwvhrr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtofslljrk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.andypj.xyz/gtzpwutlpt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtpdwhowew.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtzfamdjda.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtqpoghmir.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtrthznvcu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtjcgpiwqp.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtidhrklpq.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtcvobzjan.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtolofuryp.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtsqdxmpex.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtiyqqlbur.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtwmnfyzlc.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtodnqolul.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtotpkwiee.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtofqnttgm.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gtlxbattuy.html

[G11] getter / setter
来源：http://hz.c1oappe.top/gtthekqsmc.html

Py:   @property 与 @x.setter
来源：http://hz.chenlongwang.top/gttmmddoyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtwxycrsum.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtobyhloob.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gttgtsyxoc.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtyqtgxqfq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtrrzfrnfi.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gtmrltrqxo.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtertffuth.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtnodcchhw.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtxexhjhmq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtxctmmfhs.html

JS:   toString() { return this.name; }
来源：http://hz.jqgufenzy.top/gtqjmxswqi.html

TS:   toString(): string { return this.name; }
来源：http://hz.meibo888.top/gtwvkymbow.html

Java: @Override public String toString() { return name; }
来源：http://hz.yvedp.cn/gtfuhicutk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtwshiybdt.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtxocafveg.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtthtslooy.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtpikmjpkx.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtibsqrkgw.html

PHP:  $u instanceof User
来源：http://hz.kuanghao11.cn/gtmqvcxsba.html

JS:   u instanceof User
来源：http://hz.c1oappe.top/gtzglgjbkz.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtprtdxbja.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtocdtgvtk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtkmrbcetg.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtwvnkiqjo.html

C#:   u is User
来源：http://hz.xuanzx.com/gtrfgocept.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtcbqnpnne.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhongyouzk.top/gtkjrphelk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gthuhfoabu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gttdiepsiu.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gtdkcskvmm.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtxzgaiblz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gtsteczhpk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtwdxivjlj.html

C#:   record User(string Name, int Age);
来源：http://hz.pycfn.com/gtwgfidmxx.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtwlucsebm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtnloumaga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtoqvvlxmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtrxhcvakl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gtqwdxauuu.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydjk.org.cn/gttquhjuqz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtdygbxvsp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtiagnefsq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtinfhbzdx.html

[G16] 对象转数组 / 字典
来源：http://hz.gotoacloud.top/gtzticiwdg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtzxgtoeux.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtppimhffd.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtrzxhsosq.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtgrjxtoba.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.andypj.xyz/gtpvtilwzw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtbjpvyifg.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtniqjsxmt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtsoscihrk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtuwhoymps.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtdvjcvzof.html

================================================================================
来源：http://hz.svipenyu.cn/gtpgpfjnji.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gtxiocukhw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtajszcona.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtkawrwzdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtizzflqod.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydzc1.top/gtjdssshfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gttieyrzix.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtjocbhwpr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtbbqelzjg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtfucfhpug.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtunpjeurz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtlkmtszmt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtgqfsitko.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtuqkfekpb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtujgxiyew.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtauifmdmb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtziksnouk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gtsgqcxnlu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtdhoiteqk.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gtszaflxja.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgufenzy.top/gtgdoqhrls.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtayaaxhlk.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtfccivuje.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtbsjxbdtc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gthoavkoxt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtifvnqznf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pycfn.com/gtorbsvtyz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtsdebczor.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtdgvjvhfx.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtrofrsvkx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtcscbakad.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gthcymxyox.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtnmqvpvls.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtjlyjeojl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gttxpwutkr.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtzjugzrfm.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtgzlpvqdn.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtnsyyzshn.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtpvrqviub.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cucudq.cn/gtralclxwp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtzlfzittc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtmqlmgblk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gogol.net.cn/gteyhtltbx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtajgbcolb.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtmyxegbqi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jianghu66.top/gtgsvptlxy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtzympsknh.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtoizwuoze.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtsgxskrnp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtqldwqoem.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtfkaaanmm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtcibtbepl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtizelcuat.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtjbtmulpm.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtexuqeoka.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtmsilvtuc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtszqqpmoh.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtohwldthn.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtjxwjqsrg.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtcbwvqjdr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtyapbhzvn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gthlumpxzi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gtkmmecfol.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gthaaiqlei.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtruaiktnx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtueblgbqt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtfdhlqlei.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtwdvhyhqu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtsgqslxqk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtmtejbulk.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtbsjpmute.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gttyvjflsj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtcdkihbdr.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtkvewgpsr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtrwpjzcuh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtavhzoddh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gtllmyrobs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ybcxt.top/gtbbvpbcax.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtitqvxlag.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtxszcdmrr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtkxzgbqfp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtgsxolndh.html

[H10] 资源自动释放
来源：http://hz.ydjk.org.cn/gtlnluxpld.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cashguo.top/gtpkblkyip.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtugsrkmuy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gttwqxmcdg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gttzmicvtq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtpjhtrzkh.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gtlujbrieu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pycfn.com/gtmbsgfxxq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtzdymoyxe.html

================================================================================
来源：http://hz.shuidangran.top/gtdmfunzqk.html

I. 正则表达式
来源：http://hz.yj20258.top/gtmvnmgptw.html

================================================================================
来源：http://hz.jinqigufen.top/gtmxfnoblv.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtnhaerhuk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtzsfithza.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtorkfouse.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtspgxouba.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtmlnspfzd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtisdmeinz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtfvhbgmjv.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtqflytlal.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtugrljkzp.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtmpqnozrv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtevzhdkvv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtoxezzsdz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.9152youxi.cn/gtuasoysjv.html

TS:   s.match(/\d+/g)
来源：http://hz.quarkkingdee.top/gtgqivysay.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtsdbktpun.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtmhesbzbz.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtolnlfptc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtbnjuzpuc.html

[I03] 提取捕获分组
来源：http://hz.wangdashe.top/gtyrkajrkl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gthhirnolu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gtjidqtods.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtablvfkuh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtaqtqmpxz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hnxiangtu.top/gtqskqyyek.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtzisspuny.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtghuhzrbu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtpkysawsl.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtrujwmdwq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtrdfptxjo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gtvcslhluf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtpgwtyyrr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gthteckivx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtmqkjbwij.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtjlkctsre.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtlfjbdkpd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258888.top/gtmyerlvfv.html

[I05] 按正则拆分
来源：http://hz.zhengqikj.top/gtjqvtjvrh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtwyhmkyqx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtzytaffkw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtzigupinr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtyksjtiqk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtvbfgjdsi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtmdjlhztf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtodvbfgbd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtolkjxyvi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gtpeafrrhs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtuztutcxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gtqtyumdhu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtiiwskllj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtzxnomitb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtwqttmmkv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gtqyzhaier.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gtehotwils.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtjlytimre.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtakmphmyw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtslzqerxh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtkarwfndu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtfdvulttv.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtjfjabsqh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtufnhswvh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtsqnlsbpo.html


<!-- 参考信息 -->