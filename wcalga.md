代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.hnxiangtu.top/gtksfcmpho.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gthedrqkly.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gthhkngtdr.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtpcwmycee.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtficfxoli.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtqcppqkmp.html

Java: private String name;
来源：http://hz.gzhubu.top/gtpzoqrrrl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtqyfnllvg.html

Ruby: @name = "x"
来源：http://hz.nanxuanxn.top/gtmnekpgql.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtemtxauso.html

[G04] 定义方法
来源：http://hz.jlsjyb.cn/gtkdijofeo.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtcyoxukyi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtyitnvlne.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtyhtlwafj.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtoqhcnibm.html

Java: String greet() { return name; }
来源：http://hz.zhengqikj.top/gtwftmshzz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtcqjwuzdh.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtjslfpguc.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtrlfgisje.html

[G05] 继承
来源：http://hz.daxiang520.top/gtqlkmvvdf.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtkssxdigb.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gtdbxvkijt.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtqhtiywzw.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtykkfadcu.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtaspcfilo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yanxiufei.cn/gtcgxorbmu.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gtpuxwytth.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtyugipuhg.html

[G06] 重写方法
来源：http://hz.shanyushiyangkeji.top/gtqenorkub.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtysywoknb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtrrttxzzi.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtyfaenbuy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtajawmfcd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtytoitrde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtvibitnym.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtefxpitsq.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtogeymcqv.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtcisbvhts.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtponcanaj.html

PHP:  parent::greet();
来源：http://hz.iojbl.cn/gtylbzdazj.html

JS:   super.greet();
来源：http://hz.sweek.top/gtxdrysyvp.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gtulszolgr.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtlorubrre.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtgrdtapki.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gtksxbvclg.html

C#:   base.Greet();
来源：http://hz.daria6918.cn/gthsqbzvko.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtcppyhuot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhijiandao.cn/gtrreagrks.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtkhyiqwxm.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gthrcmwrcp.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtcmlcehzc.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtwqvzgqzh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtmgnkapos.html

Ruby: def self.f; end
来源：http://hz.redwolf501.top/gtqjjxejfo.html

C#:   public static void F() {}
来源：http://hz.feifeiyinyue.top/gtdxpoljst.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gticuuxutu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guannengcc.top/gteelnzgdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gttxoknvpt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtctllzahl.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtwrwpsywt.html

Java: interface Shape { double area(); }
来源：http://hz.vqdsnc.cn/gtvichvtwt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gtjcgmqdyv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtrdgzqynd.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtmikoyvyy.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtesejuqjf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtyhqjrnhv.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtwjlafudc.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtigajjgvl.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtfdtlibsv.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtiftwkrpn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gttwormsrh.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtydfswpex.html

C#:   public / protected / private / internal
来源：http://hz.snrcjt.cn/gtmewvpozt.html

[G11] getter / setter
来源：http://hz.pycfn.com/gtkbzsvrok.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtsuiawbvm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtyiwywege.html

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtdrpgccor.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtrscidyvd.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtnuaihanb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtxwsofmfl.html

Ruby: attr_accessor :name
来源：http://hz.dashuyun.cn/gtryiklrje.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtomfzpghp.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtsaiuhkts.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtqirehaus.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtrkbfqsgu.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtfdmbboqz.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtfqpviknd.html

Java: @Override public String toString() { return name; }
来源：http://hz.tianlin.xyz/gtmgwzpgep.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gtjjcnjuvc.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtkxkwneac.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gtbrfsqijz.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtxspijgfq.html

Py:   isinstance(u, User)
来源：http://hz.pycfn.com/gtwfxnvwyq.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gtisfbmjvi.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtklxymfmg.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtsxcimmcs.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtltivgnek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtkppcwfrx.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangtech.top/gtalhksook.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtzsqszuup.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtpfihkvmu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gtfbimsxbn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtrojyvhlf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtnzcbbalu.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtrkbmpkcp.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtkyuxtspm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtwmmylqdd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.havefunace.top/gtweulsvwo.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258888.top/gtwyxqkbyo.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtbdaihchq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtojodrrhk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtzqrdxnzi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtpdngbqxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtlaodlane.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gttfxpgtjo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tian-w.cn/gtohphxupo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenzaomai.com/gtrrziinsv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtjmdwbces.html

[G16] 对象转数组 / 字典
来源：http://hz.zhoulong.xyz/gtdstbagfb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtphziiuqy.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtxqixnsdk.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtnogzozfc.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtzjgsykcx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtrpsynkeg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gthzyrjehi.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtzmnxlikt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtwalnaeee.html

================================================================================
来源：http://hz.yonumen.top/gtxmszlzoh.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtyenullcv.html

================================================================================
来源：http://hz.yj20258888.top/gtareztakb.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtlkoxkxxu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.smart0.xyz/gtvouwubyw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtaojeafiz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtoiswpxnh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtvahbcjnj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gtythjpbti.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtxxdtvszi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtrmqwnuzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtfliiykyf.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtummbmuir.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhaomingkeji.xyz/gtldschdow.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtsivsdwac.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtcynhbmqb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtzfypgupd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtzroksegk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtozigtlsc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gteqggfpee.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtctkwqjuw.html

[H03] 主动抛出异常
来源：http://hz.zhengqikj.top/gthvlaxshr.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gtdxydoaok.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtayzttyux.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtmhlivbtz.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtaiemspyr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtbxulegcn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtnexaaqym.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtgnccartm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtnvyeosoh.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtzoebtsjg.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtievpynbx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtewgtuziy.html

JS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtizztqxjv.html

TS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtzjrmaxxi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtqdcxkftp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gthixzqdhe.html

Ruby: class MyError < StandardError; end
来源：http://hz.nwbrower.top/gtppvbycug.html

C#:   class MyException : Exception {}
来源：http://hz.hysaishi.cn/gtsccoqpwh.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtxdszkxwl.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtnqeyzvju.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtjqvapvtm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gthomdetgw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtzapwtcuu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gttaushewg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cucudq.cn/gtpcnttdfu.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gtyxnycfzd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shangyingyoupin.top/gtyiidzbow.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtcwznsvbu.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gtdcvbroxi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtkquomsmq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtcdampwlv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtbwvttyab.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtmnexchqc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtgduzxhvx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtzsuwlgcc.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtvatvumqh.html

[H07] 断言
来源：http://hz.redwolf501.top/gtlivhgutb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pengpengdd.cyou/gtuclfcvpq.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtpwbxjhzp.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtfmbethrl.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtidwquyxh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtgopabbfh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtitwssuea.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.snrcjt.cn/gtyoibgfdh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtnweyumrv.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtulrtgzxt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtvfxaogcb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtycltrxbw.html

JS:   e.message;  e.stack
来源：http://hz.hnqzz.top/gthwughuui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sysykeji.top/gtwpweidbl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtkncsfdbr.html

Go:   err.Error()
来源：http://hz.zhoulong.xyz/gtfxnoamgi.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtthknykux.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gtxufktthh.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtvppdovpr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtnlvpiqon.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtxrspszgl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtisnalmcj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gthrvjexvl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtlqcyhgqk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenlongwang.top/gtgsuisefi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gtuutauxnj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtctcehvtf.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gttywklxao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtosqwimnf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtbimrhitz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtqupyxacd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtztybqpie.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtebgocjuz.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtahuixdrb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gaohongyu789.top/gttuuyhztu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtcqplnczl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgkkhdbgx.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtvyyzdbev.html

================================================================================
来源：http://hz.316326.xyz/gtxbnmvzzh.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtuvkhxirk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gthnksqaiq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gtmtcxpjrp.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtqkcqhuac.html

TS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtrgzexeso.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtppyckmmh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtlmxfqtmu.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhixingplan.top/gtrjazyvti.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtyivtuikn.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gtpcwvcbge.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtpfcwewcs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtcjagpmzn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtalrjzcie.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gteszfipnn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtylqmdgsw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtsvdnaykf.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtuuqzhcua.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtzqfupkdj.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtnxvmzsny.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtzwqdghlr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtcglkijdi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtkajoeiii.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gthnaxuqnz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtxszrmjwn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnqzz.top/gtpvigoqgx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pengpengdd.cyou/gtydqftvez.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gttunhruoj.html

[I04] 正则替换
来源：http://hz.pycfn.com/gttoaniezm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtuborucey.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtwjaeuror.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtxbtlboaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtwyrgbdpv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtraqbetzo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.iojbl.cn/gtxlamlgad.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gttuxjfxal.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtvwpzgdyl.html

[I05] 按正则拆分
来源：http://hz.gaohongyu789.top/gtnkdpigmb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtpqnidtof.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gttvskzaqq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtbllcfxxa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtauiebiux.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtysecczgb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtoetsvbqh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtaypazwkc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gttwgvlvps.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtzkowxqmh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtafcjihrc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtjzlufibh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtepijlzsv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtoqonctre.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtjnedodxt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtzuplntcq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtsaubumjx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtlgcfbxls.html

[I07] 忽略大小写与多行模式
来源：http://hz.gogol.net.cn/gtealfueth.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtttnnqqqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtwajeknhn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtzietivga.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtthcdigfw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuanzhike.top/gtkrtigjit.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtkrugqcnb.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtzhsbrnpl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gtcgpipsqf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtaafmmygx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtjrhvfqgh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtohusbnoq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtvxcormxt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gthggqtllt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtavqkgphg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gtxqogxtrr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtbuwjnmof.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gttnvcwccw.html

================================================================================
来源：http://hz.pycfn.com/gtqshzhhtv.html

J. 日期与时间
来源：http://hz.cucudq.cn/gtrgurkiwb.html

================================================================================
来源：http://hz.yuanzhike.top/gtbrgkxgyl.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtmzoxtvso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtnhjumeey.html


<!-- 参考信息 -->