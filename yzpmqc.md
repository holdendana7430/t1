代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtwwstdnwq.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtxipsnbjd.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtdgaqqltl.html

[G05] 继承
来源：http://hz.gaohongyu789.top/gtdkbfuniu.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtcpeldrfc.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtioyhqdyf.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtwnkszmit.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtelcpwfmz.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtryqnsueg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtoigyozvd.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gtbgedutwr.html

C#:   class Admin : User {}
来源：http://hz.redwolf501.top/gtoqjkrdeu.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtsosbmjxm.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gthpofkpje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtwiqcavmi.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gtaahqgeai.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gthqdxwuqh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtpciqvpmp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtpyhgebmj.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtodydfluu.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtikpojqjy.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtnxgshgub.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtwxqqqqzx.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gtzxeavwsn.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtcfulayxx.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtgnuosmie.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtfclrdhfa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sysykeji.top/gtpewiemyg.html

Ruby: super
来源：http://hz.jiagoushi.top/gtwspmrrxu.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gttnandacg.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtgpuhvxrz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtohbllcne.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtdieiytei.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtfaiurhdi.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtsrivjrfp.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtridikhuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtxmzaayaf.html

Ruby: def self.f; end
来源：http://hz.jqgfzy.top/gtlqdcrkjf.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtrbfhyvtl.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtmsiexyyp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gtywhopfee.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtuauvspff.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gtivzxkepr.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtoyvyjjjm.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtlkcrpdff.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gtkuimfgfp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gtrtsnssrw.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtplsdocna.html

[G10] 访问控制
来源：http://hz.xinyue.icu/gtnsksqyzl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hammf.cn/gtzvfghfgh.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtpifirqcm.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtmjcwcqox.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtaldkqqcg.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtfpfqbffs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtnajclkgf.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtnkcqacwu.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gthpfyeudf.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtcsmwhqtr.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtscziszpj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtvpazdpud.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtwklfgijh.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtxdkrfafc.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtcmefonso.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtrwlmbesj.html

Ruby: attr_accessor :name
来源：http://hz.meibo888.top/gthvkznccy.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtphwjiqil.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtxkimevjw.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gtsyqoiqhn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtvvzxlyms.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtydojpgai.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtyaduectv.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtqoyoygsd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtkrrwgwhm.html

Ruby: def to_s; @name; end
来源：http://hz.xziqi.cn/gtqnqslbld.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtmonindrk.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtssfcjncq.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtmsqzblza.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtkomluhzi.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtincedaki.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtdguitphw.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtkngdvptq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fengsongda.top/gtgbfbssft.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtqtcvqxol.html

C#:   u is User
来源：http://hz.yuxming.cn/gtrlmmfvyq.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtukonactn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gthscfousa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtxoqgcymb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtdnpxhoxc.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenlongwang.top/gtmysbxavr.html

Java: record User(String name, int age) {}
来源：http://hz.0kj1m.cn/gtsfwqosmx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtokodpygx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtwhnamxho.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtkjsuoood.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtpjhiotye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtzugtohkh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtyjylzkeb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtbabzdzhr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtybkpwlvp.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gtqfgmlohs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtelnaigni.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtdneuwapl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtqeoltpzt.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtzlhjahkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtlonuorkc.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtwonfwehx.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtlnmixtwy.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtfuymppsi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.9152youxi.cn/gtsgxyihgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtvhmuzrgb.html

Ruby: obj.instance_variables
来源：http://hz.fzhhl.top/gtasrgdzve.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gtoayxsdyl.html

================================================================================
来源：http://hz.cashguo.top/gtuzdpadjt.html

H. 异常与错误处理
来源：http://hz.jyoumei.cn/gtlltlbxoo.html

================================================================================
来源：http://hz.xziqi.cn/gtqubbbnjr.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtfelabeam.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtpwbscyxb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtgkxeolnk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtcspwqfou.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtieaphdvl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guannengcc.top/gtolebjcwl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtnjkelsrv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtjnmmekiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtwgasdyow.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gtnasvtqqv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtryqrdhok.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtopolnezo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtqkobyxrz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtfxqbsqdq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtnftkktco.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtagwhpxsp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yongpay.top/gtdgouuumw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtbijtbpqc.html

[H03] 主动抛出异常
来源：http://hz.xylfe.cn/gtujdbause.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtfyswwpbq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtrkstyoyk.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gttrgrzoql.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtfqdcstst.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtjtgbpvvo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gttpqyejdg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gttluyfbex.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtrivfdnpq.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtzksqoerh.html

Py:   class MyError(Exception): pass
来源：http://hz.chenzaomai.com/gtxxwxusbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtnzjjjruo.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtuoeaodji.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtswgkcawd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtklputqvx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtqpqitjrh.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtojnndalf.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gthbefcyxr.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtwsgwmwke.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gttdsjiaam.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtqasblxbi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtffzgkdfa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gttzpcxite.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydjk.org.cn/gtsftiveor.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtylimmkbw.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtvtmvyglz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtnuubxohd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtggifkjdp.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtruqbutmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gttwvthmff.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtuwvvyejm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtgpxcuemt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtmpvgrkga.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtnelhrjbh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtojfraqfb.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtajyyifbu.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtwheynhtn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtilqxnjot.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtwmzuzone.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtgbkfgktx.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gticdmdxfh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtevsydfir.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtploqwoye.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtvlnsedxh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtdhyravws.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtiufawjru.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gtdhbrszfa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtrlxsqsqm.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gtpzbipxhe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtrsvhybmx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtiqcrpocw.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtbtjhuimf.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtazauicrr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gzhubu.top/gtfkwohtkt.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtotxudxsn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258.top/gtmrsplbek.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtncxpwvak.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtcrykgoao.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtrndduhxf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtrmibomhk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtaslzjesd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtmqzzclrq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtoawdruwy.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gttjmmodwa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtcqflmecg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gthhirodor.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gthsujsyor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtgqqnmart.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtdtgrkdbc.html

Go:   defer f.Close()
来源：http://hz.smart0.xyz/gtdafmubdj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtkelinxhn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gtrtjdpcux.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpkzfqifx.html

I. 正则表达式
来源：http://hz.cheryme.top/gtrdwtjiqh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnotykgem.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtbxeqhruy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtncxolaux.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.svipenyu.cn/gtszsjhzvh.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtztcxnzfy.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtgmhbfkaj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.smart0.xyz/gtfojqljuu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gteqvmxqyx.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gttnrzgkug.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtydcaujsv.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtgijrafib.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtajthquvt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ivvv.top/gtgrjcmuxd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtaxfxoadu.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtbsvfsptn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtditmzxjk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtgvtsxyby.html

Ruby: s.scan(/\d+/)
来源：http://hz.pycfn.com/gtgijvrihx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtqduxhszy.html

[I03] 提取捕获分组
来源：http://hz.ywan-chungtsiang.top/gtqibrmggt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtfznsnonb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtqjmfxthc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtzrdywcaw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jianghu66.top/gtxoijzlqr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtpxfkiavh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtpmgyjiat.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtnqlxkkjl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtxtysyzpr.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtfrwqrvts.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtqydyrpyr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtalkxqtuw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtkbagbcpe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtmyxvckur.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gtnyoxvlof.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtyjkhnilp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenzaomai.com/gtpsollaht.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtdgepprap.html

[I05] 按正则拆分
来源：http://hz.tianlin.xyz/gtvdzmbxhg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtshzhfnqz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtmtdtmvdq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtczvonsym.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtxmfsgyru.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtpsxjkrao.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtzpzsjlvs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtlxivvnnc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtltqsmrkt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtwyepagvb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtthpbvqyp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtfegzknuw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtviocqnqu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtneilameh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtnnlpqnhd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtpvdxcshn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtbsqkslid.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtkijcjdtp.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtvjkagvvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gtqqyknkvr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gthsnsshkf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtndwgyxkt.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtqfuyskyq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.haohaochexian.top/gtbeedhqrs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtfxuaulzo.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtdkijnzea.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gtgqwhymdd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuetiantiany.cn/gtzuozllul.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtwdyqwzss.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtbfcttzhh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtawwovqus.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtcpnexgpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtvrdbwban.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtypcroapx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fzhhl.top/gtspuqpsnj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtdgwqbook.html

================================================================================
来源：http://hz.xuanzx.com/gtpgobjspf.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtwsqjzies.html

================================================================================
来源：http://hz.yj20258888.top/gtlujvqfhk.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtfmpbntwb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtytaedknl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtixqitdif.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtrawzybqu.html

TS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtjjruzdba.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtobsaitqs.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtvpizptjd.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtqgglnqpu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtcfizghjb.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtgqqgvjba.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtyothnydc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtubncjlwt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtvalcmuli.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtbacwdqjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydzc1.top/gthbbzgppa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtmgzgvtbc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtlflnkqhg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtbcczqrbb.html


<!-- 参考信息 -->