代发 wailian999

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtavgawfsk.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gthweclwwf.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtcperxoqf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtpcodosnd.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtnrkcdzuj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtvnxakaap.html

[G04] 定义方法
来源：http://hz.zycfv.cn/gtivudiksq.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gthhognvob.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtklrjdwul.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gtvhhtevgt.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtziqwzfkk.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtmcpdamci.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigfzy.top/gthyvjpjik.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtmquybywv.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtrigtcmko.html

[G05] 继承
来源：http://hz.xylfe.cn/gtbjiwcprj.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtqmixrjnz.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtmyezifku.html

JS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtbpreyixk.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtuyaqvfbx.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtlrytofab.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtigdwdpnq.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gthjghwwae.html

C#:   class Admin : User {}
来源：http://hz.vqdsnc.cn/gtbklwcfhl.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtrbtapdfz.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtnbrzwwlg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtyosqqeyp.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtlpycango.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtzxkzsryw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtwqftznbw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.meibo888.top/gtxbbpzkll.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtnnughzyp.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtoncatkjy.html

[G07] 调用父类方法
来源：http://hz.sysykeji.top/gtgwsvssok.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtplbtnhqj.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtqhbrxruc.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtvkzynwsk.html

TS:   super.greet();
来源：http://hz.yj20258.top/gtmcieemot.html

Java: super.greet();
来源：http://hz.cheryme.top/gtsujrwyrb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gthvwajtrf.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtoesjszdw.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtpzsdyipl.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtycxssmyn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtupuzbtbj.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtiilbkcao.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtpybqvjlx.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtdamuyjyz.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtbhjztqzt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gotoacloud.top/gtsclrcbsw.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtnwqeeqrv.html

C#:   public static void F() {}
来源：http://hz.nanxuanxn.top/gtyqttvprd.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtqicgzndq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtciwayypt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtgjumiijz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gtfkimkykf.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj202588.top/gtufnnzpsy.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtpktloxeh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gthyrsoxjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgfzy.top/gtsbslcmkh.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtdfgftaqc.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtlhscuelz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtzvmiorbq.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtzevyivji.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtzjvikyva.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtmqcimlpi.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gtzvuppbcr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yangfankeji.com/gtqqpukciv.html

Ruby: public / protected / private
来源：http://hz.zhijiandao.cn/gtwfwvpxtd.html

C#:   public / protected / private / internal
来源：http://hz.tanke756.top/gtmfaplxzd.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtfqkoghiv.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtotkbvlyi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtcaitczil.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtrcskdjos.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuetiantiany.cn/gtcyqpmhhg.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtketnxhdp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtxtuvzucq.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gteowgiqfl.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtcisprdeb.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtzbnptxod.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtlshubyul.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtnvuyrgza.html

JS:   toString() { return this.name; }
来源：http://hz.52xcode.cn/gtzohcejjo.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtuzmtmzqa.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtorktgdfy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtnjqwrndx.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtlugwkyot.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gthelrmpmy.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gthbhhaayi.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtpxrrferd.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtravwjwik.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtcmgvjgik.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtozjyzcln.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gttguehhqy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gtjrbtwmkx.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtjwksojbl.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtqcnbeumy.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtajgcrrrz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtunuejqhl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtofdatvjb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtksyjedga.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtxsdgxrrv.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtynfpurae.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtaizutkbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtaxjaifro.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtbfdhbbbg.html

[G15] 枚举
来源：http://hz.meibo888.top/gtxgpoebjo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtqwvfhvyh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xziqi.cn/gtgoixfvqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gteojsjxzd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtyurnwnii.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtbjubngqt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtelopfctz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtpgbyakta.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtmiwgrpxl.html

[G16] 对象转数组 / 字典
来源：http://hz.zhijiandao.cn/gtkgvwvyty.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.vqdsnc.cn/gtxikuwrpp.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtxprkhcgn.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtgxelmuat.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtdpbguleb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtojrkivyf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gttblcxfnq.html

Ruby: obj.instance_variables
来源：http://hz.yuxming.cn/gtcoqnvkxu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258.top/gtghpggmcm.html

================================================================================
来源：http://hz.yj20258888.top/gtfzwhwygg.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtxvpjmbrg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwmdfgikm.html

[H01] try / catch 基础
来源：http://hz.chenlongwang.top/gtfbcdgcxm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtmuxvfxsp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtewqnvflq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gteltofnar.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtzvlqxsxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtuuwvqzpi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtwzfxlscr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtqslxlkxg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtgrznazdj.html

[H02] finally / ensure 收尾
来源：http://hz.kuanghao11.cn/gtepswndmr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtxqlovfyb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtxudfymdp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtyesuxerp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtbwbziyal.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtikthltyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gthknrseqy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtmojsucyn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sweek.top/gtbdlybvnh.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtunduxboh.html

Py:   raise ValueError("错误信息")
来源：http://hz.feifeiyinyue.top/gtvdwtaeut.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtkwgghnvc.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtcwwgirlb.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gttcspjwoa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtoircfocc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtevjlhsby.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtbtpxoxyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtbrqowrsd.html

[H04] 自定义异常类型
来源：http://hz.wangdashe.top/gtmtizsqqq.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtpzmuqzdv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtxpcujyjp.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtsvuohool.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtujvcmnqu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daxiang520.top/gtpkmqhjil.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gttzictzqj.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gtnvlccwdf.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gtnhkiluxf.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangtech.top/gtsrlfscyk.html

Py:   except ValueError as e:
来源：http://hz.quarkkingdee.top/gtidqytusz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtnqwedijl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gthwvbpnww.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtwohymiac.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtssqlcaxv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gttrqnlaso.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gtrwyamabd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtstmqmdya.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtzvjgpgji.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtjjyturyw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtvkcujiec.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtnillxbls.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtrjzhfirl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtqrnryvlk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gteygsyhqx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtrqfhdvif.html

C#:   obj?.A?.B ?? default
来源：http://hz.xylfe.cn/gtbpyedeaq.html

[H07] 断言
来源：http://hz.52xcode.cn/gtyrflyvdo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtnppgumvm.html

PHP:  assert($x > 0);
来源：http://hz.tanke756.top/gtkbfrnwfh.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtpgzbzlge.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtyausawai.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtmefvzutl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtborgqikz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gtssytjtpm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtikhltber.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtpaezeaxm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtlpnfnvgq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtpetragto.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtkhrevpsj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtzlhbyakz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtmhfwxejo.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtwlchrnas.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gttvfkghxy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtgyatzgdz.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtgxowvaow.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtovfheuey.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gtvysvbgpk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtqdmzpteh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gthrgesepe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gttzdgsvdw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtemwydnvw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtfetarqza.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuanzx.com/gtmgznjamb.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtajvrksil.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtuyxdtsvz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtqylojybe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtnnancdby.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtovsrvltg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtsofufovz.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtuspguxrp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtpttagmut.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtvqhkpasp.html

================================================================================
来源：http://hz.snrcjt.cn/gtutugaytm.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtdalwxbic.html

================================================================================
来源：http://hz.hnqzz.top/gtygrqnwzt.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtzlubyhxd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtiqwtfwuz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gtwkqibrnb.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gthaeyxmky.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtigrvvpgu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtnrrjducg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gtmxyondse.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtitgscbxh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtcxwimjly.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtjtnmrkbc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtqstzrvuk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtnmkuqymc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtbmorsbar.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtsfgocell.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dashuyun.cn/gtgukelnru.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jiagoushi.top/gtokiospft.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtbabwndjw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtcsixpkjl.html

[I03] 提取捕获分组
来源：http://hz.nwbrower.top/gtxpsliijv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gtaxnbtzmq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtvzlgjuwc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtnoxftwwt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.smart0.xyz/gthupvjemw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtayzoiwsr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtrohykctg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtnaqjmehm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtvyqkjvbv.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtfulinymc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gttxkupjdb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtozugglrl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtaakvmgzk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtcojszfkw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtfvwaskzb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtpofjpiif.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gtrzuvtfkq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtzbjcwsfz.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtkofywtdg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtzzvxmrhg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtyhjsqimh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtqhyzarce.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtjyvjmjau.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gtujjvydbb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtbeyvlkpu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtamkvbebx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtnqvqamhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtroafyvox.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gttjtlmgrn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtvydhsiyt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtapeiaguj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtmbktbenm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.feifeiyinyue.top/gtphdpksap.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtrkwrdyrk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtfveorcbd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gttapfnybq.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtxnxltvfm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtncywwjnr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.feifeiyinyue.top/gtumqxghhq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtehnbwxoe.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtnepldqox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gthgocpsdx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtobassctv.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtcabzbflz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtldcnsabn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtuvnjukyw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtkpeenlgj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtkiiwndzo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtycxvelew.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtcseckpqq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtgsdsqcnm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtofqcjtvc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtlvgjlcjk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnqzz.top/gtunbkbleu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtskrsnzus.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtvfxsljff.html

================================================================================
来源：http://hz.c1oappe.top/gtomebxhsy.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gttfixgiap.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtxnuoicuy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtynxevgtt.html

JS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtucqhatvc.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gttiknhzxl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtulrxwega.html


<!-- 参考信息 -->