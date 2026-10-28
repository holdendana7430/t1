代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtbqspwwvt.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtlbgdkvyt.html

TS:   greet(): string { return this.name; }
来源：http://hz.zycfv.cn/gtxdqdxtky.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtpquejyao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtcrfyccmy.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtphalejze.html

C#:   public string Greet() => Name;
来源：http://hz.svipenyu.cn/gtcwghbngg.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gtsculgwbq.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtrfpjabpb.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtgqbxzwpq.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtabsirqqb.html

TS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtgkijjqfz.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtzibazeic.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtjyluobut.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtyluppsuc.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gtfpjiqwmk.html

[G06] 重写方法
来源：http://hz.sweek.top/gtwaxkzqhd.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtnfegpngx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtqrwedvgc.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtumdvxddt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtkaydxhqa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtqneayoye.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yonumen.top/gtokvmabbz.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtpznlxmgo.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtkumcctih.html

[G07] 调用父类方法
来源：http://hz.jyoumei.cn/gttmrxltki.html

Py:   super().greet()
来源：http://hz.ehwqpu.com/gtmlhvyvzv.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtsyjjoyqm.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gthcldunrk.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtfnkbaqfg.html

Java: super.greet();
来源：http://hz.hammf.cn/gtblezunzf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtzeoprmqt.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gttooihniv.html

C#:   base.Greet();
来源：http://hz.cucudq.cn/gtfversjsi.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtxatxidls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtccdmqvsh.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtvmedbwzs.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtiyjdutou.html

TS:   static f(): void {}
来源：http://hz.zhiwuduotai.top/gtmvawnlht.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gtacjenfgh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtqqlgqeai.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtvhwamgqb.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gthnzvbfdp.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtgfungkpl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gttbykkrnf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtjpwtvhat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtjtppyvcx.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtybbsuobp.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtdemywzsi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtpwnbiaze.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tanke756.top/gtvvgecoss.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtwpldvjph.html

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtjggbqmac.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gtzyzyqyzt.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtehdwsswd.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gttucyyayq.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtosvekfep.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtslrddcvs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtizgbjnhn.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtyhvmfbbx.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtjmdhzypw.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gthjuyakok.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtesglzpra.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtfkrpztwt.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtaphnzatt.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtywunrzzd.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtgvqadoqy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtgvejkbiy.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtgwumcrzf.html

C#:   public string Name { get; set; }
来源：http://hz.birdmap.top/gtgspmsgsr.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtqnamsllo.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtzlxxbqts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gttmvbyngx.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtbebjsoza.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gthilzgrbn.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtidiquxtp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtxtkrlzqo.html

Ruby: def to_s; @name; end
来源：http://hz.hammf.cn/gtfcruwbzn.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtpejzezlr.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtmqyojdme.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtwwoousqh.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtxmqjppur.html

JS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtnnebnhhf.html

TS:   u instanceof User
来源：http://hz.cdnleiting.top/gtzptusxpc.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtnsvuihcl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtkygoieaq.html

Ruby: u.is_a?(User)
来源：http://hz.mhx1999.top/gtdcirqziw.html

C#:   u is User
来源：http://hz.xziqi.cn/gtrevyazij.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtlviarspu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtifnvfxuw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtafyszgov.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hfpthk.cn/gtlgnkdwcf.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtpzjkqetc.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtehuklfka.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtekfsxkpt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gtjqavmrex.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtomirpwno.html

[G15] 枚举
来源：http://hz.bjfxy.top/gtkrwutohk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtdgrnztnn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtpggyjupf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtbrzyxzpp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gthrbjmbcy.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtgawmwimv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtshufbnmo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtvsuisxtr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtfsircgni.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtgktoqmnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtbvmdjnhl.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtoigymiwo.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtqfgqxvad.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtexjuyyry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtrhuklrmr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yonumen.top/gtjxxfvamv.html

Ruby: obj.instance_variables
来源：http://hz.hfpthk.cn/gthxwrxsul.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtgzsritys.html

================================================================================
来源：http://hz.cqqwz.cn/gtpmjfcbhg.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtcmbvripc.html

================================================================================
来源：http://hz.guowangkeji.top/gtrlmwtczz.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtfnxmanvc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtlszkqbmp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtffiroelh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtyfshulhc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtpqthqsxd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtfcrllmwf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangshuangyany.cn/gtpbeqglxj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtcxedeifz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtfmmrwwqt.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtnxfuxbkp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtquyeyaoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtcmkoazxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtdhnpvqbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtgrquxuxg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtomsrdwjr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hywenlv.cn/gtvlhiggmt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtwrbqehxh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhongyouzk.top/gtpurcvctf.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtdwcbnbjl.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtwpouqune.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtmkzfmvai.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtawaoztrn.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtlwnmholo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtxrzyvtlm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtbvsdwffz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtjtjzmgjw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtsudtkaze.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtbumjflnz.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtnfelahfl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtksbltjds.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtiheggbbx.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtjbsbywei.html

Java: class MyException extends RuntimeException {}
来源：http://hz.meibo888.top/gtslvzogmd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtwgcopwrn.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gtojcrqquv.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtsoeunzez.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtczgrwoaz.html

Py:   except ValueError as e:
来源：http://hz.kuanghao11.cn/gtuyotimfc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtqpujqhmq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtxnsfbjiy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtzdzvnzbn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gteccedzxg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtmtafclsp.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtnftkgklg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtovltmwaw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtkmhlujui.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gtmohfeeko.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cqqwz.cn/gtgczyslcb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtavdjeuzt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtnneibpen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtskecught.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtspkoryjb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtaykyrvjn.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtxvgodtiv.html

[H07] 断言
来源：http://hz.bjfxy.top/gtjdudmyid.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtabhyclir.html

PHP:  assert($x > 0);
来源：http://hz.zhijiandao.cn/gtqogotbrv.html

JS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtiremvpts.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtiliefrpj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtuzagizyy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gtopealacj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtrjjncwor.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtvtdjbtqg.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtybpedymn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gtrrzldnev.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtjbmkogoy.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtefbjsatm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtwryusbdr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxinkj.top/gttwbkcfps.html

Go:   err.Error()
来源：http://hz.sweek.top/gtlqtuxwge.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtiujfmqqo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtsuezzskn.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtkcvdybly.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtqijiruzu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtryzyyvez.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinyuanbaomall.cn/gtwpixaiig.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hammf.cn/gtupdaxsos.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangshuangyany.cn/gtezlwleay.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtivwvcgvk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtndsrwgjx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtofbfsuaq.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtztfostqa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtceevcpoj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtotrdbccu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtecdhmpxt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtqihtoogm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtfurnvsyl.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtfttijnsp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtqbysjmog.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangtech.top/gtavhsblgd.html

================================================================================
来源：http://hz.smart0.xyz/gtayrqmhpl.html

I. 正则表达式
来源：http://hz.yj20258.top/gtsuffzdpk.html

================================================================================
来源：http://hz.tanke756.top/gtofojhuax.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtghenqvhl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtpvcdymfh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnqzz.top/gtbkbeulhx.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gthrqyfobl.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtrjhakbdb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gttbmdompl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gthkobgygt.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtrskvwwrg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tian-w.cn/gtqkalzdux.html

[I02] 提取所有匹配
来源：http://hz.gotoacloud.top/gthceijagf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtgltwtxni.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtcjjzsrvd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtkvznrmsd.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtehgonkei.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtbznwlajp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtyidyjodm.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtpsnzflqu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtmokxjpvw.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtdhtvfjpu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtxawvaajl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gttsaenfzb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtmphbiqbl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gtirlotxxx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gtjasznatv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gtsvkolhmx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtfjhtefee.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtmjcswloc.html

[I04] 正则替换
来源：http://hz.zhijiandao.cn/gtidozksdy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtxtpfxiyy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtqoukaewt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtqeelrpue.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtvkcpzodm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtjrzqihpi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtykjlucga.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtrqrnyjzj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtwzawqppn.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtwjfgubzi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtgfupaswr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtuljuruvx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtyjwtctiy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtijopnycl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtimxmplih.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtjfgabukj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtarudtucl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangtech.top/gtkwprybef.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tian-w.cn/gtyrxfuccf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtplizviwi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtpkenpgbl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtitjloqfy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gtewfmkbjj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gtvzzrbqkx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtndlovlmd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dianchejie.cn/gtwcmjcrnw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtfwfdbeaw.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhaomingkeji.xyz/gtgzlokxmf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtmmhoszal.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtvokmowzz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtaqpkhuos.html

TS:   /error/gim
来源：http://hz.zdqjudy.top/gtcaghrzxc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xinyue.icu/gtoqnhcarv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ppjwa.cn/gtddwygmvb.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtmnvgzcyt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtxsimdqyz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtbnlmnlia.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtkzgkacov.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yueranfly.top/gtmvarponi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtmpjlgaqr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtzqvbfjyr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtwhyviocc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtkgsihrsl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtilizktth.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtsfcsytkq.html

================================================================================
来源：http://hz.cheryme.top/gtjvpovxay.html

J. 日期与时间
来源：http://hz.yueranfly.top/gtovyzempi.html

================================================================================
来源：http://hz.sufxvd.cn/gtdpbozoit.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtmvqsizdx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtplktsocw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gthkycwpzx.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gthwvljlgk.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtkbbagzgw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yongpay.top/gtavwjugzd.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtbhjnfwbk.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gtsxfyoekf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtbbdsquud.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtbbdversp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtbeeiecey.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtbjnsowkk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtjvsrawki.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtqjxzfujd.html


<!-- 参考信息 -->