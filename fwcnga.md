代发 wailian999

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtxwziernb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtkehbwjai.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtxbgalaoq.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtbephlrhu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.birdmap.top/gtxwdxsvxy.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtcakvzvap.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtjqhhecqv.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtlimrypyq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtqmjpwhog.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtquuqscxd.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gteznckzvw.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtyxtbypzu.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtbxyzekld.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtqribanaz.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtncxetzod.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtwetmioox.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtilfepszh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtteuxsnxo.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtxlalmhnz.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtmhbqwrty.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtlgakxfhf.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtzaxfmdkt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtoczqwgky.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtdirchouq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtnjevunyp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gttivkkvse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtonmsjnpa.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtqlgcvjhx.html

C#:   public override string Greet() => "admin";
来源：http://hz.sysykeji.top/gtaekjurik.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtysoagyxs.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtnwnposqb.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtdfaaqjxt.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtydbnoacp.html

TS:   super.greet();
来源：http://hz.chenzaomai.com/gtywrfjbun.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtzlwtvpqx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtqjjgjqqc.html

Ruby: super
来源：http://hz.yj20258888.top/gtycfnwbcu.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtpapyhoen.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gtjedttzen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtwjcyvzvh.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtisrogzeb.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtpanatkut.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gtbvaoplom.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtoehpwxaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtialgngyg.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtknsysyat.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtifaomkan.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtcqatqbie.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtvfqrtwkc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtzzsnfvrt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gtqbbdkjeg.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtlovpbrpk.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtkdlhfqgs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cheryme.top/gtvrbbycix.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.iojbl.cn/gtmpwupwml.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtvjxceddz.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gthejngkct.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtskpxcgen.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gthzqglwpf.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtfyloflsm.html

TS:   public / protected / private
来源：http://hz.jinqigufen.top/gttwhkvskh.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtuvrefiht.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtmxwhmbpa.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtaaggxeyv.html

C#:   public / protected / private / internal
来源：http://hz.ehwqpu.com/gtzkciurxv.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtaggjxrpp.html

Py:   @property 与 @x.setter
来源：http://hz.smart0.xyz/gtqtkbaqli.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtrcirebox.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtzqsjjsae.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtybycwgrl.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtevjfzvwt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtvwozzacy.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gthjfgmvnn.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtumrjrogz.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtuykvfngo.html

Py:   def __str__(self): return self.name
来源：http://hz.yuxming.cn/gtakrddxlz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtvvyvtflh.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtvtoqwqhf.html

TS:   toString(): string { return this.name; }
来源：http://hz.redwolf501.top/gtqnviwfzs.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtnidsyppz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gtbcsclehz.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtudisxdyv.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtnxhzrlvi.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtwnyprxhr.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtmxwpfnhb.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtnwcbdfeq.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtjyshxlvc.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gttgalmfcy.html

Java: u instanceof User
来源：http://hz.smart0.xyz/gtooksqhlk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuanzx.com/gtlvpgzvli.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtnvphbswp.html

C#:   u is User
来源：http://hz.ydzc1.top/gtcirynjkm.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtwluftpts.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtbatimzme.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtryvhvavs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtptrtiesp.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtapjgwqln.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtqwpzepai.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtpnitxfeu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtwecnpevl.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxuanxn.top/gthibcyayr.html

[G15] 枚举
来源：http://hz.cheryme.top/gtoesyxyev.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtkgjajeuh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gtwoqcfseg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zdqjudy.top/gtnmvhzhhr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtzjstrrhv.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gtomgsecvw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtsbhcyrhj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgfzy.top/gtyxdjjvjn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtchnxiwtv.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtsujjtuka.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtqfhdrmkx.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtxhkdtcjh.html

JS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtywdjufks.html

TS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtwwvuowbz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtzduxogas.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtwbgrueqh.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtzavtdzwy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtalsxjgvu.html

================================================================================
来源：http://hz.cashguo.top/gtnaxlfinq.html

H. 异常与错误处理
来源：http://hz.yj20258888.top/gtmszkwhow.html

================================================================================
来源：http://hz.yuxming.cn/gtddfuhpwf.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtghusliub.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.c1oappe.top/gtqgjxzkna.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenjidiqi.icu/gtuofuigfx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtlvqxujpt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtuwpnidfc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtyfuqhjde.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtmlmklcxx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gtjjlqcyjp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnxiangtu.top/gtpprymhid.html

[H02] finally / ensure 收尾
来源：http://hz.nanxuanxn.top/gtylttkhul.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtmhfmgtki.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtvzacdmdw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtwdnzjful.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtpllzcopu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtmaqexrsj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtkbinegly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pycfn.com/gtickoqtkm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtbibxlzqn.html

[H03] 主动抛出异常
来源：http://hz.guowangkeji.top/gtksnmwqbz.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangkeji.top/gtekvqvuhm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtvwurbuwp.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gttjdbvoeu.html

TS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gttnhhhhzw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtmeqcbwkb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtknsdxbhf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtaojskhaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtiltwyhmo.html

[H04] 自定义异常类型
来源：http://hz.jqgufenzy.top/gtvdgfzbtw.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gtjyaiubmu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gttizljmco.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtiimffule.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtltqbkbea.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtsowtbplv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gthcbpgmwp.html

Ruby: class MyError < StandardError; end
来源：http://hz.hongshengwenyu.top/gtologhfiz.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtnbzvmxoz.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtbwedtxct.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtfqeaazmx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.quarkkingdee.top/gtisjqmzlx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtgmhvlpag.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtitjtccqa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtgkttledp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtbgodfvxh.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtvkvmruki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtwjgujxzz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtcbttildv.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtupkoubkt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dianchejie.cn/gtirfwedpj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtzoxyfenn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gturzetzso.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtreoerxhm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtenxzcshs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtpsuoymcv.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtcthwxtob.html

[H07] 断言
来源：http://hz.cheryme.top/gttqvyvsnq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yonumen.top/gttltxuyjf.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtqdjklamt.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtpsbjlfwu.html

TS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gttnmtgdwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtntgdelan.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtkqxhebwg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtuvweesoc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtrbphyqfq.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtnqngbrgs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtcqqpgypo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtoqxrvush.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtypnunypm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtfmcywoup.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtmcnhrckx.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gthyknvfsn.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtbeizannm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtevxprfjb.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtjdwqxnvg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gtfppcluvo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtxjgcknxe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhaomingkeji.xyz/gtpgwngbgb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtqymmbsga.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtxtawxrdq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gttmjzkxdp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtabvxyxwo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtlgjthbmn.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtruswgnhg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shzxlz.cn/gtfzvxprwo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtydqnjkic.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtymvvxuzm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtobizhjou.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.andypj.xyz/gtioorhtwt.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtarsfflld.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtkacfjwpi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtxnrwxfll.html

================================================================================
来源：http://hz.yuanzhike.top/gtdmfipvcr.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gterbdnwbr.html

================================================================================
来源：http://hz.cqqwz.cn/gttbgpeyax.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtdmqprwbi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtnrbjnhut.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.9152youxi.cn/gtmveqlqeq.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtcywoljbh.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtgktbjgim.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gtudfcxisu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nwbrower.top/gtqpzdgvuc.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtdmrvgalt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtjfyiiqia.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gttzkcyeex.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj202588.top/gtielhghig.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtajburhcg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtnzybbzag.html

TS:   s.match(/\d+/g)
来源：http://hz.xuetiantiany.cn/gtnvxkqymp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtqzuqwkel.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtegutjdkc.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtxygjolql.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gthomcxrix.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtgvmbhjmx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtzgqzlqds.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hammf.cn/gtotnyxtez.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shzxlz.cn/gtggacgkcz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuetiantiany.cn/gtepfhjoaq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtrnswyyvj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtfvbvamur.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtqwceyqjv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtgjtahzph.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtvxrpsela.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtblkdjpts.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtrnfvgtfq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gteewchusc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtwhfrxsac.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtugktvyoe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtbyyewbwm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtxzkxsdcd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtlocafbak.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtzmfocore.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtmceaovgg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gttjdoyqtk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtauasblwv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gthhyivqhc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gthbltlbxu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtvbbvtwuz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gteyajkxtj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gthimopfta.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gteinifier.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtdcbyzzqy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydzc1.top/gtigehwfpu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtzrsibdav.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtegtmzumg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gttkfusary.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtjkzqqene.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtsoohavcp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtzzgakwyi.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtfmvoljsq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtfpjdsyik.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtgjdekrwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtgiydeaoh.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtidylxiwa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtasevkpnd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtprzbafgw.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gthundjymu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gtxsjxvumv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtsdbegqea.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dianchejie.cn/gtdepdtzua.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtvjlfykwx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gttwfgzwux.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtbaujlovp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtpiubycgf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtoogrohay.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtxvajvivy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtilihnwzj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtewjlhgez.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtyasfhuvr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsvludemr.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gteknmpyod.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgfzy.top/gtewmicojv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtxcnjsfff.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtaibdtdbk.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtzpawlhpw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yvedp.cn/gtpxlexbbn.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gtbojwlyth.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtzwdnolck.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtwyzlytje.html

[J02] 格式化输出
来源：http://hz.xuanzx.com/gtmwisuttw.html


<!-- 参考信息 -->