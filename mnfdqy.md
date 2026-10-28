代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtggtmejrb.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtcqizdsyx.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtjiewsugj.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gteosncpii.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtfbhiiuhd.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtsazqtbik.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtnliqdvgv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtbfrdpwsm.html

Ruby: @name = "x"
来源：http://hz.yj202588.top/gtbhaawqgk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gthwqqbcry.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtcuffzdym.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtfmwxrfpc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtbparzgej.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtexwtgmqe.html

TS:   greet(): string { return this.name; }
来源：http://hz.meibo888.top/gtxodkpivm.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtbwnoykql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtlgkggwdo.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtgsxsvtwo.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtiayokknk.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtgalkrmmj.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtfewrzqyu.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtsmsytods.html

JS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtleehgxgk.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtyrwazbqw.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtjjsdqetm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtuduiixmp.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtzkcwpinh.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtofscluag.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtzzpvdlvg.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gthxfnpapx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gttaxldbbj.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gttbtpihyk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtwokrjpja.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtnkxukmsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtugdlsobz.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gttpzawkzc.html

C#:   public override string Greet() => "admin";
来源：http://hz.cqqwz.cn/gtzefmnmet.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtzjbcjhxl.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtkhrsrezt.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtrayaiukn.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtuwtimyyo.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtadjrldxa.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtflqbuykr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pycfn.com/gttzsbfksp.html

Ruby: super
来源：http://hz.xinyue.icu/gthgbgelgf.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtjgzfyggh.html

[G08] 静态方法与属性
来源：http://hz.yj20258.top/gttktzlqey.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtftactqkl.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtqtzidleb.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtaknpwswi.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtxtkvqjoi.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtvgotmmdm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtplewlfkw.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gtmjyrspyi.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtzupbkucx.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtjjeyychf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtdmbgbbra.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtoxbzvlhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtltikdeon.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtsqmcnddk.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtuslqkujo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fzhhl.top/gtalpyqptf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtkhrjjhxz.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtbhyvmtcs.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtpdffhlgh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtowzgucrh.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtjpcokumv.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtnpktaeoo.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtvosesurh.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gtespmiukr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtamtojqkw.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtityehjnk.html

C#:   public / protected / private / internal
来源：http://hz.yuxming.cn/gtkioswehx.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtpexskgdm.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtqospecce.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtllpugrwd.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtrjzsawyx.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gtzaejspxd.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtkjznudjm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtdtgqlyyo.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtlbuwhhlg.html

C#:   public string Name { get; set; }
来源：http://hz.ppjwa.cn/gtrmkoxvxg.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gttxorilgc.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtjntawizu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtwpwhfmli.html

JS:   toString() { return this.name; }
来源：http://hz.hnqzz.top/gtuorhrzqh.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gtdyxpeabg.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtbhuuomhr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtmsedervn.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtacgnrrir.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtisoapzsp.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtqgostnsy.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtdqzvhflt.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtaxtgzbdn.html

JS:   u instanceof User
来源：http://hz.sweek.top/gtzbcjvloe.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtxqgkreii.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtewdlbwyr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhongyouzk.top/gtvkiqxdst.html

Ruby: u.is_a?(User)
来源：http://hz.yanxiufei.cn/gtgncznctc.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtphgqwmso.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtpspwkqsf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtxhryreqk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhengqikj.top/gtlcujbnxx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtdargogul.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtspcckdsg.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gthxyafpfp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtksvifjls.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtrxeucopv.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtfgmrgxvq.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gtzyppomrk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtuqkjweku.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtbitiexdd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gthprbtbvu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtbdhiajkz.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtujqdgbnz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtjensyakw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtdabguwqu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gttedylrhk.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtgvousuad.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ivvv.top/gtiiyvfens.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtogwqkxoi.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtflgjgjli.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gttvfncxol.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gteveplkyx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtumxskyjo.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtyqszugtm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtrjbcphzz.html

================================================================================
来源：http://hz.c1oappe.top/gtartufcac.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtwivejgqo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrutcjquj.html

[H01] try / catch 基础
来源：http://hz.xylfe.cn/gtdxwbtyot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtdwvggnal.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sweek.top/gtuqobsgwz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtpfwybmsa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtsjjfmfcy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtkggwvkux.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtxxzzcpyv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtuzryxvvy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtmougheru.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gthkvseerv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhiwuduotai.top/gtcclssyxz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtdutupuvu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtxlyjyoiq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtrvofsqlj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtezacpksd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtabassguk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtiadnufxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtspwptyje.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtkykqkghi.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtycchuexj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gthkzvdttu.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtwzvrwfhb.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtdobxzogq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtvcqwyjuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtchsdpmbl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtidhxwaiz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtxnrlhgdi.html

[H04] 自定义异常类型
来源：http://hz.quarkkingdee.top/gtcdjovrud.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gtolsbkxof.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gthgpxmhau.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtkzrxcagh.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtxjhsxsij.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtioxvufkw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtqqekzkdi.html

Ruby: class MyError < StandardError; end
来源：http://hz.shzxlz.cn/gtiasxdsnw.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtkdnemeox.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtvdrhbawc.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtbftkbiaf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtpvpgkbla.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtkjuuzcaa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtpkvqmmnr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ywan-chungtsiang.top/gtbdxaamjo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtyqiuubtj.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtrayjlpzq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtzoocbkxo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtqqblroje.html

Py:   value = d.get("k") or default
来源：http://hz.smart0.xyz/gteltbgusz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtshmljzxo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtehdqvtyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhixingplan.top/gtinaehooq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtnrjydayq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtefzaqtox.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtrznxzwlt.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtwfyvwgmw.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtnubcpomc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtcdavixqv.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtsrsawtym.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtbwonwfle.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtamvsjnsn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gtjgfcqmaz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtqinzaehj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtzzeibfrn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtfwhljshr.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtmddvnurr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daxiang520.top/gtjqgjgudf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gthxbkcilk.html

JS:   e.message;  e.stack
来源：http://hz.gaohongyu789.top/gtmklkkgip.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtcjlvznxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtchkhcwbf.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtjltxotgt.html

Ruby: e.message;  e.backtrace
来源：http://hz.hammf.cn/gtviwicigd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pengpengdd.cyou/gtecmerrxx.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gtdxpiogcm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtiuflljxr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtfmmzydro.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhixingplan.top/gtimjqnixr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtzarzfloq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ppjwa.cn/gtbozhtsgq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtjmxrxqud.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gtvfxmwghe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtesecydcq.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gtsvsntpmv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtzoivnprg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtrpurvihh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtgrzmbiul.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtzbbqsnbk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtysialfsh.html

Go:   defer f.Close()
来源：http://hz.svipenyu.cn/gtzgjrpzcu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.316326.xyz/gtnpumfmsa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jyoumei.cn/gtlpljooze.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqelvvnej.html

I. 正则表达式
来源：http://hz.yonumen.top/gtbtevnvjj.html

================================================================================
来源：http://hz.svipenyu.cn/gtdwuxuznw.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtotmkikpu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenzaomai.com/gtkwqmscdc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtfrqzxpuy.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gthfwvxycf.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtkvfzkdrl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gthtiwccpm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtwdcjnbzj.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtwampcdff.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtnvbqpruu.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtfrsxvrlg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gteiyejqwa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnqzz.top/gtssuzekzy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gtnynksxqh.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtbfqowuwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fengsongda.top/gtcowbijde.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gthbhiugug.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtrihzxvaf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtjcghzouu.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtgkypbzyp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtpgukelfx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtpcvcfahi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtcpfcjzvr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtvzlkszpl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gtiihkitvc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ivvv.top/gtzywfnrod.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtevzeysdq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtffhfedcv.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtrokxewvl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtnnuoqwjr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gtldupewus.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtnbypxpkw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtfkardmlj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtazwwfldh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtflbjnlll.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gtjmcuwksk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtmwhjinga.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtecmgyqxp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtsgzxjtvs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtiduhxyfk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtcihzmocc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gttxwhtfsh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtqynejfqs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtpucmdsxo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtxwnhorfy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtgkennzay.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenzaomai.com/gtoiyocqyb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtryazgjob.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gthgclqmnw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtrgumhjib.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtntqpfekq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtdtomasxr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtvzvebjjs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtatdrmaad.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtzojixaeu.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtozixhiim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtwrlzbuug.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gtokmgdqfo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtpaboqlab.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtoqnavwau.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuxming.cn/gtxpesycgi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtysnxfnor.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtbtrshpok.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtdggnfonc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tian-w.cn/gtuxbpwyuf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtfmtbsoxo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtgamwwibc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtdeemfahy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtoqoyyipx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtgbxbnyns.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gttgelqwna.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gtztxscyqy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtcxccuqgs.html

================================================================================
来源：http://hz.tianlin.xyz/gtvnfcvfej.html

J. 日期与时间
来源：http://hz.tanke756.top/gtrmkqhozp.html

================================================================================
来源：http://hz.guannengcc.top/gtzqpdlupx.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtnbarpmto.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgfzy.top/gtvzezudoj.html


<!-- 参考信息 -->