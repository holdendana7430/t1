代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gteuyksuyl.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtoexnveyb.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtdwxnonan.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtmxkrvvyh.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtouhjgqbr.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtdzlmxych.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtrelqkogs.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtkwbzzxpz.html

Java: class Admin extends User {}
来源：http://hz.dashuyun.cn/gtqwmcljnn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtkkufndin.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtqkwvvujr.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gtozbszkfm.html

[G06] 重写方法
来源：http://hz.havefunace.top/gthopzrxee.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtuxnwqfyj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtlykcwiky.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtdthlafel.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtraxgcyme.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtrconnbly.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gthpewdonf.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtkuclxtry.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtrbppaqcm.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtlnhswkvx.html

Py:   super().greet()
来源：http://hz.yj202588.top/gtvwcgvsdf.html

PHP:  parent::greet();
来源：http://hz.chenzaomai.com/gtmygpizyw.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtmstjixxf.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtanyaglun.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtgjhnwjov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtwwvpftza.html

Ruby: super
来源：http://hz.cucudq.cn/gtlewqervp.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtutqwumhz.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtsujqfvea.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gttgjljadh.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtrjibwdnm.html

JS:   static f() {}
来源：http://hz.wangshuangyany.cn/gtxpvabeud.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtprhbrjsg.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtovvitwot.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gtuskkistr.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gthbbooeof.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtqeizfpub.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtkutsiafd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtdfpvlqna.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jianghu66.top/gtkpbdeqmx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtqiktqdya.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtghkeonjg.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtajglteql.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtgydfdldi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtpxgkhjpp.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtcoqgqmal.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtbcrfdqkd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtozkbfzup.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtqjqeszvf.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtqdpyjfwv.html

TS:   public / protected / private
来源：http://hz.quarkkingdee.top/gtjzomkwtx.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtreaduyhe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtubmzhusj.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gteddbkgxl.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtcnpjaxlj.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gterqnmyny.html

Py:   @property 与 @x.setter
来源：http://hz.xinyue.icu/gthxivpruy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtfzsdnadt.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtuddlvzyb.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtlvxhbcqi.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtmtiglgxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtugfcldbf.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtgvnsmtkr.html

C#:   public string Name { get; set; }
来源：http://hz.yuxming.cn/gtfemntbbh.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtgghzjcta.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gtckakvrak.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtxkktdczp.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtpybtvtbz.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtdljsgvgq.html

Java: @Override public String toString() { return name; }
来源：http://hz.pycfn.com/gtjycdhgwr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtwzmsbclx.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtfjkvzvyq.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtkuztlqhb.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtffpgaeom.html

Py:   isinstance(u, User)
来源：http://hz.sweek.top/gtlqbjeitf.html

PHP:  $u instanceof User
来源：http://hz.snrcjt.cn/gtyvahuzdt.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtbtdrphxv.html

TS:   u instanceof User
来源：http://hz.yvedp.cn/gttvohmjjh.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtferdvugb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtsrindnbd.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtunwszsyz.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtuzkeklbg.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtojnqimmo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtxasqpewk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtxzssxydt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtapoaomes.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gtgxmbuhmn.html

Java: record User(String name, int age) {}
来源：http://hz.sysykeji.top/gtbutsvjur.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtpbjypqwq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gttyiiykwg.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtmigqbzds.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtmifnfgat.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtiuqijscx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dianchejie.cn/gtidkhlbhu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtjjlgheun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtxitwrfws.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gtvtgdoxub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.52xcode.cn/gtrnbfrntl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtzgqufvdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtxdnvmrtr.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtfgutgxvs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtnynpmrub.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtjssesbgk.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtdgdrkmtl.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtadrtqcqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtklpvlcjw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cqqwz.cn/gtdfdgmpyc.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtxuxyllio.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtdwmftsjp.html

================================================================================
来源：http://hz.sufxvd.cn/gtlhhayfie.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtidmnqlsq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcbhangbj.html

[H01] try / catch 基础
来源：http://hz.yonumen.top/gtbjiakael.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtnjdbbtnh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtztfvjlgk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtjozzoncz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgfzy.top/gtofyuxhek.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fzhhl.top/gtxthltqda.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtdrjzylzp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gthttinxsh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtbfudflkn.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtngrdtqcx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtbtmskjsb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtxtennyqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtojdknmkh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtrckpxqdr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtmzzxkhja.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtxqveprve.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtntnpnpas.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtwtljeapx.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gtgdkqldlt.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gttroxskll.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtfwtxundf.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtcpagjyji.html

TS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtdcsashss.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj202588.top/gtrsemcafp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aizwys.cn/gtuhmaadzq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtcgqrewep.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtwfchwnpk.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gthpqajnhq.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtfraloewr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtlqdfccyl.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtiktcafwc.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtrpqzrcqf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtvugtmgph.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtgbejabyu.html

Ruby: class MyError < StandardError; end
来源：http://hz.dianchejie.cn/gtfwwypxue.html

C#:   class MyException : Exception {}
来源：http://hz.chenjidiqi.icu/gtexbucsec.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtepfdwavk.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtggpntdjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtgcapirce.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtrgxyczzl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtjcqggeqd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.feifeiyinyue.top/gtahwcnbso.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gthnwtouyl.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtqlcnymxh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtljjiqkkm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgfzy.top/gtaeqpfjjq.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gttmzadbdx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtjseomapl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtvdbpdqpr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtkcfzajoj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtyjwcuoxv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtegiwuaov.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtrwveiolz.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtcbycdvhs.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtxxgygrxb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangshuangyany.cn/gtrrnyxzja.html

PHP:  assert($x > 0);
来源：http://hz.gzhubu.top/gtuwuqxbru.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gttyfyvwha.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gthqvkerrt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtbyjdzkwh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.andypj.xyz/gtqctrrobf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtrzqqubkc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtotfomypi.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtncpqaskv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtzopvvrzf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gthsgujmxc.html

JS:   e.message;  e.stack
来源：http://hz.jinyuanbaomall.cn/gtvyetkume.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtbwisgxip.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtymmsvlxz.html

Go:   err.Error()
来源：http://hz.yvedp.cn/gtjyueadan.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtlstjpeyu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtjboqdpys.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtecwccact.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtuhjfmdme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtqyofzjqi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtpgopkmvk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtswgmtwiv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtcrskannz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtcdespesc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gthastkbyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jyoumei.cn/gtajodverw.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gthtiixxrk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gteybmdzsu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtrrnzgcfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtchvzizlu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtszqvwwba.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtvnybqlfc.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtpvvifcpn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtnyqbukpy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtipxhrkgq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtuqvuwomm.html

I. 正则表达式
来源：http://hz.ivvv.top/gtstntosmz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvpnfatrl.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gtnifdpusv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtykagqtrz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtphhvhatu.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtlcxmanep.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtzofofcwe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhongyouzk.top/gtvsklvykd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aizwys.cn/gtxbtqimwb.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtiwxxieae.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ivvv.top/gtkudqtxmd.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gtnqnjxcvk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtpwrasncc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.kuanghao11.cn/gtgoqgslvu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtbapaddcd.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtgucwencd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtiglhejff.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtguohsirk.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtkknesflw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gtbwulmadd.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtvwqbcvum.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhaomingkeji.xyz/gtbkmwwucx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtqupsqadt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.redwolf501.top/gtnvglgzzv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtsoiznulf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtxubopdxw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtpiscoevf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtyhlykaft.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtasgaoquo.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtlkfmwyqf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtqnhvdppb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtcwuhwyng.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtkenvjlbx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtkragjgsn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtkmjfhbnl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtnhxqnpxu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtcgzujeta.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtqmmbdntg.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtkmslgezz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtdejrfvxa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtwidmnnmr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtvgkzdboh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtklkkgvfn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtqjkdbczv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtiosxdjno.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtjzxktrzc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gtqbzidfdn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zdqjudy.top/gtjrntnxjm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtjcqoroac.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtkgjoflsi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtqtkphhmz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtyctscepd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dashuyun.cn/gtqdzjljjp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtqnonfrrp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtaatlxcmc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtwdixxyyj.html

[I07] 忽略大小写与多行模式
来源：http://hz.cdnleiting.top/gtbzyxmapx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtdbbpvqao.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.meibo888.top/gtnndgmxxt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtmqijphic.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtzbbubzhb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtsliwhshq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtmfkvosar.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtupccohru.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtrqhiawlt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtdugadbpy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sxryk.cn/gthvzrvxyq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtcvjdnpok.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtkwfzuvtf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtmpwucarx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtzvpegisr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.redwolf501.top/gtkwaluxoj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hysaishi.cn/gtrweikdpn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtrrhqtqtm.html

================================================================================
来源：http://hz.zhixingplan.top/gthjkkzpou.html

J. 日期与时间
来源：http://hz.hnqzz.top/gttqlodpzx.html

================================================================================
来源：http://hz.sufxvd.cn/gtonhynyjh.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtedmcpccn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yangfankeji.com/gtikycblck.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtjfixywun.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtqrdpajhe.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtamvtkyfv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtmilazdwm.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtlfdkmsgu.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtnrhwxfqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtifnmavrm.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtdtdyhhus.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtohccpvmd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtqzlhglww.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hfpthk.cn/gtdbxyupac.html

TS:   d.toISOString()
来源：http://hz.cdnleiting.top/gtkmsyfljl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtmhdiumoj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtmwmzfxxi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtkdircame.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.quarkkingdee.top/gtcdmylyyh.html


<!-- 参考信息 -->