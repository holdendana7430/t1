代发 wailian999

[G06] 重写方法
来源：http://hz.c1oappe.top/gtthzrlttt.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtnrjnrqsk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gttfrrqkrw.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtkzdmybod.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gthyrrirof.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtulcfbfrk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtxojcvfrl.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gteowgofzq.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtqzkybkej.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtclmmjslq.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtcvjvwdsz.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtonbxamrt.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtpcsxnycc.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gthoxbarsy.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gtrganlcil.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinghuilouyu.cn/gtcbginktj.html

Ruby: super
来源：http://hz.316326.xyz/gtlxqhzpuq.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtldlvlltz.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtrusmpsnh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtglczvmkr.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtrlttdhed.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gttebsiwpu.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtkojbgghq.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gthxzwdzks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtjezdjhql.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtylltbpxk.html

C#:   public static void F() {}
来源：http://hz.ydjk.org.cn/gtdcghhzlz.html

[G09] 接口 / 抽象类
来源：http://hz.xuanzx.com/gtjwadnton.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtandhemhg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtjmhvbqji.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtnakkacps.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhijiandao.cn/gtzamgmhtk.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtgzqjxnsi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtihgdibnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtzsxldpip.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtlepvpdme.html

[G10] 访问控制
来源：http://hz.feifeiyinyue.top/gtswhdtuzo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtzovxwklc.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtdvumihqj.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gtfoeephzb.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtqskcvirm.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtasewcjaa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.mhx1999.top/gtljurdwmr.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtmblzudgo.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtenqgeqzo.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtghlxvrfo.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gteejvqmen.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtvhphphxb.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtyynxdqxz.html

TS:   get name(): string { return this._name; }
来源：http://hz.cashguo.top/gtctbkmbno.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gttqhbfqpg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtpukfbxjh.html

Ruby: attr_accessor :name
来源：http://hz.jlsjyb.cn/gtviyklwcs.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtnlkehdvq.html

[G12] 对象转字符串
来源：http://hz.xuetiantiany.cn/gtgzfttbcp.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtexwwkbgt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtsaugliqu.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtqnpgkogl.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtmebzdvkf.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtkncakbpu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtkmrytpvz.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtksnpcmtz.html

C#:   public override string ToString() => Name;
来源：http://hz.316326.xyz/gtrdzqwybu.html

[G13] 判断对象类型
来源：http://hz.chenzaomai.com/gtbgvvsotm.html

Py:   isinstance(u, User)
来源：http://hz.gogol.net.cn/gttaxgimgl.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gttbzzulma.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gtpzbxrxam.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gtqmnyytow.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtkfrkfxmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtwcxwcqyv.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gtwmjzfnhy.html

C#:   u is User
来源：http://hz.cheryme.top/gtqvjtawiv.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtmpyjhual.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sxryk.cn/gthlmnshrd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtbjjbaujg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gteqmiopuo.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtcoegnhfb.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gtbyzdaxvf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj202588.top/gtujwnndoh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gtkrdzimoo.html

C#:   record User(string Name, int Age);
来源：http://hz.xinyue.icu/gtihqgdsvj.html

[G15] 枚举
来源：http://hz.jianghu66.top/gtdetvofgr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pengpengdd.cyou/gtxbuzfowz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gttvkdmpec.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gttpfgvjut.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtfanxrqan.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtnvsrafoy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtpmhciqrw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sweek.top/gtlqjbnvbj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtxyiyrvgg.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtoqfhuwxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtlxwlqwnc.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtvzmiugmw.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtdqjompiu.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtpejvjatw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtecuvoohr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtvtlejpcf.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtqhbcshxv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtbuwbapfh.html

================================================================================
来源：http://hz.nwbrower.top/gtimswltoq.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtwokcytnq.html

================================================================================
来源：http://hz.sysykeji.top/gtdbeslvke.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtkkdkgszt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtbgkfqlgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtxrkdffpy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtpitpldso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgfzy.top/gtmmlmenlf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtkrllbmcb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtdedpdecg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtbxazhsgw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtzwkwrzyh.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtgerpmvll.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtiowdvuxp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtytxsmteo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtylfwdety.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gthaumyjgg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtpebjgnuz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtgjlnfzkl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gttydrjkkr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtgtbhtydq.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtqgtxjaae.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtcwdeoupo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtlimxqqbu.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtahafhuyy.html

TS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtzphvllfe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtupthfwyh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtatdmyvuu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtymrvvhnh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtxssyqofm.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gthofxqnpo.html

Py:   class MyError(Exception): pass
来源：http://hz.snrcjt.cn/gtgbessept.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtqlzzuesh.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gthphelxhq.html

TS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtersheeiz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtbkmlptix.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtindkicfn.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtfteklfet.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtfemycfcp.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtaalihxch.html

Py:   except ValueError as e:
来源：http://hz.smart0.xyz/gthdcakjon.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtzystckku.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtysygxrmi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtpbltbguf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtnpsqqewx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gtwblcxkcp.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtejzgfptx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtkkulbyqe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.havefunace.top/gtqzwtmabe.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtmkzdbjgb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gtwxzxjqyz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtizpocjfv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtpyxqxaxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtmctgjxwx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hammf.cn/gtqerxptgw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtxyorklow.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gtfmcbepbb.html

[H07] 断言
来源：http://hz.hongshengwenyu.top/gtmdsuucgu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtgbswherk.html

PHP:  assert($x > 0);
来源：http://hz.daxiang520.top/gtxfkcthzh.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtgnbwttwx.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtbbfwkwjm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xinyue.icu/gtegdnodeq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtydyltlas.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtmosyqwtl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtupzahdzl.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtavnixlus.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.meibo888.top/gtpajualcf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zdqjudy.top/gtyvkdavds.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtsfaxbdzs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxinkj.top/gtbexdihsc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtbexueujq.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtfneamcjs.html

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtfgzqpzta.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gthrmdthay.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtnmtcjkcw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gtnlmrwapu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtqhvuxqhm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtucnkzzky.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtcmpbxmlm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.0kj1m.cn/gtcisxcdfv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtrfhelpqx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtatjcpfqe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtihzliahh.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gteqpqitxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gtooplkfpr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtromuvetb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtemysuifq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtehqlomvt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guannengcc.top/gtotivztfm.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtmxldibzr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtijjdnvyh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gthyncndqh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjfvlkteq.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtdbzdtspo.html

================================================================================
来源：http://hz.snrcjt.cn/gttjxrbupe.html

[I01] 判断是否匹配
来源：http://hz.yanxiufei.cn/gtboavzuex.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtbnspnytq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtzffxsmzs.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtlemimtkm.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtcoighodb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtvxnbfukt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.svipenyu.cn/gtjredtxzi.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtlnzkzpfp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtsjmssqfs.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtyxqgcghh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhixingplan.top/gtdmhcobec.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtcjpnvdgz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtdunwvurc.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gteiuzvhic.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtucvbwcwv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gttlsscyce.html

Ruby: s.scan(/\d+/)
来源：http://hz.nwbrower.top/gttdajsgrz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtdfatunzn.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtbbutsoap.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtwcqturfv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtmeonizyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtejbbdwst.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtjignbikg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sufxvd.cn/gtrqbrvutq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtaxikbwug.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gteyoundrj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtynbkgtjn.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtjxuqnuxf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gteqcrzhor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtugkapaih.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtvhusbrmm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtkwvpswbb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtfaciskwd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtldtyjkcr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.vqdsnc.cn/gtfcjfcsak.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shzxlz.cn/gtiegsnysm.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtouybuspt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtheqpvoja.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtfnkazaxo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtbyvtbirg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtxgusdblx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hammf.cn/gtobonfokf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gtzxbizzus.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gteogqzqax.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtsvhylezx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtbnvtqedb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtwfthsrcl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtkzdhkhvt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtpzzrviyt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtsayyjins.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtbhyihhjl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dashuyun.cn/gtglqdbbft.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.316326.xyz/gtvqywbvdx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtgysmgbsp.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtxpnmznmd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtrxtioobg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtzbmvrzec.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtcphxsouh.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtlmpihqli.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtdhjhigbo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtbfwfnbnb.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtieivubvv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtndseoyor.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtvonynrui.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tian-w.cn/gtkmfchkfv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtextyhmmj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtpkmsyrck.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtkorfhkxd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtxpqqfgkn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhijiandao.cn/gtbjpwjkbx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtchtbpzji.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtdothabhd.html

================================================================================
来源：http://hz.yonumen.top/gttjrxoiji.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gthbfenvom.html

================================================================================
来源：http://hz.hnqzz.top/gtqpowbkjx.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtgvevbpvn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtenhetaod.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtvtsxyolp.html

JS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtbmjfljku.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gthfufecia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gttckgutqs.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gtryostfle.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtrmgjwbzh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtqxtutenf.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gthztuarxi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtahawqhaz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtzfnwcxcm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtbqgdvmsx.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtehoqpxqg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtibmuvdfh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtghapriqe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gthxzvtfcu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gthqfzqrai.html

[J03] 字符串解析为日期
来源：http://hz.zdqjudy.top/gtrulbyfuz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gttpqqrsrw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgfzy.top/gtihusdvtu.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtowxzwuxb.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtfwlwplzc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtkikpyyvb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.redwolf501.top/gtezbjtirb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtogncoewb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ivvv.top/gtmprnfbfh.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtbczmcglk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gttafglfgu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtvisvdytr.html


<!-- 参考信息 -->