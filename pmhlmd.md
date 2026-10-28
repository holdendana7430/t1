代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtvjxfrwyd.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtwnvejiym.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtlchzrygs.html

[G05] 继承
来源：http://hz.yj202588.top/gtxbursncv.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtwlaxivah.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtlaxohysg.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gthfkiwlar.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gthnxnihxs.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtgtlmvzke.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gthzsjioue.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtiavucdhn.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtixxnwrkz.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtmuamdhjx.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtpgzqtjwt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtnoowgjnx.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtdwmgolzo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtfzzinsmn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtpgchmjai.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guowangkeji.top/gtgbfnpvqz.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gtygwoptpc.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gtvmxruzyj.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtdnrqdixi.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtzsprrehs.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtftiopbsw.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtszwzunad.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtblejjvpt.html

Java: super.greet();
来源：http://hz.jianghu66.top/gtjfxoluui.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtjuoqvbzl.html

Ruby: super
来源：http://hz.zhongyouzk.top/gtxldqgtei.html

C#:   base.Greet();
来源：http://hz.ppjwa.cn/gtqrrbeftn.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtajrfvziy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jiagoushi.top/gtajmaiuae.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtjwdzafeq.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtuszsezef.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtbpcvpjpm.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtbanqqclc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtyziqtknr.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtwsditdmc.html

C#:   public static void F() {}
来源：http://hz.ivvv.top/gtgmrbjqys.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtycduaipl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtmixhijjo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtumelnnkt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtktvqldfu.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhaomingkeji.xyz/gtpibiqxck.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gteijngaav.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtkaoflqoj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gthgmznwes.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtsjggemzs.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtnqfcmacg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtarhdafez.html

PHP:  public / protected / private
来源：http://hz.jiagoushi.top/gtlvbubykk.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtlyuahxof.html

TS:   public / protected / private
来源：http://hz.gaohongyu789.top/gtffzdeprf.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtfbzcaram.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtdhkleilr.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtikoxxdyc.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtkinjqjym.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtforiqvql.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gtsjvqsopi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtjzvnkoar.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtnxcjdhim.html

TS:   get name(): string { return this._name; }
来源：http://hz.iojbl.cn/gtdqlogsql.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gttcadrjpy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtoyyzoqmn.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtraudechi.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtpyacnhww.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtaqrfyeup.html

Py:   def __str__(self): return self.name
来源：http://hz.daxiang520.top/gtwhyqhsqc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtvsxquqgs.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gthvagnxwy.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtfrbynjoi.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtgkzokprl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtamvzcmnm.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtiaqrbqdn.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtftiegqfy.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gthqsjspir.html

Py:   isinstance(u, User)
来源：http://hz.chenlongwang.top/gtzwhvmakx.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gttnglporb.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtpgsvdreo.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gttindkwxp.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtaupjlpoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtxjdymwmj.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtmqvwpeft.html

C#:   u is User
来源：http://hz.smart0.xyz/gtdaexyybu.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtqzsosgag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cashguo.top/gtguzbvbpt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gtaqznftmm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gttmiyigjb.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gttwygirhy.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtjixsnkdh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtkslnastq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtyulkakxu.html

C#:   record User(string Name, int Age);
来源：http://hz.sweek.top/gtjpesmbwc.html

[G15] 枚举
来源：http://hz.52xcode.cn/gtzubhvdzz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gttglqraul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gttihiaays.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtjcnxzzmt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtchhawysz.html

Java: enum Color { RED, GREEN }
来源：http://hz.xinyue.icu/gtiljiyllk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtpqxnfcsd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtiifjkkwu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gthvrsqkqn.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtcuuqvfob.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtdzwghsnb.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gttehzyuor.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtxvbvzxip.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtxalbfopo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtibggbpig.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.kuanghao11.cn/gtmggccsbm.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtaigqlbrq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtwkvzmhhe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtopjgymts.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtfcrfckvi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqdsuotol.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtayjcivjv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtbimmufov.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtutrohetc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtexihdxka.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtowijklox.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xinyue.icu/gtcerazrpm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtmbqsyxfc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtyyguyjmx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtfkrcvsyc.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gttmxbnomt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtvorskrai.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtjpfkdnpt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtarooplet.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtuwfjrjto.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtpptdckmn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtufaiitkg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xylfe.cn/gtelxqtyka.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtxhzhszwg.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtonqypcpe.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtcjflnikx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtxmxjekhj.html

JS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtnqmufpmt.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtghirznqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtzvocbkbb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtdahydwzl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gthrhsvmxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtbbzelkgb.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtuxhwiyii.html

Py:   class MyError(Exception): pass
来源：http://hz.vqdsnc.cn/gtzgqlwcie.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtpslrvgmk.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtjelxamds.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtginyzjzj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtlkxsetdl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtctmuvydi.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtctlnwwqf.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtzgagwins.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtkkfsvgkp.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtcbdjdlhs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gtrrldaxnp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtcbtpbmlz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtcnllisuf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtktylwxcf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gtkrqwwnxo.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuxming.cn/gtcqmyyofm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gotoacloud.top/gtryiathib.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtqktwsngt.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gteywvjfqh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.iojbl.cn/gtbmpxfsyv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtducavhtv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtdhruooda.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.iojbl.cn/gtoooezgzp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtlkwtyppg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtptorzmol.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtkwrwloat.html

[H07] 断言
来源：http://hz.shuidangran.top/gtocutwzgm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtmfftusdw.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtfaamumnp.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gttubbxlhr.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtmmfblyph.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtemiyhodu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gtlephhgce.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtcyyiqfpb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gttquvopes.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtcxpdzuyg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnqzz.top/gtrlztqlcf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtqkyjzvwn.html

JS:   e.message;  e.stack
来源：http://hz.nanxuanxn.top/gteothuldy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtkjcoikny.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtextxsdeh.html

Go:   err.Error()
来源：http://hz.wangshuangyany.cn/gtfkhnthsn.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gthvyyxvut.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtzccwntfo.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtwvnyaswh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtiaqquecp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jianghu66.top/gtekxyanbu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtmxrkdggi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtgrsihvbu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtdojwftbo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtuchsxjdg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtyxqqepft.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gtbfdsmdmn.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gtojtfkynz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtraabxkuv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtcsgjxzyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtwugznibx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtalptxzbl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.smart0.xyz/gtjionjkje.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtjczlpnnb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtfnesfttk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtjkgzmwtf.html

================================================================================
来源：http://hz.cheryme.top/gtijzaitfo.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtfbwlszdb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtiwvdyfoh.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gthnxxkfqh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtwxmciyoy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtbzpbnswz.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtmnxgxjer.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtiaxntccz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gteqpsiudy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.meibo888.top/gtiigmdzyh.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydzc1.top/gtvfbsjmnp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtypnvexum.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gtshgngnjr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtymhbhopl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtjcvywsli.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtminhymvr.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtsfvocwoy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtnlwqmmsp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtuwkkkthk.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtfnaeetdf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxuanxn.top/gtowmtfdar.html

[I03] 提取捕获分组
来源：http://hz.zhaomingkeji.xyz/gtyacupfhn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtitxkzeeu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtkvolspbb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cucudq.cn/gtsusclyue.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtstutxbln.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.svipenyu.cn/gtiinwfqnw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtphyvplpd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtqfeeonwe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtoceucxic.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtnzlqdzhz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtaahqrerx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtijmjuftm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtcjkmmmoi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtgjnlgjcc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gteebedokw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtnpfndivc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hammf.cn/gtxldnazye.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtykebhjhn.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtuuqutzyb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtbglhyibi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtrypdjnyw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtyktuitov.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtknoqjifn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtwzvurnyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtlutimqdd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtctibtrdg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtrizggbgn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtejwqosql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gthkyvtxwg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gthxcxbwtf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtjjapllpn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtexxlenmp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtghlwzefj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtgfocjoib.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtvydbqhom.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtkymehyfd.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtpwbyxuhp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtpiicvdsf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtqshhateo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cashguo.top/gtbxrrnuuv.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtqpcfhhqx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.mhx1999.top/gttdtfzruh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtivcbrqzu.html

Ruby: s.scan(/error/i)
来源：http://hz.52xcode.cn/gtraefdtrs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangkeji.top/gtohekmsoc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtfdkhoqoy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtoznoooxd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gtyumzvbbm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtfgdsphvt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtoljksdpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtedwsogwq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtsqibvpbh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtskmbrvmp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtihgdqjkd.html

================================================================================
来源：http://hz.c1oappe.top/gtfcwdjdmo.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtdxmgzryn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyxzqfhnl.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtdqcyvftf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtoseixtpf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtpdkkkqhm.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtjelogyan.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtnpptbvqt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtgoshjccg.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gtulrgfhma.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gttyxgakkl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtuqvqahsb.html

[J02] 格式化输出
来源：http://hz.jinqigufen.top/gtfvfjindv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtugzrcvqf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtwtjacdgo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtlclgthrf.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtgeggbkal.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtmrgjmhyf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtquhgcbjs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtdfclndhl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtfrimihbp.html


<!-- 参考信息 -->