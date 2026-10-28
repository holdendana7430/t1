代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gthbczhtjr.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtackgbaos.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtncwhnfjp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtrtmrfzlq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtjokweihy.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtfqirmfjp.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtmxkzvlsu.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtbxhjluga.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtplkczqic.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtnlepgcts.html

Java: private String name;
来源：http://hz.316326.xyz/gtbitkutnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhongyouzk.top/gtfbavyzzd.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtbpzyvvzh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtwldaekci.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtpdvdfzln.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtccwnlmfl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtfeudosxz.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtqfcdzemz.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtczlzgryd.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtisxlpmsh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtgrvkfwwj.html

Ruby: def greet; @name; end
来源：http://hz.chenzaomai.com/gtwjmuamth.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gtssxiltos.html

[G05] 继承
来源：http://hz.jqgufenzy.top/gtszyzzvcg.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gtbsvfimxi.html

PHP:  class Admin extends User {}
来源：http://hz.pycfn.com/gtnpnxgojh.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtshuerzzm.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtfepofvuh.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gttnmcqtdu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtnwweuzka.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtfucrbabu.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtlrdqpqbn.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtmziktovq.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gttpyrcdgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtdmjbczai.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtqxharenl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtkgjqkzav.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtagsquyna.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtgjmkmkio.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtpzlfgtmo.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtwncfnqdf.html

[G07] 调用父类方法
来源：http://hz.yuanzhike.top/gtqwbzdtuf.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtofjbgqpd.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gttalbbihd.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtobxmhuzs.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gtxvcpjjes.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtcwgfwjwc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtyatikbfh.html

Ruby: super
来源：http://hz.jlsjyb.cn/gtxvezkppf.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtzxrprhqq.html

[G08] 静态方法与属性
来源：http://hz.shangyingyoupin.top/gtzfjzkpqm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gtmhlxenjp.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtosjloaoz.html

JS:   static f() {}
来源：http://hz.jiagoushi.top/gtmquuaupi.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtzpbkxpzv.html

Java: static void f() {}
来源：http://hz.fzhhl.top/gtfpwhffrt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangdashe.top/gtuqnzzwkm.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtwssmgkdd.html

C#:   public static void F() {}
来源：http://hz.yvedp.cn/gtjhptpnwd.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtqzrlypje.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jianghu66.top/gtdmehuxcp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtstxiqdkx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtgqpkmclt.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtfvngugiy.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtmxoutbru.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.birdmap.top/gtrwrytniq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ywan-chungtsiang.top/gtcuyfmkee.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtgkxtdzoh.html

[G10] 访问控制
来源：http://hz.ehwqpu.com/gtwstqcgwb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtkhyitogr.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtazwnwska.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtooklmtbu.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtvnithzzl.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtrqtgnkwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtujyqtcuz.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gttottpuju.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtsmjysudm.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtylgsfqqe.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtczrbtdnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtculuotft.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtpqhckqdj.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtrhsziirg.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtgnevkcyp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtaudwwzya.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtkcyommbz.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtqwicnlvo.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtfcskrpoe.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtkekvswxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtgykgxcmq.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtoldunygu.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtshwzlkhq.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtpmhkxude.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtoozebksn.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gteolnviyb.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtidiaegwq.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtqeystudw.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtnkblpdls.html

PHP:  $u instanceof User
来源：http://hz.snrcjt.cn/gtubrfupny.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtmknciayr.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtpuswuwml.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtmpqduovg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtgqlyilnj.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtmotzahqv.html

C#:   u is User
来源：http://hz.nanxinkj.top/gtygcestph.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtcoqvcxrj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.mhx1999.top/gthqouonlw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtohjhqhfm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtjoutiuiq.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinyuanbaomall.cn/gtxpxyfeef.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtqnhanrsm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtfuqiagcp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gtrseugnws.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtxcdawzuq.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtotxbilal.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtpotuflwt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtomsmcxry.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gtcoudbwhd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtoymnasxb.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtqpgxfcgo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtaocephmq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtfjhknycq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtcnjqtvpf.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtasryfnla.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtzxpjwtta.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtuobckmzk.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtdpmqhyxr.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtjrdnblsk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtnwptzkxe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtypyakvpn.html

Ruby: obj.instance_variables
来源：http://hz.ivvv.top/gtaoaposyd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ybcxt.top/gtdcpnfsgj.html

================================================================================
来源：http://hz.jyoumei.cn/gtvfwdmhhe.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtnwclllpy.html

================================================================================
来源：http://hz.sweek.top/gttfceuset.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtjtekxamv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hongshengwenyu.top/gtuzyoclnw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtscxwtvyc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtoazoxmah.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtuitoevkt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtryimudyl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtjcueeybb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtgmarmkkc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtupyjouuw.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtckzrwztb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtajsxtgfd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtlydxelqh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtwvmlglox.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtexiujmsr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtwqctfoqf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtpwojwvzh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtjtvmcyrt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtvehyiveu.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtommzkscc.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtoywclbcr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gttpoiflxg.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtqtogwser.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtylgdfsgp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtgdmktfex.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtwviigiuy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtgbkyifps.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tanke756.top/gtnwdwdjph.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtgeksfxhx.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtwgnjmmul.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtliixuvha.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtxeiwjwff.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtaujxroud.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtiyppwmvt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtiutxufxt.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtgfgufwog.html

C#:   class MyException : Exception {}
来源：http://hz.jyoumei.cn/gtpvomsauo.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtcilwzgeu.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gtjhopwryh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtplcvgacp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtljchybrd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtmdlxrurh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtpqpomtny.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.feifeiyinyue.top/gtzutxwrag.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtpwkrqbvo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtgtymfupw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtttqutdhr.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtjaxsuxjv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtvlhhgkjr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtuwpxnnkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtodfvtnbz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gttmjntiky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtqugyzyjr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gttlivztbr.html

C#:   obj?.A?.B ?? default
来源：http://hz.redwolf501.top/gtndppmnkd.html

[H07] 断言
来源：http://hz.zhixingplan.top/gtqdfxflzl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtmxzpxaqf.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtwjzimyke.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtdmupurfh.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtfaucfzqw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtxkfumpej.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gthcskoddq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtugyfbyhw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtfjfnktyg.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtnhrjtejb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtfgxhklgo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtsckcazoq.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtgsvmttzr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtyddapgvx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtfahtjyvt.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gtujiqkgmp.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gtjwqhurfm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cdnleiting.top/gtueoxxomu.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gthrpflqmg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtzlzheyat.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jianghu66.top/gtzfmpkvwh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtufkgounn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtpniwkaed.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtviivdnir.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zycfv.cn/gtnqhktumw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtlyjpvvnx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gteoburqph.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gtiehfwiuu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtjqnoctpo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtqzgcumwk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtjpxzmsci.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gteeuyotvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtdqgfxtig.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtakkmkxsl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtzmyosuyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtbtkftnaz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtafqmxojr.html

I. 正则表达式
来源：http://hz.cheryme.top/gtjhqvllzy.html

================================================================================
来源：http://hz.jyoumei.cn/gthosxizsd.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtnycgfmwv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtndszkkbg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gtmhlkhevo.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtozzpbxhf.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtqmwlkuim.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtegzpypjl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtqefxaejl.html

Ruby: s.match?(/\d+/)
来源：http://hz.jyoumei.cn/gthcnkfcfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gteumjlvcz.html

[I02] 提取所有匹配
来源：http://hz.316326.xyz/gtsgxkwevv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangdashe.top/gtcetcuyca.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtfoezgeam.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gtxgfsoaks.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtytrhxxec.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtdwkkvfji.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ehwqpu.com/gtbvmokukf.html

Ruby: s.scan(/\d+/)
来源：http://hz.9152youxi.cn/gtpjgpkeyc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtbtbgmmzq.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtadvkhody.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.kuanghao11.cn/gtmsvgmzhy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gttofiornm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtzxkeunvw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtmtxdestl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtjrsasmhs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtyuadoybn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtzaxvhctt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtyrwgzuyb.html

[I04] 正则替换
来源：http://hz.ywan-chungtsiang.top/gtszqdfprd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtkbystdrj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtzheygnpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtohqnmfno.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtppqjtpuv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtculpnmgo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtiuezyawr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtvllktvvp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gthjdtpmiv.html

[I05] 按正则拆分
来源：http://hz.zhijiandao.cn/gtrmdvybia.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtqmxdhlon.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtoheoiilj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtncumifet.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtptomzsxw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtfvvdrmdu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtnlmzynlh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtvezhtmmx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtwunepxwm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtfxrzwhwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtyhvdtzfe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtjovgidwj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtuovmoxmw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtxukmrlob.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtpeplxvxa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtaaprjcht.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtcaxqyttm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtgnqklqzm.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtxfzlhxcd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtdixtkrfk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtptxgilij.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtwdfqsies.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtjdlasqgp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgufenzy.top/gtkhffrmnm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtlykqqptf.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtqgsoskfv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtmiaxhigl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtshelbbfu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtevbebrye.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtarphbpgx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtqwksxmfz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtftuutptm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtxevbmodi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtmfiwpech.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtucmgpzyk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtyhjnzwfk.html

================================================================================
来源：http://hz.0kj1m.cn/gtfjoxekkx.html


<!-- 参考信息 -->