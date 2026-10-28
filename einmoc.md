代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtvqbvzpnu.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtpkqlutej.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtntdxtnfc.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gttuqxwumu.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtjanaxmet.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtgucedggj.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtmqkdhral.html

TS:   class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtjhguaiqp.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtqszvmkyo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.svipenyu.cn/gtlcaqtbcf.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtlninzdue.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gtyscoqgxu.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtxgjqxjir.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtblmsbfuh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtujcudkiy.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtzabxmkto.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtwpddkvtc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtzcrfmybe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtfjxbjphn.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtmldzowfw.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtrplbjskf.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtnymwrjjy.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtobqhkbzl.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtttlecvev.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtkpyffwzw.html

TS:   super.greet();
来源：http://hz.sufxvd.cn/gtynieukly.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtxpnumzqv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtqdpbkoim.html

Ruby: super
来源：http://hz.havefunace.top/gttpmyelxa.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtisahvptv.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtqfwsftsp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtqxnxprtb.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtsmfownuj.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtwsjfiuwc.html

TS:   static f(): void {}
来源：http://hz.jlsjyb.cn/gtchqunmyt.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtsnnvegvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtczevyalu.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtspwmrmtg.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gtpdpgjkxk.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtdrylvgsc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtgjmhnynp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtqvhwnfrz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuanzx.com/gteobsbnez.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gthfetgcmf.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtzyaxnttj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtagiukxgz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yvedp.cn/gtcesqldnw.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtzxttljdn.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gtwzalquwe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtrkpzhwkx.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtrcgamhex.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtizyunfot.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gtgodfkcqn.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtebwrybcm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtvypubamd.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtkpzruijf.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtdhqpibby.html

[G11] getter / setter
来源：http://hz.fzhhl.top/gtttmneffz.html

Py:   @property 与 @x.setter
来源：http://hz.haohaochexian.top/gtpnfklpni.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtxkwtuuie.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtyqjdzfom.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gttfdbqggi.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtgfrqgmqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtrvqokour.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtgynsaqfy.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gtmoveaehl.html

[G12] 对象转字符串
来源：http://hz.shzxlz.cn/gtagtzwjwg.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtdoswxplb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtymzhnbmn.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigfzy.top/gtbthjevuu.html

TS:   toString(): string { return this.name; }
来源：http://hz.bjfxy.top/gtwodupyqd.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtmhoxgjbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtepwwznof.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gthokiiqdn.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtjnfethss.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtttfmvhub.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtrdjtwtxo.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtvmffnhbo.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtkeenoirm.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtcxrootko.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtgbwodssp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aizwys.cn/gtaawjjwke.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtomvzqeao.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtletumkvo.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtwemnpcup.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtjciurcbh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtzpzknmxy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gtfffkpaxa.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtjsgnfyqo.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtgmayvrly.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtzhythayk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtuhrvwtzo.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtpxqvlaly.html

[G15] 枚举
来源：http://hz.haohaochexian.top/gtqwfokojy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gtraqyvcrm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtrrjgbwxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtjgqqplzr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtuocvpjed.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gthwtdhhkx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtsnemqmqk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangshuangyany.cn/gtwwixcdes.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtaxnyujim.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtrpqpiuyw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtsdjiibbl.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtojfngidd.html

JS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtqbtlpbak.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gttdcxmopm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jyoumei.cn/gtvwxfuurb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtmbzdoqqo.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtlfudxekj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtgceadlsn.html

================================================================================
来源：http://hz.gotoacloud.top/gtrjofhvrq.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtbtsobygr.html

================================================================================
来源：http://hz.zhengqikj.top/gtfilotabn.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtjzevfwjm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtofhggvaw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigfzy.top/gtvmfsgagz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtwpmxojdw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtefbqrajm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtaovoxrjd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtuntixnal.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtppuyzdbs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gthuhmqmgr.html

[H02] finally / ensure 收尾
来源：http://hz.ydzc1.top/gtyqqlirkw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtwdeqjggh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtzmoeqrvf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtoyjfffjw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtnftmqsbc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtupomrkrw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtzvwhebwg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.svipenyu.cn/gtqieiaxqd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtszzcumho.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtwbwbggat.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtlkmxfpxf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtyqcuckje.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtonizzyyn.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtwhlyscsc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gthwigfjlp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtbjntsjui.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gtydaaqdki.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtpkftmpxm.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtwwrriwgj.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtryrspktr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtdtutqbnf.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtzvdmhjeq.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtmmcenogg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtohxkuato.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.andypj.xyz/gtxyhtfyal.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtevcmzrff.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gtetwybxjo.html

[H05] 捕获特定类型
来源：http://hz.zhongyouzk.top/gtjmvfbmgi.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtddghlyot.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtpzbonmlg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gttwjszhak.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtymgwwjjl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtorcnqxty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtdcenyhvq.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtepbfaowy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtvxnoquis.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtpvesoqsk.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtaaltmfkj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtkcjviefi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtkpcwboit.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtrhwxpfxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xingfuxueyuan.xyz/gteeuyoxfc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xingfuxueyuan.xyz/gtcjqeupnv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtodssdntp.html

C#:   obj?.A?.B ?? default
来源：http://hz.hywenlv.cn/gthceushxw.html

[H07] 断言
来源：http://hz.snrcjt.cn/gtkhddxfts.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtbunqrpdr.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtupvoosxw.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtzrcpskvr.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtqqypmlxm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gttsqrqvhb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtpaqryinw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtnjtcodts.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtxcvfinwm.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtsfxwdisj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtovzbrifc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtmglexoyb.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtzokewwkp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtchskkjgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtmqlhvivi.html

Go:   err.Error()
来源：http://hz.nanxuanxn.top/gtwzsntldq.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtriqmyjto.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtrxxbqewz.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gtjazkvizj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtqtugqwbr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtjeaavfzz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtzctsnvgw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtclmlyccw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtsceabvpf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtisbjjnso.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gttadkesov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtxonsjwwm.html

[H10] 资源自动释放
来源：http://hz.chenlongwang.top/gtbqalftfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtcpupddnc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtausdvzaa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtwlozvnvb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtpnptxiie.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgufenzy.top/gtnxvmfrye.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtxljtfkzf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtotvpzsre.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtpsoblhgo.html

================================================================================
来源：http://hz.aizwys.cn/gtouklkmdl.html

I. 正则表达式
来源：http://hz.sweek.top/gtxcglfyjj.html

================================================================================
来源：http://hz.fengsongda.top/gtiqbowjan.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtovtmhrxs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtujtqmyqm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gtywoubqjo.html

JS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtppbdvswa.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtsjjxmcbt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtqjehbqxe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtrufznckd.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtdzorzoqi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtxvijmnsc.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gttrxlgofu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtncnbwiid.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangdashe.top/gtjbbxahmd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtklmncqwe.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtgwqjbyui.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fengsongda.top/gtaxvpnhfi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258.top/gtrausfbyw.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtifvepwyd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtwjoplxwm.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gthkzbrrcr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtqtaiotfx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtleeuezhk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fengsongda.top/gtpmemlsgo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtqkwhmfah.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gtayvcznoy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtsdrenrnl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtqzrmjekw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtjrxqddhm.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtwebfaisr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydzc1.top/gtkcxsnzzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtfobtrxmg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtawjvcpmd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtoyktkcab.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tanke756.top/gtwhkkddar.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gttszildnl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gttsthezfz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtohjjxgum.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtkrrqcyzn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gthokgijtm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtcdbingeq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtemnxdfna.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtialmgugs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtutjtnssk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sweek.top/gtcebpdnib.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtbjxvzzsj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtzqilxqrx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtlbychjik.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtjuptnbpc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtvvsbipov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtflulqasn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtaqrjowju.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtvxgmflqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtfjwexfnf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtgfqtesex.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtomikgtaq.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtfikskhnk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuanzx.com/gtrkygcpyx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtqoptpszk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtdpsxocwm.html

TS:   /error/gim
来源：http://hz.zdqjudy.top/gtjmmoogcd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gttfewatqq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gttstrsuut.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtrkfzbejv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtgyxrrdeo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtvafkhjdx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtrajkppve.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtwoolrlja.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtcwoxvjcz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtejrnjhtb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtsxfwigac.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtywpeuarr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtyjdpvgjk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtggbjmwkz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgnltynjh.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtlsdsqwyv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxcfkfiap.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtwfoblmwb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ivvv.top/gtcbvnvfyt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtuwujpgqz.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtlretvsvj.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gttefoqpoh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtvetnaaor.html

Go:   time.Now()
来源：http://hz.sweek.top/gtheedulmk.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtvtpjzdvx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gtpgtmygqx.html

[J02] 格式化输出
来源：http://hz.jqgfzy.top/gtdujcthhl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtfmynzebg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtwgnviucv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj202588.top/gtjymlzrzp.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtmeueufzj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtaicwaokk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydjk.org.cn/gtorjzmszd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gthwowaitd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtnmdhzhhq.html


<!-- 参考信息 -->