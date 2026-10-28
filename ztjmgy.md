代发 wailian999

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtwbinzahw.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtopkglrre.html

Java: private String name;
来源：http://hz.jianghu66.top/gtkqjyqfgi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtneupyjxe.html

Ruby: @name = "x"
来源：http://hz.dianchejie.cn/gtvdvjwhpr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtywvoupob.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtoyhjiiiz.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtotnrvkzu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtbywswcgl.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtxsozohnu.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtxiubojzw.html

Java: String greet() { return name; }
来源：http://hz.chenlongwang.top/gtybbqtjgs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtnkngwkfh.html

Ruby: def greet; @name; end
来源：http://hz.yongpay.top/gtvcvpqjun.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtlcuundhs.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtfaezczat.html

Py:   class Admin(User): pass
来源：http://hz.0kj1m.cn/gtwcmirewb.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtfkqixusj.html

JS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtiulucxsh.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtcnmmohdg.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtrvcuenqf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.feifeiyinyue.top/gttauszpsh.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtlzbuiuuu.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtvyognuad.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtvepbkrwk.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtlhsxjprt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtvjigbfun.html

JS:   greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtpenkbmwu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtlzfqghgl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtoxmxyahc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gttndftzml.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtpesmpthx.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtwboubrjv.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtesehqaog.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtsnuotnnc.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gtyypnqbix.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtwmjtnzsa.html

TS:   super.greet();
来源：http://hz.zdqjudy.top/gtibsjkeht.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtgyfudzah.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sufxvd.cn/gtrajovouq.html

Ruby: super
来源：http://hz.redwolf501.top/gtuziaeeec.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtxvfzwshg.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gtnecvqxyz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtfaoyytxf.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtglxapari.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtcorszxzu.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtwlgzhqju.html

Java: static void f() {}
来源：http://hz.hongshengwenyu.top/gtowprzisy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtozgqhcmw.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtzrjaljdn.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gthlqmjnsa.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtjyaodokg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtwbcztupe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtgajeqcgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jianghu66.top/gtbqjnrczr.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtkbpvvayv.html

Java: interface Shape { double area(); }
来源：http://hz.ydjk.org.cn/gtupviwpkf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtotmzlpoy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtccdfufch.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtlblbotld.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtvtnupzdo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.c1oappe.top/gtnohjabfd.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gtinpbkhfe.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtxflnqviw.html

TS:   public / protected / private
来源：http://hz.ydjk.org.cn/gtclbtdtgj.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtyxnikdxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuxming.cn/gtlingakqi.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtedtejcoc.html

C#:   public / protected / private / internal
来源：http://hz.zhoulong.xyz/gtfzhqlicy.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtubxdotaj.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtsszxaucx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtrfryjtbv.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtbyrcbgrb.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtcenyicoh.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtxmegrand.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtidyyzwss.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtgciiozwz.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtoktmfckd.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtxfxiezfg.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtbwedmoiw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtrkuakuyz.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gtuugdndeu.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtywcyymzm.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtjrwhewkx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtpnahgzen.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtzkbmmpag.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtuzxnusbt.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtbpcnecdq.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtdrlmgfhk.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtgsysoxwy.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtkvloiibz.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gttbvzvzjx.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtrffgbznk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtntzcouxt.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gtcdqvwraj.html

C#:   u is User
来源：http://hz.hnqzz.top/gtjmztlehu.html

[G14] 数据类 / record
来源：http://hz.hfpthk.cn/gtocnhyxzx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtffebihcm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtukylfcel.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.52xcode.cn/gtgzpmmrxj.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gthgwtcxdo.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtpybnlgwi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtckhvnwzo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtzbvtjscw.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtgmmthyog.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtqhxtwurn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtbuoyypdd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtariilkim.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtajbzlkin.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtwamvhpzm.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtxjbkkcbf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtdgqrgevx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtrgntcbri.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtmronxdji.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gtqbhseigk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.52xcode.cn/gtvnybmrhk.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtxnpbtlte.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtnfivxjkx.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtzmiqjsai.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtofigqsqd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtlkyelfrr.html

Ruby: obj.instance_variables
来源：http://hz.xuanzx.com/gtzkaiycuj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jyoumei.cn/gtqcxgeviy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtavleexvk.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtneexpxnj.html

================================================================================
来源：http://hz.gogol.net.cn/gtyzavtpgo.html

[H01] try / catch 基础
来源：http://hz.ivvv.top/gtykzkyibc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gtkppkacti.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigfzy.top/gtozeodtdo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtcjpbkcct.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtfgqbthmk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtugtbvbfc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtvcavgjwm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtdgptbdxd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtzkljbpsc.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtnvavhigi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtvxkvibti.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtijysdsup.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtpjbbwbwk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtiylwoxtu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtmlyqlvvj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtmetbchix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtnbsargbs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtctujlgei.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtrqgiggcm.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gtfvpxruub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtrzpbzkqn.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gthypwreeq.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtujymilps.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtroyqfeui.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtlguyufhb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtxsbprqnk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtutwkiqmy.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtkeobhulq.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtvrtqeyjc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtvwqhruyv.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtvkawsppw.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtfmnnhhgv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtvxanalbw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtbkxfselh.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtuwmjcqfk.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtsuimnzxj.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtqirmwaam.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtrfydjsln.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gthhsiewdz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtrstvngok.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtrwiregvd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtxysuinvl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gtqxqhspit.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtwkueduvb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtdclknhwk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtcyktsdzd.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gtehwbzfde.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtkgloqumc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtzdoiinzf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtinpvndiv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gttfbduwui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtzcofpuxn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtltcbctxp.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtdnncfbzj.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtfptmfamr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangtech.top/gtxlygqztq.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtvcshcqcd.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtzmceyyof.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtwndenibx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtzpmbcwxn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtjawovuzl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daria6918.cn/gtaxelpdkj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gtydcxcrss.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gtqqxjmzgi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtskfpgmjg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtbzpevdhm.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtxhinajqi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tian-w.cn/gtpbgnblpv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtspduzjnb.html

Go:   err.Error()
来源：http://hz.wangdashe.top/gtnndjhmzo.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gtqmqkxbhw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtxqaxsock.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtcqrprecx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtuoryyloc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtpfnvfxla.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hfpthk.cn/gtxhktxwut.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zdqjudy.top/gtyrfoncji.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtcnkrnbyr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtryasrknv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtojbtqylp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtqwsnhktg.html

[H10] 资源自动释放
来源：http://hz.fengsongda.top/gtdtjrvgcg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtijbmdcom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jyoumei.cn/gtlicsnngp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gteeorzygd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtlzdpytwu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtnvikwvor.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtqkmolhpw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xinyue.icu/gtgkkiepak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtlzqvucon.html

================================================================================
来源：http://hz.iojbl.cn/gtbxfrvvnk.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtzzdaigdt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtghwbogfk.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtgdsfkrkg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.0kj1m.cn/gtaxvpiqlp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gteacshbjd.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtjadqwdlf.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtmuysupaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xingfuxueyuan.xyz/gtpkrucwfa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtengzlmcf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258.top/gtxznqczip.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tian-w.cn/gtnlpgeyoi.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtghwughpu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtvworiynn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtnwbaggwa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gthkqhtmqc.html

TS:   s.match(/\d+/g)
来源：http://hz.ydzc1.top/gtrfnjxvij.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtlvmsavyn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtiaqrqpze.html

Ruby: s.scan(/\d+/)
来源：http://hz.shzxlz.cn/gtwfpohwvj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtdbdkzlkj.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtfsshrxbl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtjgfvwerd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtnsvvuxzz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtbunnwwqf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtwycsekpp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtevgsbpvn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtndfmxguu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtzgncucqt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtwehhwndh.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtfjdfkxxh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtvzudlopl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtddvqdhis.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtxgxtrtdd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gteljdnjdi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gthgsrisje.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gtmmmkdswg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtopizhknf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtzhbmxiqr.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtnvumegwg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtpiyrqetq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258.top/gttnakeaon.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gthiveqbdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtoayatmmv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aibaodan.cn/gtdvvmjvqj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuanzhike.top/gttxwzhfkd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtfxxcfuqv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtrpkcpqwb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gthpvkxpws.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtdfdncpkm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtegophrav.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtyxurezqc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtsfyhxvjl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtkafkwtna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gtqcbmxdhj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtcirkvznd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gthayhutfy.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtglsfzfxz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtmdfidnxi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gthjrcbhlk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sufxvd.cn/gtrhhohqii.html

TS:   /error/gim
来源：http://hz.cheryme.top/gtpkckcprh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtcapgufew.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtbsganwyp.html

Ruby: s.scan(/error/i)
来源：http://hz.yueranfly.top/gtjqftsgcn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gtslfrkmxj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtcliudsid.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtficsrpzp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtcwcsrubg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtfmmzopog.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtunzgndpe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtlbspkdrb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtovaguimc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhiwuduotai.top/gtvfpxcszo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtahvhohtx.html

================================================================================
来源：http://hz.birdmap.top/gtmzpntqox.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtalubsflf.html

================================================================================
来源：http://hz.pycfn.com/gtzpbzytdg.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gthwtqswga.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtxdffhbim.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtahmfgatm.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtfcprsjtj.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtojusbqte.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtvaarauyz.html


<!-- 参考信息 -->