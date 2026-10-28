代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtluduikbi.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtdoewlyrw.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtdwintkbl.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtqfsrvzpf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtuarqcanl.html

Ruby: def greet; @name; end
来源：http://hz.jianghu66.top/gtynyyipmo.html

C#:   public string Greet() => Name;
来源：http://hz.dashuyun.cn/gtdfymyttq.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtgupnxjma.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtilxqxljv.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtstgfjybj.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtwbigrlhf.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtxvkpimxi.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtawxhyoom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtohccixai.html

Ruby: class Admin < User; end
来源：http://hz.quarkkingdee.top/gtibmvgzui.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtihcqmwao.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtcmmjtuur.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtesaqdcmu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtjphwbyjm.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtyozbhrdy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtdyudyksc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtzrxyjawm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtsdzwfqrv.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtsnazmvre.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtsnaiffpe.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtbknabwbg.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gtxownkcyy.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtofmtnigu.html

JS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtgbtqgtgp.html

TS:   super.greet();
来源：http://hz.sweek.top/gtybreyfkg.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtwvfbsyge.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtzjnnpvxf.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtrkelaqza.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtiryrhvtn.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtfeasfden.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtpgphinqa.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtapiepcyx.html

JS:   static f() {}
来源：http://hz.ivvv.top/gtsjlgoibt.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtoilzzljq.html

Java: static void f() {}
来源：http://hz.tianlin.xyz/gtzvvyjjng.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtyoavlnkj.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gttsycvcxq.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtmyziabqw.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtajlwcivm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtgiewfgwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtiumwsnpq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtbvatukyk.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtovkcilkw.html

Java: interface Shape { double area(); }
来源：http://hz.tian-w.cn/gtorsvuhck.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtfglzjelx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.feifeiyinyue.top/gtycmefdes.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gtufrjxure.html

[G10] 访问控制
来源：http://hz.feifeiyinyue.top/gtpfruxopv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtixrgunbc.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtnyndvett.html

JS:   #private 字段；其余公开
来源：http://hz.ybcxt.top/gtjdwcytbr.html

TS:   public / protected / private
来源：http://hz.hnxiangtu.top/gtoqzygefm.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gtfvtoifrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtcshgtvwm.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtdvlinvao.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gteuvmpcse.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtyhwizltu.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gttilkzdbz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtoklwuwyy.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtnqsjfuay.html

TS:   get name(): string { return this._name; }
来源：http://hz.cashguo.top/gtgticvdwt.html

Java: public String getName() { return name; }
来源：http://hz.fzhhl.top/gtjzyngrxm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtmhvbtsqw.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gthljucyen.html

C#:   public string Name { get; set; }
来源：http://hz.bjfxy.top/gtwlhvtjce.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtqsqcixbz.html

Py:   def __str__(self): return self.name
来源：http://hz.chenlongwang.top/gtlmxpxmxn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtlazdzvhw.html

JS:   toString() { return this.name; }
来源：http://hz.vqdsnc.cn/gtteilncgd.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtbenqpwsf.html

Java: @Override public String toString() { return name; }
来源：http://hz.tianlin.xyz/gtqiejkttr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtkujcoevf.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gtfiltnrfp.html

C#:   public override string ToString() => Name;
来源：http://hz.shuidangran.top/gtkqrpynju.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtbeaedjjy.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtwfofwgmk.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtpvzvgbgq.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtojpbtfkh.html

TS:   u instanceof User
来源：http://hz.yonumen.top/gtaabaiyra.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtdlhftzcg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gteskkobuo.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtdemkkupb.html

C#:   u is User
来源：http://hz.316326.xyz/gtafvkefzg.html

[G14] 数据类 / record
来源：http://hz.yueranfly.top/gtdfylnrux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtkyxmuifo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtjdiqyrfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtxlldbbem.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtvzbtldni.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtgldxsayb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gteuudycgn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gttknjhjfk.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gtdulrnowj.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtzcvzjwow.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtlaiwyoyx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tianlin.xyz/gtlllgryus.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gtlqsmyaup.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtqhptjjxs.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtqwbbqqts.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtmlqrzvaq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtknorltyb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtzakittmd.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtdhmeznzt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtfxgbjhny.html

PHP:  get_object_vars($obj);
来源：http://hz.316326.xyz/gtcktjooxk.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtqqxnhdto.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtddkohlwt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtdqnjfmjy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtmjbbepun.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtqnqbiair.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gthibtgbbh.html

================================================================================
来源：http://hz.yueranfly.top/gtlahfzwdz.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtepwvizca.html

================================================================================
来源：http://hz.316326.xyz/gtjzrnyaau.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtemgflbzb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtyyhjkqtn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtxyeexihs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtgpviwqcw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtudnvklee.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtqocndfya.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gtjobsuuaa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtjrhlmgif.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtcwdebpou.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtzmhrclak.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtjgebawfa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtfrvmpzvc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtestjvmdk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtrbmrixxg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtfftpmsyi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtfzniylng.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtaxxcujds.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtipezmhgl.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gtyxtmmtny.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gtbplhjqvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtmtvrflwb.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gthnfdicja.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtdpurylie.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtzenohvyd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gthgfdnrtw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.316326.xyz/gtmqjnerdt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtyvfipibu.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtkzbfrokv.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtilgbjlei.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtdvhudtwr.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtpuyifbei.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtyijpdajw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtrlaxxunw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtcuuponkt.html

Ruby: class MyError < StandardError; end
来源：http://hz.guowangkeji.top/gtswzanqfs.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtqfhwjgst.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gthreouayd.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtyqsidlkg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258.top/gtxqdqgtwg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtjymjoghi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtiwuzvdce.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtfpulqbnm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtntvrhhpe.html

Ruby: rescue ArgumentError => e
来源：http://hz.ehwqpu.com/gtfijhbnjq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.vqdsnc.cn/gtqqvmcmah.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtvtglqwoy.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtxreqjbkq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtdcrdyxba.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtinctnfuf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtawqlvyui.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtybezeavy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtpvnotcfn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtrikeapoe.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj202588.top/gtrdbsxzdh.html

[H07] 断言
来源：http://hz.vqdsnc.cn/gtwqhhfykz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtnxsxvpus.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtmoxzihxy.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtmcyrfbct.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gthdmvpdgb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtovdyoeyi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtjsjwftqd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtlilxicyo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtukscotkk.html

[H08] 获取错误信息与堆栈
来源：http://hz.xziqi.cn/gtwjoorvrt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gtbmlgikob.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtehqdcwgi.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtlaraphzz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtsiskylrm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.meibo888.top/gthzdrvedk.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtcshhxyoe.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gttwjryovu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtklendygz.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtijbmnyts.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtyssajvyd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtabnkgeaj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtoucoacnd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtukbhqnzh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtdevxuklj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gtegjcuxgt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtlkfxvwtt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtxwudpkal.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtrybmyqyw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtbaptreix.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aizwys.cn/gtwfcjjuzv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtppodkzfc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gteldzlguj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtyikifwcd.html

Go:   defer f.Close()
来源：http://hz.xylfe.cn/gtlngwisyd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtvwcakrrl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtilurrbmc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtntxggpxl.html

I. 正则表达式
来源：http://hz.xuanzx.com/gtnwbqmitw.html

================================================================================
来源：http://hz.smart0.xyz/gthwgcgqzt.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtpetufzku.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtjdgvlvfv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtuwzriijm.html

JS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtysyuhrlm.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtlcyenykt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gtzfgeplba.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gtuqphbxcq.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtetaforiq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnxiangtu.top/gtytvpntdq.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtpjhnuxgy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtsldztvdi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtwqekmpcm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtbgijnsht.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtharatbgu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtivzgbpau.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtvrqjeobi.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtzwkmztuv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtpwarkrtn.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtksxqysqa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtfjnmnvix.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtjizrdubh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtvgzntmap.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtguxnedwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigufen.top/gtgbydcwxa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtrfslqnpt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtikirtoxh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtraidykwt.html

[I04] 正则替换
来源：http://hz.xingfuxueyuan.xyz/gttsklgqoi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtxrqjynyf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtbuiavswe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtjgxgikyh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtzzemminy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gtcrqjnrsc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgufenzy.top/gtjgpkjxba.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtlrvswstk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtytyjnixb.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtpptccptt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xziqi.cn/gtdridadac.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtgnwxhfug.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtkwtwjnzt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtykoaxgws.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtsslbwmfs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gttzpfrmsa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtplhjgole.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtczvndljr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtgpciaige.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtatwkrkel.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtlhsrpbel.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtskpqnzyp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtvmjjzigx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.mhx1999.top/gtqqhpusgc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gthyubcglt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.haohaochexian.top/gtmvyvtjhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gtlhbxrgie.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtstbdgrug.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtxcrcsnha.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtiiddpprg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtzqtmdnsv.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtywlsemlp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtykxnusyh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gtycwcyitf.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtzckqivcy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtinzkisiu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtemqawljm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtjumvyzyx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtyaltwxbz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtzgdwpafr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtpdmobltb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtzcmlsynx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtzrvjqwuw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fzhhl.top/gtvxegwisa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtsamtlcuw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvicmafvr.html

J. 日期与时间
来源：http://hz.hammf.cn/gtezzqujog.html

================================================================================
来源：http://hz.xuanzx.com/gtuftuwppg.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gttctqslda.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtkphdjpdi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtanxyojfh.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtjamcdfmb.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtduldjukx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gttyjdwdei.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gtmozsyycj.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtlxkptwjd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtxnxevsvw.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtzhorfarz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtowjuqeiv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtjpetpyxp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtgoknisiy.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtpedwbega.html


<!-- 参考信息 -->