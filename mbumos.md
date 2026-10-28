代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtiwjnngya.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gtjzxtzmwm.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtpyngmruj.html

[G05] 继承
来源：http://hz.cashguo.top/gtxlxxjggn.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtdfnrylux.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtynlgxgzq.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtvvvnnbvq.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtnvmuwyuf.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtrjynlcwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sysykeji.top/gtceaisknc.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtognwtswb.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtiiqsvder.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtfzesojrr.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtkqtxzkoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtcogzxwcd.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gteoebxvnp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtuvlhobyo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtdgepcjes.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gthiiiclzq.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtivugepnj.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtcddfiqxh.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtcvriemoo.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtsqqwmzlk.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtbugovzxw.html

JS:   super.greet();
来源：http://hz.yvedp.cn/gtgnyshxnk.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtyjnpxmix.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtakixbxvr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ppjwa.cn/gtofergdmi.html

Ruby: super
来源：http://hz.ydzc1.top/gtbvhacuku.html

C#:   base.Greet();
来源：http://hz.daria6918.cn/gtbunmpvao.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtszvzkece.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtygupkvtd.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtqhkixdli.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gtmwbgopus.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtvxjbjdze.html

Java: static void f() {}
来源：http://hz.feifeiyinyue.top/gtenhmqutz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.316326.xyz/gtjtnnblrz.html

Ruby: def self.f; end
来源：http://hz.ppjwa.cn/gtvwxyugcx.html

C#:   public static void F() {}
来源：http://hz.gotoacloud.top/gtwuiycvds.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtfcxsurga.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtonejkdkh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gthkxstgxi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuanzx.com/gtsgepcnyn.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtajgihlho.html

Java: interface Shape { double area(); }
来源：http://hz.tanke756.top/gtryprcobj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtnpiqhqis.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtgfnbpnnl.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtfalwmjka.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtroxekony.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gtimirwheu.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtgpboxwqe.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtoqvqvlxx.html

TS:   public / protected / private
来源：http://hz.pycfn.com/gtaniayoig.html

Java: public / protected / private / 默认包级
来源：http://hz.yongpay.top/gtkrbgklet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtnhiohara.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtdhceumet.html

C#:   public / protected / private / internal
来源：http://hz.xuetiantiany.cn/gtpewxgxcc.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtnuqlhvfb.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gtltaqausp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtqwveawhg.html

JS:   get name() { return this._name; }
来源：http://hz.ivvv.top/gttdamwbvi.html

TS:   get name(): string { return this._name; }
来源：http://hz.shuidangran.top/gtygykihbt.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gteqqanxpp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtifmfnjtl.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtelneyntg.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtocgdzfkw.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtbxoqqfgh.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtwibccihb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtayoxnnil.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gtxgtzgmgi.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtneeuqzny.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gtdcqinqmo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtjdhnxelo.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtzenpsbkt.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtaacxbehn.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtqakltjcw.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtxstufqtw.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gteqmcmjod.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtfxsydxxm.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtfdcxcbhr.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtckyhfegp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtaliszbmz.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtibgtddsy.html

C#:   u is User
来源：http://hz.iojbl.cn/gtdtblpbgj.html

[G14] 数据类 / record
来源：http://hz.daria6918.cn/gtguwlvain.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gtjtdrlikk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtmmtkqffv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtyzztcmfu.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gttsgjmuea.html

Java: record User(String name, int age) {}
来源：http://hz.gaohongyu789.top/gtcliroulb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtwxywylvo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtfwnlroat.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtxggmlqdn.html

[G15] 枚举
来源：http://hz.feifeiyinyue.top/gtnvfgfdxk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtgtdyljua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtfvhsojoz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtimulobpf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtdabavtui.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtagydfige.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jlsjyb.cn/gtztmohcua.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtlmguvqko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtdlwcrxqg.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtqamvwppa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.snrcjt.cn/gtaivpljjh.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtqojdejkm.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtxnvmebgo.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtdvqufncd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtheqcgpay.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yonumen.top/gtzntargks.html

Ruby: obj.instance_variables
来源：http://hz.ydzc1.top/gtwhjkxbqt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ivvv.top/gtwambihqe.html

================================================================================
来源：http://hz.yj202588.top/gtawnhusib.html

H. 异常与错误处理
来源：http://hz.52xcode.cn/gtyvmvsqbw.html

================================================================================
来源：http://hz.cashguo.top/gtbvsxeknj.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtdlhsgaki.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtafpxiozl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtekyoatah.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtguaxsyzs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtfbpcxvzw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xziqi.cn/gtwehgynwl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtcnyofftc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nwbrower.top/gtzfncbjvi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtovpojevq.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtheufpdqz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtodkabdtr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtghwfylrf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtegilozfc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtqpkpjzfh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtedzoxgto.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gthxayzcwy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtvgrhzuet.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gtyrizlzou.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtdumiaetd.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtbeklypxq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtpafmrwnb.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtbzgkokyx.html

TS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtewmuwrbb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtrirkmfjl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtrqkpcyyn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtmzfyrref.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtqzcrrvqr.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gteukgqllu.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtzgymbcep.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtmdrgimpw.html

JS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtdirkthyr.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtytkyjejr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtggtriqyl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtfkixrqys.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtocxfgiqf.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtdycbokro.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtyyawjnkl.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtfrpayrfn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtnieailai.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtzfmzlohz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtkhisbpzf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.feifeiyinyue.top/gtqymonmsr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gttxqhggbh.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtrahwkfwn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtshbplbhm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtnwuskniv.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtbelamnik.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtdvduiqam.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtarqqptbk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtdccfcajn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtphyxthac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtpysiloka.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtctjkygkp.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gttxcytffg.html

[H07] 断言
来源：http://hz.fengsongda.top/gtebhfbbjs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtdkdldnsm.html

PHP:  assert($x > 0);
来源：http://hz.mhx1999.top/gtvnuwdlee.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtmtzkqoqk.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtcefsxuyc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtjvkxkcbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gteqsgzfkp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtpxbgkfwu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtynxraidr.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtgyzvgver.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtxvpkzsol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtnvprddfs.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtvsaxvvyg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtpjyzhdcl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtossccxhu.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtmgkyrtkz.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtkmknznre.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtyyamhvkj.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtocqrkokw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinyuanbaomall.cn/gtkhweatoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtywbdtigj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtoobyicsi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ybcxt.top/gtzslwobyv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtqljgdgzg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtibqvlgnp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtgnuyyqpe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtnovisjnr.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtrxkovdfz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtilaipjij.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtiixvcgru.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtamzvotdg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gthuficwfa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtudplgljw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtfrlhhqdw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtblznzona.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtbpmcxopb.html

================================================================================
来源：http://hz.yangfankeji.com/gtlwgcfuud.html

I. 正则表达式
来源：http://hz.zdqjudy.top/gtxeunlnfs.html

================================================================================
来源：http://hz.cashguo.top/gtkryeshhi.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtfcmmbjry.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtbuwcirje.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gttqdpcnqd.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtptoypogg.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtdboqjwdm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtgaeedrqb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gtiacejvvx.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtygigakmf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtbnhgollp.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtsjmcaozf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtmafaqkhq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtflqhrmuk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtzvpyfvkb.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxuanxn.top/gtdqbvupmh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtdudaxxxt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ppjwa.cn/gtejvcwzjb.html

Ruby: s.scan(/\d+/)
来源：http://hz.tanke756.top/gtcirjoimq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhengqikj.top/gtgxmrljfi.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gttmqkqyoo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtqgufuwdn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtowonbocp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtkqbvvuwc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ywan-chungtsiang.top/gtjlurruky.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.redwolf501.top/gtdqeqnkrr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtleampbai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtqvwonvcv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtuufeeeki.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtfzjommce.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxinkj.top/gtbakpgwld.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtynxghoru.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtsppkbhxn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtxpslnfgy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtkxbuggbv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtrnvgkgwv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtzancxpzc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtyotsbtii.html

[I05] 按正则拆分
来源：http://hz.hfpthk.cn/gtswhushzu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gteqihtfwh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gtxpmzstny.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtknrefpde.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gthauquiyl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtxscgucys.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtavuayvkm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtfivtmmlr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtanwrufsx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtxfgpqtxv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtxbjrencq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtfqfdfylc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gteeaoavmj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtknulmiab.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtcrhtysiy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtqndhlglg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtkfbjpksz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtbiccbxts.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtsdgcivoz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtvnmzlxfl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtspfrfhzv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtqvivuonr.html

TS:   /error/gim
来源：http://hz.chenlongwang.top/gthvrtujya.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtxvldrhfa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtistkhegf.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtokzwtsys.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dianchejie.cn/gtycmupkmh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenjidiqi.icu/gtbpalczsa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gtpopwcynl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtdfawkvve.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtprfzasal.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtkadueqio.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtaaqknjwo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtngtldgwf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtlhfgcdrd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nwbrower.top/gthbrsnctd.html

================================================================================
来源：http://hz.hammf.cn/gtrjjfueqs.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtuczsnmzm.html

================================================================================
来源：http://hz.yueranfly.top/gtwvajnukf.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtluekntdy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cucudq.cn/gtalsbzltz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtaizctwto.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtcdpbtrai.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtcdfcyhsx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtpovurjsv.html

Go:   time.Now()
来源：http://hz.yuanzhike.top/gtndvyonsb.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtxorjkbkz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jyoumei.cn/gtmeyjjdjo.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtyokjbvnh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtnguqbwbs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtacdozkhv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtlohknrbo.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtdtluiinr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gttxnjjckt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtsuitcyyx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtdomfjtdj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtrgcvytcn.html


<!-- 参考信息 -->