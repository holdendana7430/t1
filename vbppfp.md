代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtunvaxxtg.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtrzzglmrc.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gthmtcdihe.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtnahsueiw.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gthlaqxxux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.bjfxy.top/gtypjiwfda.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtaxajhbjr.html

C#:   class Admin : User {}
来源：http://hz.jqgufenzy.top/gtbkholshc.html

[G06] 重写方法
来源：http://hz.sweek.top/gtliexntgu.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtcnonuxvh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gthawaunqo.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtympgejdm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtvatundyk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtxfjxlfcz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gtslrnukjz.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtqhtqaipx.html

C#:   public override string Greet() => "admin";
来源：http://hz.feifeiyinyue.top/gtsdztowvp.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gthulecqog.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtfwjyngpv.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtngkrxdry.html

JS:   super.greet();
来源：http://hz.cdnleiting.top/gtknsgikov.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtjnzmuncy.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gttzhcxfxb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtcurgltir.html

Ruby: super
来源：http://hz.guowangkeji.top/gtnkxyczxq.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtnjrekkqq.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtfqtmvnbv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pengpengdd.cyou/gtkvahoxqw.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtfzzdmshb.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gthkszjbtf.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gtgdiubbvi.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtptcyawdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtuzdfpcue.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtgkzwctca.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtunpaipcu.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtmskdnich.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtxwkeymnc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gtecvtmdgv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtksdaklwq.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtnmqfocaf.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtsnppclrp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtcpisfvrp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtsombxebz.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtralcruku.html

[G10] 访问控制
来源：http://hz.zhoulong.xyz/gtcfltxpvk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fengsongda.top/gtpbyxpbmo.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gttfqvgfbn.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtqkaoldbg.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtwiznlwxm.html

Java: public / protected / private / 默认包级
来源：http://hz.yonumen.top/gtpvjjikxg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtojklomcp.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtxeextwck.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtbxcddfov.html

[G11] getter / setter
来源：http://hz.pengpengdd.cyou/gtnsqnluyl.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtiplojuxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtrlslbqxz.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtbjohiqla.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtbkohirqn.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtduhebkns.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgfzy.top/gtbayarlhl.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtlfrkxcdn.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtcfuawlif.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gtcjmptzjr.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtdujotapz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtxxdsvddv.html

JS:   toString() { return this.name; }
来源：http://hz.sysykeji.top/gtcvxpbtts.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtfiphjaer.html

Java: @Override public String toString() { return name; }
来源：http://hz.aibaodan.cn/gtgkpvbnii.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtabjeygoo.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtvjhxjwep.html

C#:   public override string ToString() => Name;
来源：http://hz.hnxiangtu.top/gtnoewnjje.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtgkpsqocj.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtzsogksxg.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtwgbfnnwm.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtngcpruet.html

TS:   u instanceof User
来源：http://hz.cqqwz.cn/gtdynhnvqi.html

Java: u instanceof User
来源：http://hz.sxryk.cn/gtsihvrsmk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.vqdsnc.cn/gtmafykdon.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtbqsapzjx.html

C#:   u is User
来源：http://hz.havefunace.top/gtpzgohwlm.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtzpgvfjjk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtcybohxah.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtmtsrksgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtyturostz.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtndooeuds.html

Java: record User(String name, int age) {}
来源：http://hz.gaohongyu789.top/gtutmritkf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtnmzvugih.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.kuanghao11.cn/gtjfltrpkr.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtssfvwnez.html

[G15] 枚举
来源：http://hz.jqgfzy.top/gtkccanfja.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.redwolf501.top/gtykmokrea.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtstgfuige.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtyxfobwhj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gthpeiovhw.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtjcmzxhum.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gzhubu.top/gtaroitbaz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtptpxairb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtiffjslbw.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtfdbyowxq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtcuxlnnyt.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtalquamxp.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtbuyyoubt.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtzuqvhhhs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtaiodkdwc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtesztkcto.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtmzyqcjvf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtarrsgwfe.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkslpdvxo.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtdlyszacg.html

================================================================================
来源：http://hz.sweek.top/gtbpnvgxgc.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtuvnblprx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gtnofuxnyl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtsrbakevk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtjqerbqnm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtvgofobnz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gttgoggamz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtbaciwtml.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtrqmulvfg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtsuulbmdl.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtjpohknbn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtsvdmywmn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtgpebbdot.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtvnkjpzhp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtmkskfchj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtdluszpyy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtlbyroizp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gthfrwpfhd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtxuazyvna.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtxubmioth.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtwymexrsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtaelbifxj.html

JS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtcwqvadwz.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtcvlnjhwm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtikvtrhmu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtkxyzyhjt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtubsnwyvs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtiwyfcohe.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtiusgtqra.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtldwmqcbf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtyqmrtvyd.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtpzndghpj.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtsugllxja.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtphoetiot.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtiyxcwenn.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtsvcmthqf.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtmxvlhhfb.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtxccgluva.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtmgyykjjm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtuahmmtyx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtlpzzgwfx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtxvtvlehx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtnndluwso.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtlfikwuoy.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gtrujrgkej.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtyswnjrhj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gttmbhcxed.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtkwhesaif.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtrxburnjy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtbyxlmnpn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtbkgngzeh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtquwxiqqc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtoqhagxid.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtkwzsvwkj.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtyoqsasfu.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtwonrnnrv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xinyue.icu/gtlhblwwko.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtdouqozyg.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gttpnktypq.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtsjadsuyw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtohrfxfie.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtcgcdpsho.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtowlyilsy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtaehsbbqs.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtexvsicwn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtlxcrxjdw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtfggpztlh.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtxcqgjiha.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtgfrerkql.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gthdfickrd.html

Go:   err.Error()
来源：http://hz.mhx1999.top/gtctiyreqs.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtbtztryay.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtldbisnrn.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtuydyykuu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.vqdsnc.cn/gtvhfbeijd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtswfrcnlj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtnmvmobjl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtkztyjmoa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtwyutullq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtgrmshcxp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtlguhqzqz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtvwgcnqla.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangtech.top/gtejbgnevb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtdsucumyd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtujpqesfv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtxfkgqrwj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtltmjmrip.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtniebjezj.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtrgkakmup.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtpewnmtpv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtnfstwgwm.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbgtuzykl.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtibrhfdll.html

================================================================================
来源：http://hz.cucudq.cn/gtzeaemezv.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtrilmqupp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gtcjawjizi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtxirvzsis.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtjvqfwipe.html

TS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtkcfpptsm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtunkhwags.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gttaoacljc.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtzntbfzhu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hfpthk.cn/gtsgjoakiz.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtuobbjhzb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gthtjakhuf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aibaodan.cn/gtzixmwljd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtvsfukgig.html

TS:   s.match(/\d+/g)
来源：http://hz.zdqjudy.top/gtuoeemicz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtteffpbwp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtjszrpqvi.html

Ruby: s.scan(/\d+/)
来源：http://hz.tianlin.xyz/gtbjzfmsgs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtvjjlfkgk.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtloqtorpk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnqzz.top/gtkauofdab.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gthpcdkksw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydjk.org.cn/gtapycfzii.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtubysrwbw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ppjwa.cn/gtdyuhtbgm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtrwvfrzwg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.haohaochexian.top/gthzwrbcdj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtwvtdvjjd.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtiuytnrjd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtaxhftxja.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtoxiaezjx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtkkratbwl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtfgfpkeee.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtfejjkjna.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgufenzy.top/gtizqjhfbv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gtetpbmqsn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtnihkfuwk.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gthvlkrzmi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtdejhuoki.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtdstkussc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtjgvjnjvg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtcmmjskyz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cashguo.top/gttjbodtgq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yonumen.top/gtydcewbnc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtmufdmiol.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtymtptrcn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gtehoggqmm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtdzhzpoyx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtbeumkqch.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtmdjvnjch.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtgbfhzjub.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gthwiobnpq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtsjnaygxv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zycfv.cn/gtdhkpicjh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gthxdaqapn.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtysgebzao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtglgluqtx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pycfn.com/gtvvzgdodi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtmjdzqojp.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtfkrvxwje.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gthvpsdtyy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gtqhnclvhj.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtpmdyyses.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtitoogakl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtsmxvohjw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtenfzbjyn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtobehpzds.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gthcodtedh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtjyvtfiua.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtbggrvhqi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtjkyyuavr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gtnlpdgjko.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cashguo.top/gtarnjgutz.html

================================================================================
来源：http://hz.cucudq.cn/gtyjbaujtm.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtrfavamgv.html

================================================================================
来源：http://hz.birdmap.top/gtrbutntsl.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gtrdqvhlwl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gtifudqyut.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtvswezknm.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtgqgjrlfj.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtlupwobpw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtbvxibjzn.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtpgphcplr.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtlyewdjdx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtbvzhfbkh.html

[J02] 格式化输出
来源：http://hz.9152youxi.cn/gtbnvrjnie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtdtomcdpb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtuayompkl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtfhxfpqhe.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtoqzrmajb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zdqjudy.top/gtvgagegek.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtjlrfdjgz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtkgqdkgsu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtnecwcfyh.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gtveagsavr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtqkqoyhol.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtxzrtnmyt.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtbrayxeow.html


<!-- 参考信息 -->