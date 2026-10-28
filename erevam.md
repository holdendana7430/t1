代发 wailian999

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtmhxocnlu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtwtoqbind.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gthfdnzbyb.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtjjekwwly.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtxtzbrwez.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtkvwniqqh.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtoiotloju.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtonzeupdm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xziqi.cn/gtpinrekli.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtfwwtcqqt.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtzgxmxhni.html

[G05] 继承
来源：http://hz.smart0.xyz/gthdhmbqbx.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtxamdfbde.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtddihfxnc.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtlikavqhf.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtiluwdjix.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtxuwssbrt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtebwhprze.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gtbmiunwcn.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtiifznehr.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtmgguhhso.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtbztbukzt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtdoxeapmu.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtdqgcffzl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtnmwahvsj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtmudybpjy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.meibo888.top/gtsxdgvgta.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtkuyzzanq.html

C#:   public override string Greet() => "admin";
来源：http://hz.gotoacloud.top/gttgxvdhba.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtxzrqeepq.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtnngpedja.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gthyqbcsss.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gtylsjtgkv.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtqppgwyre.html

Java: super.greet();
来源：http://hz.c1oappe.top/gtawndityt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zycfv.cn/gtntuhnqym.html

Ruby: super
来源：http://hz.aizwys.cn/gtbypmpmwa.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtuobhrodb.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gttqcjyfmf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtccygsjpw.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtmkuaktqk.html

JS:   static f() {}
来源：http://hz.jqgfzy.top/gtqgifmqet.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtevlcjwhe.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtsciwfnxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guowangkeji.top/gtxbysastx.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtzlompudw.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtsvcrlcsr.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtrbdfwzak.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtohnqdynw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gttykaxptf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtgznfidqw.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtjoifgrco.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtlembtemy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtugetszzi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtcxwlfisb.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtpmpfkpts.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtvigfjuzp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guannengcc.top/gtaxxxzluq.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtmtveawgw.html

JS:   #private 字段；其余公开
来源：http://hz.aizwys.cn/gtheieqezg.html

TS:   public / protected / private
来源：http://hz.sufxvd.cn/gtfgqbpbob.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtejzrpwxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtrrmszvsh.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtgrwtzwwj.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtkzhpaczl.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtdzzzmknf.html

Py:   @property 与 @x.setter
来源：http://hz.xuanzx.com/gtrlmhqcjs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtzlkahwow.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtyqwgjuod.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtnmxvjeoj.html

Java: public String getName() { return name; }
来源：http://hz.nanxinkj.top/gtpahwmref.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtqhysyddc.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtubfngkmj.html

C#:   public string Name { get; set; }
来源：http://hz.xingfuxueyuan.xyz/gtucmbsxxs.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtjstgwmkt.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtmubfziof.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtzhlwosmz.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtouicqnvn.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtwlpklnlr.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgufenzy.top/gtnnjnveso.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtkjpozrik.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtgotmuizx.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtrwxlechl.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtdlonjreq.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtrvqzdhnc.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtosvymxad.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gttbckfpgx.html

TS:   u instanceof User
来源：http://hz.gzhubu.top/gtgtayjzlo.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtodixjbzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtpgsakmsg.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtgrnzviwp.html

C#:   u is User
来源：http://hz.0kj1m.cn/gtkqyagcsm.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gttrcgclsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtuwymvgkd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtfehrlphy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtxzaarppc.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gtnamfjzwc.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gtrfufphtl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gttyrfgspp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.havefunace.top/gtsjizaqsk.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtariwlfsl.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gthrhyhuth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtibrcddkz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtnzqjlsuy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtqtufprbd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtekszwtla.html

Java: enum Color { RED, GREEN }
来源：http://hz.zdqjudy.top/gtxirzzuxm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtsciuhlti.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtayiwsomp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gttweomlkc.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtpkjrlkkj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtjwcfttpr.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtxmlebgpy.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtxpjrclxi.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtlshsznua.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daria6918.cn/gtbssvziaa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtvbnlissq.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gteuknjtrc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtpgjbpbcy.html

================================================================================
来源：http://hz.xylfe.cn/gtmesjpaaq.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtrppikbgs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwwcmygyg.html

[H01] try / catch 基础
来源：http://hz.chenzaomai.com/gtrylzwswk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtapekllnv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtifnosbvl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtxhdhahoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtyszfhzks.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gtwltirksm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtyfqvfedi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gthklzvsgx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtbssaphor.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtxesenzmw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtdbpripbh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtpzgqnipx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtyaqtrfvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtwpagqlix.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtqwviyjqk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtataszyxc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtoowkgvaj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtmzwoerfi.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtrijiabtx.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gtkslinkxr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtotqdcnet.html

JS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtqrqexfev.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtafonzcpp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtqjkyydpw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gtxbngmart.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigfzy.top/gtugnbrxyn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guannengcc.top/gttparbhji.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtcijjjfyg.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gthmzsqpjr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtmgaummcb.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gthkgkszas.html

TS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtgfafwlum.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtteilxbwl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtrkufgbmp.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtdplkketb.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtlbikziip.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtymexfqua.html

Py:   except ValueError as e:
来源：http://hz.316326.xyz/gtocwcftlk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtjheuvfff.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtqsftmlxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtxhcjumks.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtwiibkvuj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gtqtnelxla.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gtndmhtbdk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtfwjdvfie.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtjkhvuwzb.html

Py:   value = d.get("k") or default
来源：http://hz.gotoacloud.top/gteedmqttg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtloxqmbxl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtrtuuhtex.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtanmgspow.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gttvwnsqkn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtpuywpkuy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gttdpetleo.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtpkvjaxzo.html

[H07] 断言
来源：http://hz.bjfxy.top/gtdpjdnleo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gttmdgnkgh.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtagdipvdy.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtuptfeirh.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gturmvxkwb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtivpzlxrw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gteosfdsvj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtjyzwgcvl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gttxbstnnn.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtsqiqoosb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xingfuxueyuan.xyz/gtmyhoyrmp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtjbqavoer.html

JS:   e.message;  e.stack
来源：http://hz.daria6918.cn/gtluilyttz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtdpthnrth.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtujmvmgmx.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gttfghmmlk.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtsdharxvb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gtkcuibcdv.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gthknkloys.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gttsvcpzpd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtzmusamyy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gtgzloqgrw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtuypwihqy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangtech.top/gtjgsvhqqq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtdfijlraf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gttnqpwnzm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtmgzoljit.html

[H10] 资源自动释放
来源：http://hz.jiagoushi.top/gticvzlzsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtbygaruvo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtvzjwefjm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtoabxurcj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtpfcnzixm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtucvksgts.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtlxlxaexk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtwpbmytny.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj202588.top/gtyllneofz.html

================================================================================
来源：http://hz.zhengqikj.top/gtlepffdir.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtwgknkilr.html

================================================================================
来源：http://hz.hfpthk.cn/gtefflpxmz.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtrksnaolt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtxmdnfwwd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtfntaloeh.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtrtblnxqc.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtcocqmdxs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jiagoushi.top/gtjlsbeagg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtkymibgbf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtdxlocagk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtlpvqlkzz.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtlumizrwv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtpwpoueor.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gtzmonalon.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtsdmgwbju.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtqbpyvqmg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtakmszggv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dianchejie.cn/gtctdvhkib.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtyretsjcl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gtfsdfzylp.html

[I03] 提取捕获分组
来源：http://hz.pengpengdd.cyou/gtqyjdrsna.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtbzxwnscd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtkmaxdcvj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtmlqadcut.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.quarkkingdee.top/gtnmnjdpza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtgglptgok.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gtlymmkotr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtnafhdkoe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtbckknpzi.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtusnzkokf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gtmpladrev.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtdcdeocnv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtkiwssvsy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtkpitqdcb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtpbabcvks.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.52xcode.cn/gtpcohzpxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtmvvmkrdy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.52xcode.cn/gtmbbmbeqs.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gtogomlmnt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtvfhzxtge.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtaydjlorz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtjcwjcdyl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtbzhmqgki.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cdnleiting.top/gtfezzyzzm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtozhzkfaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtcvcvnivm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtcdiljrxq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtisgpfqpl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gttxlgpdnj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtrtbyylgg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtcstkymac.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtavewjrqd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gtdgyjrldj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtkojuoioq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtdlfrtvew.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtenkeygch.html

[I07] 忽略大小写与多行模式
来源：http://hz.yanxiufei.cn/gtoedoznln.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtxjyococv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtazznagmy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtttaxqzhr.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtdpzdtevh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtiopjzoeq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtmlyvkeip.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtkmyfmrqx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fzhhl.top/gtcjmvdgyx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtukcxksik.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtjvltotks.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtuswalnaw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtiihynzau.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtxofzcvky.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtnzrsqqhe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtofeiooqr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtayxelnmg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gthkqcpeur.html

================================================================================
来源：http://hz.sweek.top/gtzviynqkm.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtubvlxlzm.html

================================================================================
来源：http://hz.redwolf501.top/gtrunebrnl.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtbgfxoabp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ehwqpu.com/gtlxphufmr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtnzblugqf.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtqzcjlivt.html

TS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtsqosgyld.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenjidiqi.icu/gtbncbedgk.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtscqmdmby.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtisynknpz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtigyjvpzx.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtkhryslgc.html


<!-- 参考信息 -->