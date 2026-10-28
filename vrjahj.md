代发 wailian999

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtttjlcazi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtmosjohno.html

[G04] 定义方法
来源：http://hz.xuanzx.com/gtuqmihkem.html

Py:   def greet(self): return self.name
来源：http://hz.nwbrower.top/gtujzcsrqb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtqlogriha.html

JS:   greet() { return this.name; }
来源：http://hz.nwbrower.top/gtemfwbezb.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtejmigcnp.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gtbmerfgob.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtxijengxp.html

Ruby: def greet; @name; end
来源：http://hz.smart0.xyz/gtrihbapbc.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtyqpqnevi.html

[G05] 继承
来源：http://hz.nanxuanxn.top/gtmjaiqjal.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gtzyxkvoqp.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtdtvbdwcb.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtqrxjpwmy.html

TS:   class Admin extends User {}
来源：http://hz.yonumen.top/gthmzbsizr.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtfogprkym.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtcafyxmwj.html

Ruby: class Admin < User; end
来源：http://hz.xylfe.cn/gtzcxbabyx.html

C#:   class Admin : User {}
来源：http://hz.fengsongda.top/gtbvhrpqmr.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtpfaynoiq.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtmwuabefl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtdfbzgunl.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtrmicysau.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtfamrqfrr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtwomlusjr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinyuanbaomall.cn/gtnxwcmtjw.html

Ruby: def greet; "admin"; end
来源：http://hz.havefunace.top/gtpkzkoysk.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtklhfzauc.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtfhpxkhtv.html

Py:   super().greet()
来源：http://hz.jqgufenzy.top/gtvkhuzfqn.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gttgerpbuo.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtotczdbfx.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtrawtjiih.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtirpcsyvu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.vqdsnc.cn/gtrwglteqh.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtcervprmw.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gttbncyuvt.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtgjcpxmak.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtnsfmpjef.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtuezxdadr.html

JS:   static f() {}
来源：http://hz.yuxming.cn/gtasmcjipa.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtqhrvtlde.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtsuethkfk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigfzy.top/gthwtawerb.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtcplodskf.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtrhtjnqlr.html

[G09] 接口 / 抽象类
来源：http://hz.cdnleiting.top/gtgyzzkzka.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtsxcbuziz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtdkldzkjj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ppjwa.cn/gtnxncvqqe.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gttjbekyok.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtrlqhvqrp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxinkj.top/gtagtzldtf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtaqljzxfv.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtalegglji.html

[G10] 访问控制
来源：http://hz.smart0.xyz/gtlfkfjyno.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtdzkftpzn.html

PHP:  public / protected / private
来源：http://hz.zhixingplan.top/gtautpcrsx.html

JS:   #private 字段；其余公开
来源：http://hz.quarkkingdee.top/gtjlpsvgig.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtqlzfgphv.html

Java: public / protected / private / 默认包级
来源：http://hz.jlsjyb.cn/gtkverbbme.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtifcdrbns.html

Ruby: public / protected / private
来源：http://hz.hnqzz.top/gtdaycbiox.html

C#:   public / protected / private / internal
来源：http://hz.tanke756.top/gttehaiqgk.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtcnykpphl.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtnbujwtfv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.meibo888.top/gtbwwiaxsv.html

JS:   get name() { return this._name; }
来源：http://hz.jiagoushi.top/gthmuoiiet.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtjswwwmyr.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtisgwhwfv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtwtswuzki.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtzywfggkp.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtmvjcrycx.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtxuqfqpms.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtwzbjphpl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtgzoccsty.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtuuaszmyo.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtvpfjvnoh.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtgzvybeii.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtjxpjjwts.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtrwwwbmue.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtiadftywz.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gttlyqnsci.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtqogeomeg.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gtfnogexvw.html

JS:   u instanceof User
来源：http://hz.cashguo.top/gtngjsrrwo.html

TS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtrhjvyahq.html

Java: u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtypsnigdq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fzhhl.top/gtewksjuil.html

Ruby: u.is_a?(User)
来源：http://hz.havefunace.top/gtatruyvcf.html

C#:   u is User
来源：http://hz.hfpthk.cn/gtbbpofjam.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtllgnitqr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtdfhmdrjh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sysykeji.top/gtbhogotko.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtaqcnieup.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtzqklcwbp.html

Java: record User(String name, int age) {}
来源：http://hz.yueranfly.top/gttbikjswo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydjk.org.cn/gtnereqcar.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtzzwmejip.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtqcdqxcfv.html

[G15] 枚举
来源：http://hz.sweek.top/gtrlumpybd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.52xcode.cn/gtiutexqzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtbdzeajgt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtldmmzxzu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtsstxqkxd.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtcsiiqgej.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guowangkeji.top/gtbkuhxxxj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtvremplgx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtbwzdozsi.html

[G16] 对象转数组 / 字典
来源：http://hz.daria6918.cn/gtzejxqeod.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtnxkhhptg.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtbhozztxw.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtprsjrayf.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtpgtkunrl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtebgsfzee.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtkifcitvw.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtprxdidwi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtrgxgiubv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgvageyxp.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtsydkpemf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtevhbbnzf.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtrenczlxh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtitlsdeit.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gtyqvzsgqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtegryeekg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtihepuyee.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtocpszhox.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cashguo.top/gtgqntbfad.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtuywicodu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gtvfxhvkjh.html

[H02] finally / ensure 收尾
来源：http://hz.cucudq.cn/gtfzawvqsf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gtmzvhztmq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gteaewlrjv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtcjkjysut.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtubolyfda.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtdqucsqfj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtahwwjadj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aibaodan.cn/gtfgpecjhn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtgvdelhxy.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtclddfuss.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtnmltehkb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtdnnbxcve.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtxxkmitoh.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtxbrdvkcd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtreyhqxtl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtnseastwk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtrtxdclqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtruqnsbkc.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtzjtalfmf.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtnzardvoq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtzcjzyqdn.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtlutjelpq.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtoxplbfqe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtugdnwiqo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinyuanbaomall.cn/gtnrdlpwda.html

Ruby: class MyError < StandardError; end
来源：http://hz.quarkkingdee.top/gtsewfcdbb.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtwebrrdkm.html

[H05] 捕获特定类型
来源：http://hz.cqqwz.cn/gtwhwgimgd.html

Py:   except ValueError as e:
来源：http://hz.zhongyouzk.top/gtngatazna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtftnuhtrz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtstgaezai.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtartqmorz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gttpmbwapb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtipcpzmbe.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gtvdcywgep.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtzujkdkvs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.havefunace.top/gtltagbmnf.html

Py:   value = d.get("k") or default
来源：http://hz.pycfn.com/gtyamyovkq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtipvkjend.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtogcqubjh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtsbaadekf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtzzllbuzr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtxymkmile.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gtljsqktnz.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtmimkunws.html

[H07] 断言
来源：http://hz.yj20258888.top/gtwpdvozrw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dianchejie.cn/gtcijyqjuo.html

PHP:  assert($x > 0);
来源：http://hz.shuidangran.top/gtcxeqqauc.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtqcdkyeki.html

TS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtzvielagb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtaoqaseag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtspdckhhj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtxvdpnkdz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtbvplqvnr.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtssmfwmgm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtxsxtavqp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtjtywmiig.html

JS:   e.message;  e.stack
来源：http://hz.yvedp.cn/gtomfbbpmb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtaijurmoc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtshvpaddl.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtdgxwylat.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtyiidfsju.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtoqtffwna.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gtotsdierf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtxvffjoqi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtgrutcezc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gtssziyjjg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtglkyioil.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gtuhlvomjx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.c1oappe.top/gtkjiomuoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtoaexysow.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtiodsenlj.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtghcqlcsq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtlowxixer.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gthwobrcpu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtuaziules.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtxgicomfb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigfzy.top/gtzenrfrgi.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtbmbijyqz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtokoqppjv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtucmlhijc.html

================================================================================
来源：http://hz.daria6918.cn/gtyixdjrnq.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtpgkoqlnk.html

================================================================================
来源：http://hz.hammf.cn/gtghjdgicr.html

[I01] 判断是否匹配
来源：http://hz.xziqi.cn/gtlynjcmlz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtariidcze.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtvspxmzmh.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtqtnnbpnz.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtinmvjqtu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtzyelyyyy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtrhhmhsza.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gttanoaqpr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtfillimxv.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtsboiurlg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtscomikld.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtpndjqcul.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ivvv.top/gtylvrsjgk.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtoclukwcd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daria6918.cn/gtewaalcfv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtaenvctys.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtjcknubcr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtpjgmizdr.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtgthrrpsh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtjsrrpfll.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yanxiufei.cn/gtxizapfer.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xylfe.cn/gtuzhwujim.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gotoacloud.top/gtpqegykvu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtgfpavlqo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtvohvqrer.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtislbmery.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtzrfxywih.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtqgujtxtk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gttdhtrasw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtbbhjmreh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gthvqbatfc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtjghhjlxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtekwwrqai.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtnywqhqee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.c1oappe.top/gtpoymzfyd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jlsjyb.cn/gtrajnvyxp.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtfmcksmgt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtsheqphke.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtsoxawcrc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtisgtaugj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtmccbtpsg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtwhixwgkp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtzrbnqhwo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtgejjfive.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gtjvevatyy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtrqifqvml.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gteqgzwbej.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtivanoulm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtypsnedkv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtqusamoqw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtihtadzqo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ywan-chungtsiang.top/gtrdortvxj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtgzwfveuf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gttnytgxua.html

[I07] 忽略大小写与多行模式
来源：http://hz.hammf.cn/gtxppfasfa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtibrtjnfh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gtwweqnjxo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtdpeisdlo.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtijcbetmt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dianchejie.cn/gtvikgnnfj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jiagoushi.top/gtevsmrytz.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtqdosofis.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtwfdjhjxq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtrpwpqdfo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtzszjxrsh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtihbdzhqn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtbmdfbllc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtrqxftfgs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtrpfldszy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj202588.top/gtlditfdys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtzriupfkb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtacbylpcv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtizsypbrj.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtaxnfmner.html

================================================================================
来源：http://hz.zdqjudy.top/gtlpdjsdwa.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtnjlfmvii.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtzqhasavj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtvobhnqdn.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtdtpjtlbe.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtxcsacjyv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gtzflexqyh.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gtzwdzhpov.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtwxifhare.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtwpdpvtfl.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtybimlmgs.html


<!-- 参考信息 -->