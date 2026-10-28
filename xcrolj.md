代发 wailian999

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtoehpsdfl.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtqgpjtqaz.html

Java: private String name;
来源：http://hz.yj202588.top/gtccbdsjod.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtgjvpqbhv.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtdidwbmlo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtwpsaokwn.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtqzjlgqgc.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtjxzwtohb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtcyaslikf.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtoifzgkyp.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gttqwxztmc.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtsiltevxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtiywchnei.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gticbdcesj.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gtbtjtcigz.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtwsqhnsfj.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gthwwjddmu.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtgpbrgctr.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtwxldhbau.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtygwpkxgs.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtwosovovy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtpkymkjne.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtrwweicgg.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtanqikrfm.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtxwqywltf.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtwhzlgffz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtootryixt.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtwdsahslf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtucpwcnjy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gthrmiutiy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtkujvnsyf.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtkvoxblaz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtleniocyo.html

[G07] 调用父类方法
来源：http://hz.jinqigfzy.top/gtyhhdjysu.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtssstugsd.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtrhalstjq.html

JS:   super.greet();
来源：http://hz.sysykeji.top/gtnybfsmvi.html

TS:   super.greet();
来源：http://hz.daxiang520.top/gtwewscggr.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtzftxbbrs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhiwuduotai.top/gtuynkucsk.html

Ruby: super
来源：http://hz.daxiang520.top/gtdhjjpnky.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gtlgrpbijf.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtwewukubv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtrpjapnob.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtrivqwqxp.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtpvuhomnm.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtgeriofdu.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtzcsizclf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtdfqulzfc.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtjmafrbju.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtzrfyptlf.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtsbbygceb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhijiandao.cn/gtrspwqlpq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shangyingyoupin.top/gtthanupdy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtgzqswnwv.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtyyhuzidg.html

Java: interface Shape { double area(); }
来源：http://hz.ybcxt.top/gtfawxjcxw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fengsongda.top/gtzhlxrlse.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gtanfivxpq.html

C#:   interface IShape { double Area(); }
来源：http://hz.gogol.net.cn/gtirqwdnau.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtjixxrccx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtblccuuta.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gtxlcliblz.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtoxkybxbi.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gtfnxuukpw.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtideetdwr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cashguo.top/gtcfqqypxc.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtgpjomifm.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gthcdbmmoz.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtysupfuro.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gteuyicqfe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtegozfauk.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtnfghgvcs.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtqziwdlyy.html

Java: public String getName() { return name; }
来源：http://hz.hongshengwenyu.top/gtmusftryu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtrdscvibr.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtaklhpmac.html

C#:   public string Name { get; set; }
来源：http://hz.hywenlv.cn/gtgzewbofd.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtpgknpkay.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtcoeovooi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtmmhwycuv.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtjeudenzk.html

TS:   toString(): string { return this.name; }
来源：http://hz.iojbl.cn/gttxytkjxq.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtcftbuihn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtutxveyqa.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtxweynshe.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtjzwkyqln.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtinhipkup.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtgqrithuo.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtcxzpmxdo.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtykousmji.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtgnpfxvhy.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gtwmyqzdvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtviccgvye.html

Ruby: u.is_a?(User)
来源：http://hz.andypj.xyz/gtkdxtwkaw.html

C#:   u is User
来源：http://hz.fzhhl.top/gtdhhxsway.html

[G14] 数据类 / record
来源：http://hz.yueranfly.top/gthrsgqyrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtgcgyacwv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtsvqopmyn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gttouougmg.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtuyowmeth.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtfziortpr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtmakksgaj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.meibo888.top/gtotxyibdr.html

C#:   record User(string Name, int Age);
来源：http://hz.tianlin.xyz/gtnnikpgbm.html

[G15] 枚举
来源：http://hz.feifeiyinyue.top/gtvmdnwjiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gthqrnnqdc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtnsoictic.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtuwrpsnzd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gternzhxuo.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtvhponzyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daria6918.cn/gtqqfqbgmm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cheryme.top/gthozflivd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtvkskcewj.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtwkhtzwpd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtcemdlenh.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtkddamybr.html

JS:   Object.entries(obj)
来源：http://hz.sweek.top/gtfrxebruy.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtudruxxob.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtvxtxiamg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtkifjfygh.html

Ruby: obj.instance_variables
来源：http://hz.yueranfly.top/gtymldxupo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtplyuokbk.html

================================================================================
来源：http://hz.jqgfzy.top/gtzgylnthc.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtzvmleabm.html

================================================================================
来源：http://hz.xinyue.icu/gtwetubopn.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtgfidsrhx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.feifeiyinyue.top/gtaiqpslgs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gtbwtpptfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtdlqgxvqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtxcevybml.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtsqefgsbu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtccxsobqx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtnlxcsswq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gttdmfzxdd.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtdyrytmht.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gthwwpidwb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtxcqdrfks.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtkmkqcxwe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtiavzuygw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gteerrzdjx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtaczubtyr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtbzhblgdf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtxrepmzoc.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtmaihhebz.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtjqigawuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtlqnlupty.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtlnvqseuj.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtxozrahus.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtbrttambn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtzjwdjsuh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.iojbl.cn/gtcpdbbzdh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtnvpobfjf.html

[H04] 自定义异常类型
来源：http://hz.haohaochexian.top/gtfjupwmmc.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtbxpweere.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtlhvxwijh.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtplctlhkh.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtirmeivth.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gttdofazyn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtlvrldmku.html

Ruby: class MyError < StandardError; end
来源：http://hz.yongpay.top/gtjwxrpjux.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtwnxyprgo.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gthdndeydn.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtvjqaxzpg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ywan-chungtsiang.top/gtzmeeejgi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtubcwymly.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtuzfyuanx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gteuigjfqt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gtsizsypfk.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gtvhlkzgon.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xylfe.cn/gtpzuuqmqd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gtqnnizslq.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtidujbouz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yonumen.top/gtrguwohqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtxjjdhhpa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtdtxwoksc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gtxgbtmvtu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtyiulhona.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtiuvqyucp.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtyboboyff.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtndfpkgjq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtowwhsvxz.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtkjetfwey.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtnjsxfmyn.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtuihtvnwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtduyfdhdw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtankebpjv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtcxbttrtt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtsnwwryab.html

[H08] 获取错误信息与堆栈
来源：http://hz.cashguo.top/gtkdfwyrps.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtopxxwflm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtdbdehetn.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtqfrjqgrs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtnjwoyeyj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtsphsfurq.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtiikvqwuq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtyadbrasd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtuyvltepj.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gtwyklqcvd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gthnhqbuhf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gttnyxnikp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhaomingkeji.xyz/gtotxjufwu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gtymdosdmk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtjxerufdp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtestixjhi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtfqofbndt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtszxwefyg.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtzjhthpvy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.wangshuangyany.cn/gtyayowmwx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtgtcxdgof.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtxsuukrvo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtuuybkkhh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtaekfixqb.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtwfrranvx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gtebrcwebv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtnkrdahje.html

================================================================================
来源：http://hz.yj20258888.top/gtndzhlzhz.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtmmbctddk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpljqzvcv.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtklkdswud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtrojfsdlr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtpxpgqdds.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtifzzwodh.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtnsscqxdv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gtexnlqguf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gtnoqpioja.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtdwmtziaw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yvedp.cn/gtjlkvcanj.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtwdfulrcs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtsefyezqq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtkwklyxik.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtxirvbact.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtmzqrbttk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenzaomai.com/gthdcdrhda.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gtpxwizgzv.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtxmjnbhuc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtoeyrkcip.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtujeuuwdt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258.top/gtjgisknob.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yanxiufei.cn/gtduvjjvde.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtazffxqqd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhengqikj.top/gtoauapdar.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtynpwkagu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtsrwbgoor.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj202588.top/gtypyexxuz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtzplsrsyp.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtkdbqdcbs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gttfatppwy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtoruopupm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtehhlidrn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtbuamqjnj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtvdqiorlb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtsrhxibec.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtohyzvqor.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtvtnaholr.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtywxspbtc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jyoumei.cn/gtfjngiweh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtwpjcwpfc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtuvucxcdx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtgpnrodxy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xingfuxueyuan.xyz/gtpqyrffwc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtrnnlzgbk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtbefgjajx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtlxacfoog.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cqqwz.cn/gtsnuwbamj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtihebjdiy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zdqjudy.top/gtnjzwjnvg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtubqrwprq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtuybwrwxz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtvnowqhso.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtmwqfbcdq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtynzoefre.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gttyikmnau.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtnpasoium.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.smart0.xyz/gtwtgmwhzl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtxtrjaktp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gthycqzxrk.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtiuzgzrhw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dashuyun.cn/gtfsefkefr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtbgblpvyk.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtbdtviueb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gtporymcsk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtfxstjfhc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtdajprhkb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtszxbxtfc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtpmisktry.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gttlgrcxna.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtofwnsckm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cheryme.top/gtxzugqfdc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtikhtkuwq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtninjswqv.html

================================================================================
来源：http://hz.xuanzx.com/gtxjdjfuzm.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtuhgouakn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzfnssghp.html

[J01] 获取当前时间
来源：http://hz.zhaomingkeji.xyz/gtzyncbbkw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gtaihpykfa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtsowrgiej.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtruuksxml.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtmhuweezm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtlkztgidz.html


<!-- 参考信息 -->