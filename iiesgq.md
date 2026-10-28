代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtapmpyphu.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtremdhsth.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtmzicsbmg.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtfkxkyffg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtggvqkzlx.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtiriphaaa.html

C#:   public string Greet() => Name;
来源：http://hz.zhijiandao.cn/gtxwhniyrj.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtpjmodqct.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtvndzqfyj.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtqqvzqcbe.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtrakuxyih.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtqkfwmrfw.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtiouwimbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtlkfhdeaq.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gtstrjdxzf.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtczmejpzf.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtusfdkxpm.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtpalagpqh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtrgawiwyk.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtsmdnxxna.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtmeguatfy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtjcpydkph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtqdtarjai.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtrfquafjc.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtrdhtijkh.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtpyncoifz.html

Py:   super().greet()
来源：http://hz.xuanzx.com/gtuyyulojm.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtctwehdqq.html

JS:   super.greet();
来源：http://hz.nanxuanxn.top/gtkxrlvbzz.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtxjbzpgzr.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtxfzurote.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtrplrtwid.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtxjpdjubz.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtfjmnwuom.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtgtdrqnco.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtsmachzqe.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gtvczvhrnl.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtnwdlzfqj.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtxxztlftg.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtpzvfbskq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtnqunkqlp.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtychvsibr.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtgijlhsvj.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtdbzksneq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtylkdtktp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ehwqpu.com/gtdchjjnef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daxiang520.top/gtovlygpjt.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gtojnbrfvo.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtbeyjrbty.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fengsongda.top/gtebyjijnw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangkeji.top/gtzqrysqpb.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtbukubzef.html

[G10] 访问控制
来源：http://hz.yonumen.top/gtxfnoqhpb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtgmypwbag.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtwndevuvu.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtdwqmcfgl.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtrewxtlcp.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtmwybryzs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gtxigwcyje.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtxmrvqdji.html

C#:   public / protected / private / internal
来源：http://hz.hongshengwenyu.top/gtjhxhrefe.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtfdcjvtui.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtaeqzheiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtsaftjvdz.html

JS:   get name() { return this._name; }
来源：http://hz.pengpengdd.cyou/gtvjrhlkzs.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtqexgweep.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtcbrhxwwe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtsvavprbz.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gttsuvqert.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtnnstixvv.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gtifziedrk.html

Py:   def __str__(self): return self.name
来源：http://hz.shuidangran.top/gtmmtyazif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtgtczauhw.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtvomxzapd.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtrgoybxfk.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtroxeedki.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtlkmpqune.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtwveqywas.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtopvilrgb.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gttucmmtwj.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtneydjbvh.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtuxeochpx.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtviokfilx.html

TS:   u instanceof User
来源：http://hz.jyoumei.cn/gtytcomngn.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtvwkpoqtn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtvadlvlvw.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtnqecqnzn.html

C#:   u is User
来源：http://hz.zycfv.cn/gtnfganaqu.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtsjqsuqej.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hammf.cn/gtfvwclbiu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtsputnivf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtyjqmobwn.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtotechfnb.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtrmremzlm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtiiegerug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtqiurhgqi.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtplxhsbdh.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtehxruaji.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtbqexqjqe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtvmgniwnx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aibaodan.cn/gtmvhawjwz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtqcbdtbxc.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtwwzqefda.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtrfjteolz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtsrpmjnic.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtdzrwzezr.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtnkgyafqk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtgkpiqfwj.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtlxaxoknl.html

JS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtephellys.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtqlbaigjd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtgmbtcntp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtefvngzoj.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtubdugzpo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ivvv.top/gtfbtzfvsk.html

================================================================================
来源：http://hz.nanxinkj.top/gthftedmti.html

H. 异常与错误处理
来源：http://hz.hysaishi.cn/gtjdzkxlid.html

================================================================================
来源：http://hz.wangdashe.top/gtqtvhpqvm.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtqvycczvh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtutueiawk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtlalcewrl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtbkswcvwh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtxbfriylh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gogol.net.cn/gtcuysephh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtpmwgnnxs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangshuangyany.cn/gtggekifkb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtbiqaycej.html

[H02] finally / ensure 收尾
来源：http://hz.52xcode.cn/gtgxkrlbft.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtttbszqod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtpnnzucga.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtygfftlrp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gthfhnsmto.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtbndpvxyz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtqdxscaeq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gthscksnop.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtppermoey.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtumrkkijb.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gtkewdjfql.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtmrbgguit.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtyozdozel.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtxhctwipx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtkmrgfnlc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtoehueigx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gtnsnaefsk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtbmhfaxut.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gtygygtxfn.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtfgvgpeij.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtjelvkswm.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtxzgnnufp.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtbawczwxk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtucuhrtac.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtwwslcuvj.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtsjukkxgo.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtbqosdlxk.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtxplcyeuu.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtxuizdnjs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gthfzmyltv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gttufgmuoh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtdzusmsxc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtfxjaovcm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtwszcddsn.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtvimrddaf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtxtsdeoib.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aizwys.cn/gtvbdmnwas.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gtgdbrvjtd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtiyrmiisy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtxsqdhire.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtbukdwira.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtjbomrrkl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gthzfgruvc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtgvsencvj.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtwkusnylx.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtqmkxbfau.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtnmsfhznk.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtqfvskffb.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtkhxhllix.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gttvsrmzwu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gtrkcfixvk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgfzy.top/gtabqqysnj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aibaodan.cn/gtzkayaqnc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtekltkhut.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtooywvtef.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gtzlnktodh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtwksgidkb.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtblmfcmld.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtebmcdxyi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtmnqmvatm.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtzuwcgcwa.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtcxbkqqbh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtwiyeywdq.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gtuxgalzqm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtybqtddcz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jianghu66.top/gtyaxnwehx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtkzlokulv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtgosvtlnf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtwthqnwqj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtcaptybhf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtilzjhnpz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jyoumei.cn/gtfokvgpuj.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtcemmhwvx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtbnmxgbfq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.snrcjt.cn/gtmckttfki.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtizyjgdjw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtemzkaijy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.smart0.xyz/gtbqrdwxlg.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtznwgddfk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtgvejychp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hfpthk.cn/gtnivrshfv.html

================================================================================
来源：http://hz.bjfxy.top/gtszivhony.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtdtitgror.html

================================================================================
来源：http://hz.xziqi.cn/gtskrcarll.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtzmadwlej.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtnngfymxh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtiyldwygu.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtdsacigjl.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtmbjyudmm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtdvlvjcqr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtrjbntsst.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtubikownb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtkfgetttd.html

[I02] 提取所有匹配
来源：http://hz.andypj.xyz/gtajcezrwb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtnefvijeb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhengqikj.top/gtagpcktif.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtqpgfimwb.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gtfvccwcxf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtaaicqovi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtadzwwmfq.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtwsppvekw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtbvocjqej.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtjwjnoyyo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtiukaobof.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtamztlyrt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtamostvof.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtwajsiixm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtdgypodvg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.andypj.xyz/gtbkyakpub.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hongshengwenyu.top/gtfyfzxedp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtdaagehgs.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtijrazkyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gthrrejtae.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtkuafsbce.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtahoibhzn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtdkrbtgyp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtkjoaywbm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtuekevqan.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aizwys.cn/gtrvljgdkx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shzxlz.cn/gtyfdndodj.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtrdaebtdz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ywan-chungtsiang.top/gtkwtpgkrb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtbzcwomjn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtuhcgigbj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtmbsqekth.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtcivzaitq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtsxljiymg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtsrkvwqpm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtmzklqbbv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtmpkgltka.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gthavfsuha.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtfhokpafc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtnsforbrc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtousrhbxo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xziqi.cn/gtypageftq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhijiandao.cn/gtjgupctdm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtxuwtoini.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtzhpmbyun.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtvvzvlasw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gttoapfrzz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtjdvlvmwl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.feifeiyinyue.top/gtitnfupgg.html

TS:   /error/gim
来源：http://hz.316326.xyz/gtlwnrgewr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtaejlpwxa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtedqkssnb.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtrajayjoz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.haohaochexian.top/gtgfizlqpt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gttzhwwyqc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtvmoovwtn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258.top/gtoadzacge.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtkqwylphi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtwsytfyki.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj202588.top/gtkqzxeltf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtirqrqfgf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhixingplan.top/gtojhwhwys.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtrbuluqep.html

================================================================================
来源：http://hz.tanke756.top/gtshurvuqv.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtsnzcfggc.html

================================================================================
来源：http://hz.ybcxt.top/gtejonbixp.html

[J01] 获取当前时间
来源：http://hz.wangshuangyany.cn/gtatdflpsi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtodszxxuz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtdcjpqvcu.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtfjxrtfrk.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtescxniwg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gtncdxiakg.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtayswqopi.html

Ruby: Time.now
来源：http://hz.tanke756.top/gtcgrlsojo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtrguxhjsy.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtsuajzsvx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtzqpblofq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtvzlcisoq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtcygtrmqo.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gteblrudls.html


<!-- 参考信息 -->