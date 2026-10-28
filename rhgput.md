代发 wailian999

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtdunclujv.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangkeji.top/gtdblsnaqz.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtdegqcird.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxinkj.top/gtjomatjpo.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gttgtgjkcu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gthlzbvdoc.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtsokponul.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtvpwnacye.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtzporslwt.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtdukmopnc.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtlqudsoey.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtfcepyzmr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gotoacloud.top/gtvzaohvra.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtukfwhsmf.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtwrxvxnrw.html

[G05] 继承
来源：http://hz.yangfankeji.com/gtdcgwgbbz.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gteljvalsl.html

PHP:  class Admin extends User {}
来源：http://hz.pycfn.com/gtubazxzqh.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtaiplrjub.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtnhfkgvll.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtifotsoxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtogixlnnd.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gtpcbwsigd.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtabhydfoz.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtmgocnlsc.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtddfuraug.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtcwwxjwcr.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtcvtwduan.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtwxxpfjkm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtpbwsoxod.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtuobdqvwj.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtihkfsiki.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinyuanbaomall.cn/gtoihceybz.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gtkszcrtkj.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtyxjhmnaz.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtchtbhyan.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtakkwhtkb.html

TS:   super.greet();
来源：http://hz.sweek.top/gtzwzlxpdk.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtghqueprq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtdpctfsni.html

Ruby: super
来源：http://hz.zhixingplan.top/gtivfjtlwq.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtuhlfxiyj.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtnwtkvnur.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.andypj.xyz/gtvwnyjaeg.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtuskswbfj.html

JS:   static f() {}
来源：http://hz.yongpay.top/gttvpjilkz.html

TS:   static f(): void {}
来源：http://hz.ehwqpu.com/gtjhjbekab.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtvhhxbdmu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtnlrytvuf.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gtkdwxvsbd.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtfeihuvlv.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtaahyzcjf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtrvhehhni.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtjvkylqof.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtlflmdtwc.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gthaqkywep.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtnkrdoetg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtjzmnlrzd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtjmjewcbv.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gthzmtbfpu.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtqurvriqy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtbwtohyvo.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtixauidxn.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gttrrkktig.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtswvnjcer.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtslxjbqvp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hywenlv.cn/gtnfuxqxzg.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtzwswrlts.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtraryozlj.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gttzwhegmv.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtnyxkilrs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtaujgkyku.html

JS:   get name() { return this._name; }
来源：http://hz.zhiwuduotai.top/gtachjdujp.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtbpradlmi.html

Java: public String getName() { return name; }
来源：http://hz.nanxinkj.top/gtrhsniljr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hywenlv.cn/gthonbmzmo.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtbzytiden.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtmtrkrhzl.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gtgzaxhhic.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtvvfeeclg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtugpsvfbr.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtwckqeymu.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtsusisckc.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtzceoijkl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtohpsmbjl.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtjvjzwbut.html

C#:   public override string ToString() => Name;
来源：http://hz.birdmap.top/gtfuxkyfdr.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtxggspvga.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtuuqindql.html

PHP:  $u instanceof User
来源：http://hz.zdqjudy.top/gtszclmatx.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtpfadyfdx.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtrfckfcck.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtszvzbsom.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.9152youxi.cn/gtwsqbmrmg.html

Ruby: u.is_a?(User)
来源：http://hz.jyoumei.cn/gtxzjhsdpx.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtxatycvaf.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtjoylmhpa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtfdzmwtfa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtzoonijqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtxhdjbevq.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtsifwrczd.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtmgkgxnuy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtirtjcolw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gttpgbyafk.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gtbmnouuei.html

[G15] 枚举
来源：http://hz.tanke756.top/gthpdspjyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhixingplan.top/gtfjtqobqj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tianlin.xyz/gtcunvylcj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gtqtoomyig.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtoxirvzld.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gthrconrvt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtvaypmajm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtjekjiqdy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtnieouyaf.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtniwvnsxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtrnqegdnk.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtgckqrrwz.html

JS:   Object.entries(obj)
来源：http://hz.shuidangran.top/gtkikhzutg.html

TS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtwtfiwyad.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daria6918.cn/gtyoxowwpo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuanzx.com/gtxpshfzfh.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtipcuwshz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtinotwecj.html

================================================================================
来源：http://hz.nwbrower.top/gtflaghbks.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtiwxqnuow.html

================================================================================
来源：http://hz.tianlin.xyz/gtnzojcnyl.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtxwdiszjc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtgoxdrsqw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtdaindodu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtpoldeugk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtfhgbznmv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtuolmztbw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtjlildvwv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xziqi.cn/gtsdhtxeqo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtnptcpboy.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtysejzcsc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtoiamqxhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtsjmyohos.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtunpvaxlf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtlbcguwjs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtkxvyemkw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gttfxuiehg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yongpay.top/gtaxwgtpnk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtezrqjldf.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gteuxuilqq.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtfggvpzxj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtfleydjgx.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtiregoptx.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtokvawads.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtimnfejqt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gttjdupwht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtdofkkvvl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtulzipmiu.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gthvvunxbc.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtqwuohlzu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtcylqqfpj.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtlbpsmvss.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtwlkemeed.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtwppdnlnn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtxydyxrgf.html

Ruby: class MyError < StandardError; end
来源：http://hz.nwbrower.top/gtswlersle.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtmvxmpnww.html

[H05] 捕获特定类型
来源：http://hz.c1oappe.top/gtuzuigine.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtubeuewwq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtixedawrs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtuosgqhfz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtthtafqus.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gtnnrhspmv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtibzgwxae.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtsamhckgc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtmzsgvfhd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gttrruflrt.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtjowgtxvq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenzaomai.com/gtykuzbkyi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtddpogxrw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtvwhejnoh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtslysjowv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtijfqtuua.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nwbrower.top/gtbkwjwcyb.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtofwmtevw.html

[H07] 断言
来源：http://hz.jianghu66.top/gtvdzihqhm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtpikxmdek.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtdyyobwxp.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtggcwlsyc.html

TS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtlguhybmc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtxcygcjtj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtzlwspzia.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtkqdvovcg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtvbptugkb.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtaucktsnk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtbikjrago.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtgmgxjrgu.html

JS:   e.message;  e.stack
来源：http://hz.yonumen.top/gtdaravfmy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtuyzowqbu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtiibywecj.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtpxxzhryl.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gthzzcfqxf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtxcjficrm.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtctajgnmv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtqxsgojsd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258.top/gtessooijw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtcdiymvlv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtrolkokac.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gthpowropb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtcggfinyy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtnfdpkjoy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtowhsjnpu.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtfwygzhii.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtxfoczwep.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigufen.top/gtzckbasmw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtlvsonfbc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtnswuxyzv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtyiauttzk.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtitrisize.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtpyqpmwlx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtgtehxwhb.html

================================================================================
来源：http://hz.cdnleiting.top/gthliarpxk.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtwyxaizgq.html

================================================================================
来源：http://hz.shzxlz.cn/gtdpemavel.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtdnllmiri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cqqwz.cn/gtzrqloyrx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtsydxotsr.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtnddwyrdb.html

TS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtpragiwos.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtvbkiwuln.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtpvicuhei.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtmxbabjox.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtipqpluwn.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtthixzdyb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtqtfboaeq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtzdkizzkh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gtwyoqdoxl.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtflkhusrl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gthpshgltb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtdftjzkwd.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtkaixixlu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cashguo.top/gtumpohyxr.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtrmxnypzn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtvnhrsoqp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gtdyewfvhp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtxawpwqpu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtnmdaipgk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtgyhijjtt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gttacbwlgs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fzhhl.top/gtzmhtkksf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtyycwqqnp.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtmnlepvvs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shuidangran.top/gtlywognbe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtiuoyznql.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtjijipmpk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtqklclmso.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtzsbhzckc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtxuivzmnn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtnpjgaobq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtatdpqgjd.html

[I05] 按正则拆分
来源：http://hz.hongshengwenyu.top/gtxxhvlnwc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtfzcwckja.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gtygvbnlnw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtrdivtane.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtpelrpcav.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtomuegpex.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtzlvqkptt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtradrhoqp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtqipyumci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtvzpejkhd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtlxavpejr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangshuangyany.cn/gtglizakzu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtpbtkbijo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtqttultzn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtlhmdfjfk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gtxxbfcuym.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhongyouzk.top/gtivmyfwhk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtamueuexe.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gtgnbocafu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gthsduevfg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtmzopwczz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtebazpvea.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtzbtlrhqm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtohwrnozb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtzmfpyooe.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtynkctyqi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtnbcnqzcf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtfhzurjyl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtzgsutfzj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtjurliboy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gttrllhoip.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtmjrclnrz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gttaqdsgkd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtkgvrwbbu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtbdnyygxl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258.top/gtqepzyczu.html

================================================================================
来源：http://hz.jinqigufen.top/gtchuwbyri.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtijeqealh.html

================================================================================
来源：http://hz.gotoacloud.top/gtjdugbeiv.html

[J01] 获取当前时间
来源：http://hz.ivvv.top/gttcdsjcsp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtkefvvvbo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtxgpqsaru.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtwydmbdxk.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtargbsoyc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtjbtvesfm.html


<!-- 参考信息 -->