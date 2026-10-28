代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.hammf.cn/gtrebqzcco.html

[G03] 实例属性
来源：http://hz.yongpay.top/gtjuuwkthd.html

Py:   self.name = "x"
来源：http://hz.zycfv.cn/gtbqukgapz.html

PHP:  public string $name = "x";
来源：http://hz.cqqwz.cn/gtlhodlprm.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtnwjjxmaq.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtfixqjwri.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtrpudoxse.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jiagoushi.top/gtdavmpevj.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtbmqtjuod.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtrnytwkbe.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtpsbpwext.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtkczffapp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtzwlwmxuq.html

JS:   greet() { return this.name; }
来源：http://hz.dianchejie.cn/gtclbrtrnv.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtucfejnei.html

Java: String greet() { return name; }
来源：http://hz.jinqigfzy.top/gtxbgqksfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtcbgnovhq.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gtuezrvpes.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gttanwrtwl.html

[G05] 继承
来源：http://hz.fengsongda.top/gtlpaoaavj.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtvghomnsg.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtujvlftge.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtcmurxtyj.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtawpkndsd.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtlcamolcn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gthjsjzrcj.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtqcygedyd.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtivzxtbih.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtqlvfdxla.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtxxtjzlbp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtcmaypcyr.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtqynuwzuz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtsqesndsr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtxkftmxnk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtqwkxnwfb.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtskbvsjie.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtdbhryeqj.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gtstemptcl.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gtihxyyglm.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtlufjaepe.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtaxhqseoh.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtdukdjpzx.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtwkhmawlw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gtyizmgteu.html

Ruby: super
来源：http://hz.cqqwz.cn/gtekvncioi.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtdyuagzyp.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtoraojmqi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtswawoida.html

PHP:  public static function f() {}
来源：http://hz.yj20258888.top/gtmljlklvi.html

JS:   static f() {}
来源：http://hz.cashguo.top/gtjimgxrfq.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtlozveqij.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtajfnwzcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtrqcxrspl.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtoitxenvu.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtbdytaexh.html

[G09] 接口 / 抽象类
来源：http://hz.tianlin.xyz/gtqhlfoioa.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtojbddibw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sufxvd.cn/gtopxrmgjf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gogol.net.cn/gtcacsarnw.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtfyjfssyv.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtsvrfkamf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtmrxxnioz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtqixulfxo.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnxiangtu.top/gtuacuprmw.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtyalamygk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtmcliogmq.html

PHP:  public / protected / private
来源：http://hz.meibo888.top/gtlxcdahwd.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtkuczotba.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtcnnpqdvu.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtmbibmxkh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtnwridrzt.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtvoigrsft.html

C#:   public / protected / private / internal
来源：http://hz.hongshengwenyu.top/gtgcxlgzfj.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gtdyeqffdk.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtyjfzjtdc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gtlrdvcqpf.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtzzcmzvmn.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gttyvkengb.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtkfrxmndf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtsexzxqhn.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gthqfakdzf.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtgjquyyfa.html

[G12] 对象转字符串
来源：http://hz.xuetiantiany.cn/gtkmzjzyda.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gtjqeuyzbx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtnxuydmhw.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtldbpffam.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtwewvexeu.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtzvswunfi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtbtdolezr.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtxnwuitol.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtxdnnuuzl.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtzwtcuqwe.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtevuitqyv.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtrlzvxodr.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtwceyhjqf.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtisioerhq.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtqwtehwzx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtelmpsgnn.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtfewejvmc.html

C#:   u is User
来源：http://hz.iojbl.cn/gtfcwhaatk.html

[G14] 数据类 / record
来源：http://hz.ehwqpu.com/gtqrowjtsj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtmlrzrxgd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtnvlenhoe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtziivkabf.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtfkxkhoxp.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtemyyhoje.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gteciiyqqi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtqnxshvyk.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtsttgtvkp.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtkthbjaac.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtabvatcim.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gthuregydv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.smart0.xyz/gtsdslzyvg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtdssjxfjx.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtjslnelrq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtwmrppkbw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuanzx.com/gttntsdknf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtikaizhvd.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gthccvkadu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gttftoymus.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtxrcohixw.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtyrejmxeu.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtnhunfltt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtzwfhgors.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtwvmonttg.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gtojoyhewc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pengpengdd.cyou/gtsgajwjzr.html

================================================================================
来源：http://hz.jiagoushi.top/gtvigqfgzr.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtwaesgfpd.html

================================================================================
来源：http://hz.jiagoushi.top/gtrjrqfkvb.html

[H01] try / catch 基础
来源：http://hz.xingfuxueyuan.xyz/gtzbtwrfkc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtmerjpkvu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gteorjvswy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtvqepuweo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtbkxdsxer.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtvvpoxkyx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtmvvhxecv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guowangkeji.top/gtrppqjmgb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gthmhlvviy.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtlwoaemag.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guannengcc.top/gtulnsnnam.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtzikdflsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtcfubxspc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtjzcndeqt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gthurpndhk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.9152youxi.cn/gtagfxuakx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xylfe.cn/gtfyrrzgpn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtsrqinkcg.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtyuajylbf.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgufenzy.top/gtupkwmkul.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtcmuindhr.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtqsamdufh.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtqycmomdp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtxsyphlcx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jiagoushi.top/gtohqbpswu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtmuetlqql.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtpvmsqieb.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gturxlfxwr.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtsgmjdqnl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gthjqotgao.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtnakwwpzk.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtcvljtnhv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtuozshdms.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gteebkeefq.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtdtrtwoes.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtecgxkmzh.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtgehrkuof.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtgtryeifv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenlongwang.top/gtxkfldmlz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtuybmxwae.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtjifllfbq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtqgqyjvwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtxdtpzubk.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtdavtadvc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aizwys.cn/gtjrjcxgnr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gotoacloud.top/gtgusvuinb.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtkpahcsxr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtlkkjfpmu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtrinxoqqh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtwxbjhncw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtcrlqbnio.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gttpxggwvq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtezjarlms.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangtech.top/gtddsyjret.html

[H07] 断言
来源：http://hz.zhixingplan.top/gtexfwkwsa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtchxdzjvy.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtohkkgexa.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtkkkajlak.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtgygkejuf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtbvizzhef.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hongshengwenyu.top/gtmyfbkiqv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gtvthptnhw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtojhbnhkl.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtkbbhayvg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtwiescfgf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtdioafntp.html

JS:   e.message;  e.stack
来源：http://hz.nwbrower.top/gtbujfdgau.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtiksrbvqj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtxyuymjfu.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtptnwnzzd.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gtziicyzwe.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtxdxxeqvb.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtfhzprptg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gterjyqoip.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtvtrltktb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtzybigmey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtmujgkknj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtbvnoojfe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.c1oappe.top/gtcxuukwcu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtuxvwlbpu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tian-w.cn/gtarnmcmck.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gteqprduki.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtxknnkigz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tianlin.xyz/gtsvvtnenf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtjiqitmbl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtwyfvnnqu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtcanelmdx.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtmsathoux.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtlywqiulp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtwyofggno.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnjnuukpv.html

I. 正则表达式
来源：http://hz.shanyushiyangkeji.top/gtccjymump.html

================================================================================
来源：http://hz.wangdashe.top/gtzkrecjld.html

[I01] 判断是否匹配
来源：http://hz.meibo888.top/gtiyzdsjkm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtubcerpgh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtgqiirevq.html

JS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtbbdvsmdv.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtwnmygfil.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtalhjfzwt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gthzrutxnf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtpfhqhqqa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtyaxmwrxr.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtbwrhdobs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gttwhafapd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gttagusbkv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gtxjoedwxx.html

TS:   s.match(/\d+/g)
来源：http://hz.zdqjudy.top/gtkfamgdfy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtmnzxydag.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtnsgfodad.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtvwpxzmyy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigufen.top/gtfsaaxgwv.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gthnftivhp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtbtalvlzt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtkzrkryrt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtitddfkxu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtugqxulmz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtscmouart.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtlhlogchz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cucudq.cn/gtfedewbcr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtfjobfetb.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gtvymzgbkr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yangfankeji.com/gtzvazgdpg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtmvalshke.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtaqysiywx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtxgkvbwfl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.0kj1m.cn/gtottqnfbt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtgfmqnvdz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtydgphdzx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtwlrrrjkt.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gtemgkawas.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtdpmvfelh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtchoeuxmu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtjwkdotrg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtjoyhofwn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtnqrokbex.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtwubcjufl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtkfltkxrc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtrpynsmhk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtkuqmmnky.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtgvlpoavc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gthvqoeicp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtwurltiwk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtbrkqirup.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gtxilgbbwh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtirqxprjp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtgeanigro.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtxmtplvvy.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangtech.top/gtubaliqtx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtojsxkdll.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gttgbwgirr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtlcgzrlpv.html

TS:   /error/gim
来源：http://hz.fengsongda.top/gthgaqcocd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tian-w.cn/gtzlsygpjp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gtfibwhvxm.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtavkxsmzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtvsgusecu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gtescvhkgv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtklhhiecl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtcofvdyob.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtbxtgviul.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtqdmcjnul.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtwqgmntpv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtvgkvdkcn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtjslllyzt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangdashe.top/gtwenofrah.html

================================================================================
来源：http://hz.jyoumei.cn/gtdokqgutw.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtedqcxxbu.html

================================================================================
来源：http://hz.yonumen.top/gtfebwyykx.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtnpgpdzjv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gthpqauyjb.html


<!-- 参考信息 -->