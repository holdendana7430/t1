代发 wailian999

[G06] 重写方法
来源：http://hz.wangdashe.top/gtxlnswadc.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtqvnuxbqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtumkdorbx.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtlumygzsk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtimqhedco.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtyiyhhhwk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangshuangyany.cn/gtziaooqrg.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtrzknweuz.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtkntubqsb.html

[G07] 调用父类方法
来源：http://hz.guannengcc.top/gtrmlwevki.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtyovlpooc.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtasbsjdsf.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtfvxefllt.html

TS:   super.greet();
来源：http://hz.ehwqpu.com/gtttuqtyxk.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtghtvzhvn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtxqylylrw.html

Ruby: super
来源：http://hz.hfpthk.cn/gtkmcixzzt.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtjpoelutg.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtwmafcade.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hywenlv.cn/gtoxxjrlth.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtojuomysr.html

JS:   static f() {}
来源：http://hz.52xcode.cn/gtbayjbvph.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtxmwfipze.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtmygwdqwf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtumkwlbcj.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtsqytxasj.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtfrxmqscc.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gtalpkvnnn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtjvhmosau.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shangyingyoupin.top/gtawyvqdka.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhengqikj.top/gtnsontlob.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtisdwdlcy.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtmeujzwrs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtixuybalc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtgdioyahg.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gtndnqpube.html

[G10] 访问控制
来源：http://hz.meibo888.top/gttsnuqvpk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtoesytamk.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtkbchlrcs.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtfufohjjw.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtcionmefd.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtgpuzwdmu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtrognoqox.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtwmbsktpe.html

C#:   public / protected / private / internal
来源：http://hz.cucudq.cn/gtykypcqnw.html

[G11] getter / setter
来源：http://hz.hnqzz.top/gtjkvuwmut.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gtwpuzxrzo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtmyfvmjde.html

JS:   get name() { return this._name; }
来源：http://hz.jqgfzy.top/gturertroq.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuanzhike.top/gttvnultlk.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtanljzmwm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtgwokfhgu.html

Ruby: attr_accessor :name
来源：http://hz.guowangkeji.top/gtqooxwtpa.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtotaoxhrj.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtehmsdbwg.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtxrmktzxv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtrawhrjiu.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtaxdfalsj.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtnurjpphq.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtdhdurcea.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtkxnxfdwl.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtgzbdjgom.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtvbdykcsl.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtmmtohcmg.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtarrxlptw.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtzfqgxuue.html

JS:   u instanceof User
来源：http://hz.fzhhl.top/gtfkhbsjpq.html

TS:   u instanceof User
来源：http://hz.gotoacloud.top/gthedjzwtk.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gtdbcxrsdq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yueranfly.top/gtdipskilg.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gttdxppmpc.html

C#:   u is User
来源：http://hz.cheryme.top/gtofmuymzy.html

[G14] 数据类 / record
来源：http://hz.shangyingyoupin.top/gtikarohzo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gthflwlvwz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtsthaikur.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtmxzwbeob.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtihkleyeo.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtmysrkcug.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtuuynnooz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtfromcuff.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gtayymnxsl.html

[G15] 枚举
来源：http://hz.nanxuanxn.top/gtaqiletdd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtmnjqedsh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtgwkswqxe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gthnhhlnbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gttpdpkzcq.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtnealhzhr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnxiangtu.top/gtnxmeikuy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtlnzrzfka.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtwrrfambt.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gttojqykya.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtatrqkbgt.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtvxpjjyqn.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtrftsaxbs.html

TS:   Object.entries(obj)
来源：http://hz.yuanzhike.top/gtbtmkcvcf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtlkjgebhy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtfgajtbei.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtwenzrkcu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtfaecnmlv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgvzlodmp.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtptvnvjev.html

================================================================================
来源：http://hz.hammf.cn/gtqedwubfu.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtnzpcqdfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtvmqnqecx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtoawdtdtp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cheryme.top/gtqahciowf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtissuspny.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtqqtqawtj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtnxrpurkx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtxyofemok.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gttldhzygg.html

[H02] finally / ensure 收尾
来源：http://hz.sysykeji.top/gtcxyuchwv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhengqikj.top/gtfgznnjlm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtbbhlkedr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtxkbbjhyz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtupipuuwy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtbmrrkekd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtqocdzssu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtzmmhsgbj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cdnleiting.top/gtmlwoxbgb.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtudwzdhgc.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtiditnkbk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gthpurzvgs.html

JS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gthlscwsgb.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtolhweggy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtwwmasilc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtyitebtgd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtfpmahaxx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtsrhhuhnn.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtzdwzndsd.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtppwquugk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtefbiwvkn.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtnvounbkf.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtvwlutpuy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtcqzmcfcc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.snrcjt.cn/gtpamhduqh.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtjdjlwdyk.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtonmjqabx.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gthfeafckg.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtwnriultp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtaqsxudai.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtguddfdjb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtlllyprri.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtjiqomlyp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pycfn.com/gtypgbsppr.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtrinjcprd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtbjwmtscy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtzjooxntf.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtihexbxet.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cheryme.top/gtcfejybvd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtsfoziccy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtnrmppgjy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtneaoqmpc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tianlin.xyz/gtacquqqxx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtgrobvuhf.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenzaomai.com/gtxexwrzvf.html

[H07] 断言
来源：http://hz.gaohongyu789.top/gtfnrbipov.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtfgpuhpdw.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtluubndwx.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtgebtguzq.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtnewbselj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtskpguthu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtloqkbuls.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ivvv.top/gtukhmxhjw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gttvhtuvwf.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gtoqctprqz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtzikitifd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gthnudxbfi.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtckfekbop.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtjzurwuus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jianghu66.top/gtyfpirdjq.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtlmibbfch.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtzarfnnev.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtefwlkdgm.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtwotkqpnt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtagpmrkbe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtvveqyxnz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dianchejie.cn/gtsmghsmws.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtmmymkwqm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtplvdcjpd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtslqxcedc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtslfvwlyn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtnkxonlwd.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtvgpqkfhi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtzitnuqfj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtsyuelzbw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtlpcubbkq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtvegyoroe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtxoekwzsx.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtbjwiaajn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtmenhoasb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cucudq.cn/gtwmmxeezz.html

================================================================================
来源：http://hz.nanxinkj.top/gtyfmsuxgx.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtfgloeqfr.html

================================================================================
来源：http://hz.jyoumei.cn/gtlsvywuvr.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtycihrifo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtlatrpjnq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gtuwewogil.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtqkwtmlzi.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtwqemmdwr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtrnxwnspv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtcnktszib.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtabmzwqrp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtrcrciqha.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtstndgjnp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtsusjnpiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtzttwferw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtfmiubkxw.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtqfznmngv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtrungialv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtcbqonwej.html

Ruby: s.scan(/\d+/)
来源：http://hz.hongshengwenyu.top/gtfjahmrug.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtaltygpsi.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtnoiuxwdg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gttlsxqukz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtoxehxekl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtoxrytpoe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtqeovhfcz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigfzy.top/gtlvaegiwp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtqggarpob.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gttufhmiet.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtmlqipokj.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtiwksklwh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtqebrwysn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtriihnbcu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtkekxalkm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtvvunjvab.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtpgqvmsfo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gttnisgnzt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigfzy.top/gtykraytnt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtblnioftr.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gteoossbtc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cucudq.cn/gtrjngkipa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtvvikbkgj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtujnismlc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtcbwqmkfl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtcexmsjzr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtphcehduj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtclzwvkwt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtiqgdwxpo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtqmgbhtos.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtxtandhqz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtwhmtutur.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtakkoxhnm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtlklrjrio.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtjimlsmlh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtlccycwsu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zycfv.cn/gtajscwcga.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtwlqgjekg.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtfpkrawdw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtjvpcaltv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtpfweqjpa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tian-w.cn/gtjbiimfcp.html

TS:   /error/gim
来源：http://hz.hnqzz.top/gtjxhjcvap.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtjsjaxclv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtpupbvfyt.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtnigyuxba.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtvulfwzzg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gtltpctkvd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtwyjyzfev.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtnftoqlyq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gttmwwnney.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtgmowxoai.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtcjynitdo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtvcjwbhkk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fzhhl.top/gtyzrdsdnc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtwpggxhnf.html

================================================================================
来源：http://hz.xinyue.icu/gtuaopqnyv.html

J. 日期与时间
来源：http://hz.gzhubu.top/gtdqujauiw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtxksayuvj.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtppnxgijk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yongpay.top/gtwzeeeeoq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gtaqlcpukw.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gttphugujf.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gthvregtbx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtaistsvmq.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtzopbzfhh.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtkdutbbeu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtbbltsibn.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtmiiftpgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtkxfpewhj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtfmboqhgf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtvhccolra.html

TS:   d.toISOString()
来源：http://hz.chenjidiqi.icu/gtfidkmkvv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtoqkhvhzl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtolfciuqo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gturcufbhh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtwzchirlf.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtojkughzj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.bjfxy.top/gtvqnntoka.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtixhmllce.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtlkbqwate.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtsrculiif.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtyyglrspt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtexgwqwsp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtfrifwskq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gttekzhltm.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtrpclbgan.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtoosqvztg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtvexwzach.html


<!-- 参考信息 -->