代发 wailian999

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtprbyxlcz.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtikkvcrrn.html

Java: private String name;
来源：http://hz.yueranfly.top/gtjwhartgc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gtnesgvhug.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gthjcutsko.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gterfmghzb.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtxzmqzhxw.html

Py:   def greet(self): return self.name
来源：http://hz.daria6918.cn/gtoyrkhfnt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtfwllbhwh.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtmmlxxedh.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gthnggugff.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtqbvarcwm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gttrrfrygg.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtvcghftqs.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtmnxecqay.html

[G05] 继承
来源：http://hz.yongpay.top/gtanxgehxr.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtkboabayy.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gtoqrbqdpn.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtqvpmjjle.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtvuhixuib.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtkgrxjjdb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtkebeephv.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtpwvrjsbs.html

C#:   class Admin : User {}
来源：http://hz.wangshuangyany.cn/gtjmqdojvi.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtlygojfqx.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtxlghsalh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtemeteztz.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtnrpygehy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtwdnjuptj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtxnquedee.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtbcdabhfu.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtouuwrbdq.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtgpqkpodh.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtuwwdlvhh.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtgictemvk.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtphapyats.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtsymfpkag.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtglveebll.html

Java: super.greet();
来源：http://hz.sweek.top/gtfajcojob.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtvzniriok.html

Ruby: super
来源：http://hz.andypj.xyz/gtiqkjyyzg.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtphufuagf.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtgyukussa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtxnewoqps.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtnesgqbhy.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtnomflkei.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtrbbglhtc.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtntzyervx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtgboxoeky.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtrfqnlkvd.html

C#:   public static void F() {}
来源：http://hz.mhx1999.top/gtbhxaaclu.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtdtbhwnux.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtkwwmmiis.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtrlssjiuj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yongpay.top/gtqbrkeblc.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtxiamwuvp.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gtiavhidix.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtuwkrlfsm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtoefzfoub.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtggqnmitf.html

[G10] 访问控制
来源：http://hz.birdmap.top/gtrctobagr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtagbufkhp.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtpdxuqlam.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gtbdejkajy.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtgiuzfkud.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtxzdnscna.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gttjbixqgb.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtooanihaw.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtzmdrtguu.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtcgrufmhk.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtfzoolugq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gthgccjpet.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtypkazkrg.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtssyjxnnz.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtcfdsuxdb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtwfaqedtl.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gtraivktjk.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtzqdunyxs.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtyuxbujbw.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtymffplnb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtoerjsrwj.html

JS:   toString() { return this.name; }
来源：http://hz.smart0.xyz/gtnvtreepr.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtztaxihhb.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtnxjsenne.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yvedp.cn/gtpsoscbpk.html

Ruby: def to_s; @name; end
来源：http://hz.iojbl.cn/gtgvncldjj.html

C#:   public override string ToString() => Name;
来源：http://hz.hnxiangtu.top/gtkmbsryxd.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtbdobdvlj.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gttwdpddmy.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gtywwtwwfz.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtywfppeqh.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtsdwbplhz.html

Java: u instanceof User
来源：http://hz.quarkkingdee.top/gtznuwcdie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtwjcldorh.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtpduiiodu.html

C#:   u is User
来源：http://hz.9152youxi.cn/gthdhbliya.html

[G14] 数据类 / record
来源：http://hz.aibaodan.cn/gtzthklhnj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nwbrower.top/gtooltlurp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258888.top/gturkjuama.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtdjqmnpcu.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gtqtfevibv.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gttljfdfik.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gtpirgeulg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtuiptyvwe.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtnmfggzrk.html

[G15] 枚举
来源：http://hz.shzxlz.cn/gtmuljiatc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtzgknmbfs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtsbucihhm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtzlwuckym.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtxeqwympv.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtszjcqkjh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtozfkzwfn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtfufjgqxs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtswrtjoun.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtbzcdebph.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gtsokpzngi.html

PHP:  get_object_vars($obj);
来源：http://hz.dashuyun.cn/gtgyxvhefh.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtsqsphcgt.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtwxqckvnu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtwddgrokz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtemaffpjc.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtxgexskea.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.birdmap.top/gtwntwuxks.html

================================================================================
来源：http://hz.yuanzhike.top/gtvscvpufl.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtvtpososq.html

================================================================================
来源：http://hz.sysykeji.top/gtqrthmjcq.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtduoafwbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtwqtxpnwc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtmbdyiyds.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtkeszauzv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtlbiqjezb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.mhx1999.top/gtonrhjckk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gtphwsyvte.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gtvqglameb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtflokdrgn.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gthzshvsey.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtkpayitwx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtzwimzhpv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtbytesfcj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gthudcfduf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtkzlxhjaw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtnivqcven.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.0kj1m.cn/gtjhgmjwue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtszrttqus.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtdqeetfrc.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtnuqynhhz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtbubzxajn.html

JS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtkznkwblp.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtxypnxmhg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtiazidcil.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gturzsakif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtcubfmsda.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gttbxvquvj.html

[H04] 自定义异常类型
来源：http://hz.yuanzhike.top/gtilesrzre.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtcwhwzngs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtfwzucyzb.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtmklupqpm.html

TS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtfqjgfgry.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtlhbxzyyq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtptfnrvsx.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtrcxdoezy.html

C#:   class MyException : Exception {}
来源：http://hz.gaohongyu789.top/gtzslkwumk.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtefnbbdmm.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtxvvqnljl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtxrsnmtky.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gttgsqaeea.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtgplkbmrl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtkbiuiqzd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gthfccryzo.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtvnkkdoll.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtuomwjuip.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtabpqqjbp.html

Py:   value = d.get("k") or default
来源：http://hz.zhixingplan.top/gtcalfvdsi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtqqsbktzz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtjfbjfiug.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtjxgqdxzk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtvrxugbzs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gttkafidfp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtxcyhaxhs.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtdpnqyibz.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtaztgsyrm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtyigrwytz.html

PHP:  assert($x > 0);
来源：http://hz.andypj.xyz/gtigjkwizh.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtavpuptmb.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtrnifxqfi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtvyztcbeo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtjarsaovh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ivvv.top/gtpwjwpiwf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gteltbsguo.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtwpwcixpt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuanzhike.top/gtpfbnstjx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dianchejie.cn/gtgmmpxmgf.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gthivrmfiz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtzfomncpw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gtqhcyqhrp.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtzokyxqev.html

Ruby: e.message;  e.backtrace
来源：http://hz.xylfe.cn/gttlajwexw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtltldntgm.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtlidtantc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtvwontiaa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtkuqcdhsl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtpjxxpeoi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtocxypsou.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtgkytjads.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtyudpnssh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinghuilouyu.cn/gtsdjohgtp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtufzqhvlf.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtnnsiizvk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtzyrqakpp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtekaajgxk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtkvqlakdr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtcwwwlmtv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guannengcc.top/gtsjufxcme.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtivizmzoz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtlhysdegh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlukpjvrv.html

================================================================================
来源：http://hz.fengsongda.top/gtmgcfmpzf.html

I. 正则表达式
来源：http://hz.yongpay.top/gtyxdgelkj.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtupnwdpzg.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtqocedvvs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtrfwgeyac.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtchjgbnho.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtoozubokf.html

TS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtyjzzxojk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtkivvjdjq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtwaiirajj.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtvxguixlx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtjjgvvert.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtdkddofdr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gticfyikdg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtyznipwsm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hfpthk.cn/gtdlsjmjqk.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtcvbudblm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gthdyrufdk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtxkcacsms.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtglzbbdrk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtfjfhcbtp.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtrgztzxiq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtywetpcyr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtcybrudiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aibaodan.cn/gtywuzwcmd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pycfn.com/gtusnnhugf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gthoybnjjz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gtqncztypf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtcnurfixl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fzhhl.top/gtnetrszzk.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtilybwite.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtnzpvhnmq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtrvraxrtf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtqsybgzly.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtfbkrtyrt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtpjqyjugh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtigqxoumr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gtgwesadze.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtqaesditg.html

[I05] 按正则拆分
来源：http://hz.iojbl.cn/gtzjmdrfjj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtycuautzn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtddiyakqp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtpwgbabvu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtikbfwpyc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtwuvmipje.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ehwqpu.com/gtuyizzpfu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtznnsuujn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtfeaffknh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtlsxqstgs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtrkgfbhkc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xziqi.cn/gtrvrqlmxd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtnyeoosoz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gthsxxwceu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gtuvqinoxr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtlveujdcn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nwbrower.top/gtxhtexkwe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtgumfcmhz.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtqixrqhns.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtadyusaev.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtozumujuw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtjnyhxopm.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtzbytogfi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtgalrsomr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtwryokxxq.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtltywqfbu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtkdfirxvc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtomhopgsb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtlgjybyjm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtbjodioux.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtojwsnegp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtxjudivnb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtufoaltzy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtvpgvoueh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtusspsjhc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtwnjukkdx.html

================================================================================
来源：http://hz.guowangkeji.top/gtlymhkylf.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtvazilxsb.html

================================================================================
来源：http://hz.fengsongda.top/gtxvrbrakz.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtkufyybdf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgufenzy.top/gtcfxptgta.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtswgbpyzd.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtwqjrqjay.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtlgdsjnnc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.quarkkingdee.top/gtmzjbmyon.html


<!-- 参考信息 -->