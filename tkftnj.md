代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtaynmgphx.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gteasfwnia.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtudvefdof.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtcpafjfld.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtovurspvm.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtbdkeihii.html

Java: super.greet();
来源：http://hz.daria6918.cn/gtfwpydyrw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tianlin.xyz/gtjganhmhe.html

Ruby: super
来源：http://hz.hammf.cn/gtmhtrsgaf.html

C#:   base.Greet();
来源：http://hz.ppjwa.cn/gtuiymueqv.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtbrvztgwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtkupxpyjz.html

PHP:  public static function f() {}
来源：http://hz.yuxming.cn/gtrearawkk.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtlbraflto.html

TS:   static f(): void {}
来源：http://hz.shangyingyoupin.top/gtwyfoiqdd.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtrcmvnnql.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtonmpslti.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtzhawaydu.html

C#:   public static void F() {}
来源：http://hz.jinghuilouyu.cn/gtwrdpfziu.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtmasbyyfw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtxnaflxkv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtxbrngbck.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtnoszfzgd.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtxzhrqtzi.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gtsqxpfmpu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtyhrlcgfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtqujphuyl.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtqbiymipn.html

[G10] 访问控制
来源：http://hz.xylfe.cn/gtvxkgurfi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtsjxzvist.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtlcivcrsu.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtzhcaonhh.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gtwtivakpo.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtotmlzxym.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtqavytfsy.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtpbrbiisu.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtrizjjjmf.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtxxkrrafj.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gticiabnfk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtjhgvhfbq.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtrpnrzvpb.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gtveszxjmj.html

Java: public String getName() { return name; }
来源：http://hz.nanxinkj.top/gtbhcmucxl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtvingbhhz.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtxhxorypi.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtxiosokhy.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtoarsgomm.html

Py:   def __str__(self): return self.name
来源：http://hz.meibo888.top/gtngvhrnwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtryxnnovr.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtavgdiren.html

TS:   toString(): string { return this.name; }
来源：http://hz.cdnleiting.top/gthlplpwtr.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangshuangyany.cn/gtsiahsgke.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ehwqpu.com/gtkjdaaehe.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtqflzwpel.html

C#:   public override string ToString() => Name;
来源：http://hz.svipenyu.cn/gtypmwexae.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtmyxrfnoe.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtfiuwqqqb.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtcszvumnp.html

JS:   u instanceof User
来源：http://hz.yj20258.top/gtzfuucrhq.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtcfuzqfqp.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtmofikfpf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtecwmflfo.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gtpnpibrwe.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtdrzzwoya.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtdmdhqmlj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gtvqncxgxp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtvarwgcue.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtkpczaphr.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtfndxiayw.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtvjcghfir.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtbmvtihsf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dianchejie.cn/gtanwhmtki.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtzbocenaz.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtdvtmaptv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gthlfybrjn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gtcbnxxfud.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gthdgkygcv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gttzuxwqck.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gthnxoaykv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtuoipqess.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtfugcjnmd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtckhujoxe.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtbohglzrh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtxxoothde.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtifeuktmx.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtsggqknwr.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtjequlxhb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtuplhomzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gthudscvsd.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtygnxnnim.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtlwsiumro.html

================================================================================
来源：http://hz.birdmap.top/gtsipwxrnt.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtoqmduisa.html

================================================================================
来源：http://hz.yj20258888.top/gtwpxfpdjn.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtdqphzsfo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtuehmtajo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtdedqlelp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtrlgqdvmc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtckpkknel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtdcspafzh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tianlin.xyz/gthejwjsnc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gtwtlyaczz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtqutdsqms.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gtvqtryqyn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtrhawjkub.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtxtcjujcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtymbeldmz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtlbtbuzdx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gttrnmjtgk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtxzbkiaxd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigfzy.top/gtiukxjuvi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtzbcfcpec.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gttvvefamw.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtvwcsqrda.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtqjbdfydw.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtsnapztzl.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtkpylggvy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtwlwtoqki.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtwrmmcbwc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtxwlpheni.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtkibegdak.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtdnuvjbdu.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtsdafohev.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtmnacrrga.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtpxfaqwzi.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtpkqphjnu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sweek.top/gtxqtwmnwf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtxhnpfjfw.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtkwopeieb.html

C#:   class MyException : Exception {}
来源：http://hz.zhaomingkeji.xyz/gtplknbcto.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtnrriztrw.html

Py:   except ValueError as e:
来源：http://hz.bjfxy.top/gtztrhvdsh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtezfqpobu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gthcgnimxm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtuvuofiln.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtcmicnlcc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gtuohaignu.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtwmchmltj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtjiexghtp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtvydbtzuk.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtgkgusdfh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtclufgdil.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gttamhtair.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtncfagvsi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtwbpszuem.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtsmopinuz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtawleycby.html

C#:   obj?.A?.B ?? default
来源：http://hz.cdnleiting.top/gtkyuforvy.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtcuoppgsb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gttdpzbojz.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtpzflzaqe.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtvzluixcg.html

TS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtowwrecvf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gttbjysznv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dianchejie.cn/gtyefrqnww.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtlkzdwpqj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtvmnpfiob.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtwdsntjnu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtdxvdsaxx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hysaishi.cn/gtehbryenj.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtnejosghp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtdlldjuwr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtqmfgpxbi.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtthhwvhhb.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtceohzjfz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtifuzatll.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtctthoimn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtymrebdbj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtcaxakoce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhijiandao.cn/gtbvujufvf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtzjbbvsix.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtfskvhfix.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jyoumei.cn/gtvfsoqmbm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtcqjhfevi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtbfppizro.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtngvimjvz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhixingplan.top/gttfldsqai.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtypckhjpt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtcyspojqe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gthrkugsbg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtucramdyh.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtrbqnasfu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtjcafrinx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gteeueyygn.html

================================================================================
来源：http://hz.andypj.xyz/gtcorviblu.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtmfljczke.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkznyizrm.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtsuywelvf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gttjkfpfsu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtaiyrewmq.html

JS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtpxezitcd.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtkcokcdot.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtmnkpcjbf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtnyvtiihi.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtnfwgcaap.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gttohlwrhh.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtpghsrroe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtashylpue.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtmhpnmnsb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtnpfzceko.html

TS:   s.match(/\d+/g)
来源：http://hz.shuidangran.top/gtqyrhxvsy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtizhtpcow.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtzpdzcyzo.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtvhruilxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dianchejie.cn/gthumbfwbv.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtrnmxbfqn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtpkmdylli.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtaewoxpti.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gteqznqpzi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtnzvthlsn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtxloxkbjz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtfcxshruu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cheryme.top/gtstkptnej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtwdyhscte.html

[I04] 正则替换
来源：http://hz.xingfuxueyuan.xyz/gtahcjsyeo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtgiscuyaw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtumpkobms.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtwpehilvp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gthngktdxt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtsflsrzfz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtstscdbql.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtpeuqymvf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtxowsbtdu.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtwamyzbjp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtwcpmfnge.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtwmypgong.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gttpwvqity.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtnvplzfdq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gtimsrhbmv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sweek.top/gtozyttysd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtjnfpamhc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtjtkcumtq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cdnleiting.top/gtzbjwtqkv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gthnefjywy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtwowtifjo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtgxbihuxe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtwiyjsutf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtavicwqdz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtzfxmumfj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gtltztlfsu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtdfrfnuwy.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtwlvoasea.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtiurkpnsq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinghuilouyu.cn/gtelbevfij.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtgyhafggr.html

TS:   /error/gim
来源：http://hz.meibo888.top/gtpxbvuqkr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtryoepzvg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtltldqikb.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtmozqzwiw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtydzzhjpx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtogpnvsjk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtewfnxwsv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtuyobefor.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtaeadfgaq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtzmalxqao.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtmelzytyx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtgegixwua.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtqbfzkgxu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtabwarqjk.html

================================================================================
来源：http://hz.birdmap.top/gtftxrzrll.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtyvclczis.html

================================================================================
来源：http://hz.redwolf501.top/gtdhswfeju.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtzbegyxqw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtoppefksv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gtdummsmrl.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtnaorkmms.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtapdtkgkk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtrnajmxix.html

Go:   time.Now()
来源：http://hz.zycfv.cn/gtoidktgab.html

Ruby: Time.now
来源：http://hz.shuidangran.top/gtcjogbpjf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtppwuuljs.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gtrnlhpegj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtkwypqxzp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gthvrvwlbk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtrlbmgmon.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtfvystqwc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtenzxodrk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtcjkfkbpd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gthcatuapd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nwbrower.top/gtrbiiranf.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gttimowdih.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtgcqcwrml.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtuxkipgzb.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gttkuzangb.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtoitmhivt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtwjcrroxs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ehwqpu.com/gtwjeuahjw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtrwlazuol.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtvzlwdebu.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtisaaslzo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gtrpzelntl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtvvodzigb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtavdfvxnb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtrycrogkv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtmxikrpok.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtjnsozgnj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtgbdioeuj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xziqi.cn/gtcozyltiw.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtzimlfzks.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtjbtexkqa.html


<!-- 参考信息 -->