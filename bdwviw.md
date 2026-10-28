代发 wailian999

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtlpzbwdgv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtzakkxzdt.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtmnnwyaeo.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtdmjzggrh.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtjrwwcoes.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtjzjgzabt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtnthjftjq.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtqqnkmapg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtwxgmmpsd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtpiluuuqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtorkliobe.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gttimjqhho.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtwezcupdb.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtncjcrspa.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtzcyxhjrl.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtbbajpoyf.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtikmolhyz.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtqklvfulx.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtslimwsxc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gtbfpibenk.html

Ruby: super
来源：http://hz.mhx1999.top/gtyvarisku.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtrbscjpwp.html

[G08] 静态方法与属性
来源：http://hz.pengpengdd.cyou/gtbbygitbn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gtnkrqsrmi.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtjuspqkan.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtclupfxox.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtjuvpokue.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtxwsdcpst.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtoamdgpxv.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtfluijksx.html

C#:   public static void F() {}
来源：http://hz.ywan-chungtsiang.top/gthqarkyxj.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtxtvdgris.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtnadwwdes.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtxcdnzwmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtyjfazhfy.html

TS:   interface Shape { area(): number; }
来源：http://hz.yongpay.top/gtvictdqiq.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtnovkrrpo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pycfn.com/gtfrjuuafy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtejrqmhch.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtwpjoxvaz.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtpzqxlkxc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dashuyun.cn/gtrbsogmcv.html

PHP:  public / protected / private
来源：http://hz.jinghuilouyu.cn/gtalhwrolx.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtuwypekiu.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtuglxywlt.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtycmirnfm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtaifzupwi.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtronnzqne.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtqxsicata.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtqbtkeddn.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gthqqjllzv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtujakivqt.html

JS:   get name() { return this._name; }
来源：http://hz.yanxiufei.cn/gtimprazbu.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtennbtatw.html

Java: public String getName() { return name; }
来源：http://hz.ydjk.org.cn/gtyoaaozep.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtlliiqvgw.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtmkyymfgx.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtrrcdwlmv.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtsvumrsuj.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtmesnfmjc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtuyhbmjql.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtfvxzcyee.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtrpimzfpt.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtzurfwwhw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtyexhakqj.html

Ruby: def to_s; @name; end
来源：http://hz.gzhubu.top/gtcyzvirhw.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtfyetixcz.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtkbkqxdxl.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtncufjfpp.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtrdxqgzhw.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtvoesjilh.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtvfzmrvwq.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gthjmblbqw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtszguohcy.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtnttcnipt.html

C#:   u is User
来源：http://hz.hammf.cn/gtayhrrxhu.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtcztraapj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dianchejie.cn/gtfhgjvsvc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtweoocxgv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sufxvd.cn/gtqzfntcjm.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtqthcyosr.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtlduqadav.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gtlnflntpi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gtzxrigtch.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtlchllsyk.html

[G15] 枚举
来源：http://hz.52xcode.cn/gtqigfzhsx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.birdmap.top/gtmciupani.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtoaqycoqm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gthnlhfbks.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtfzcujmzl.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydjk.org.cn/gtgautzvbl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtrpcovdjm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fengsongda.top/gtyzrqkgcj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtlooohxhu.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtghzrbhfg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtmvdjgylf.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtlqalnxho.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtihqfbhwa.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtbnehtgvi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xylfe.cn/gtlrcnhwoz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guowangkeji.top/gtrnhbcdjk.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtmuwohxbm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtfbodtxbh.html

================================================================================
来源：http://hz.birdmap.top/gtvonzlrsx.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtiwxcqmwy.html

================================================================================
来源：http://hz.ivvv.top/gtxblxjdjj.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtizqpxmhc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtbvsqlctt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtlclanwra.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtpdlexogr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtadubbnhi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtaygmmjql.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gtocalghgy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtfkzlcnow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtqmhvzind.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtbjpbnezl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtpkiqhsbd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtyopqfkxc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtegbyfwhb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtrqvbrmku.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtvqukuinz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtsezzcaaw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtftjfukdf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.bjfxy.top/gtggjjkbng.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gtddssaino.html

Py:   raise ValueError("错误信息")
来源：http://hz.tianlin.xyz/gtfrjeggrw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtneeergkr.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtynhifyky.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gttuwuiazz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtdunhrqrp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtluiaknuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtcduoczko.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtwthbpkdt.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gttlwgobxt.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtcttpgbwq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtgqblafjt.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gteecrhrnc.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtcwoeirge.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtomquizif.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gtfvbgtmpb.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gttbdpsobz.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtdcidhsgr.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtdmgfhmfj.html

Py:   except ValueError as e:
来源：http://hz.0kj1m.cn/gtdcdunjqz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtdazntpuu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtpsshzbrq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtjchwszvo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtiozhvgrf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtuvgxfavg.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtsggegdyc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtqzzjkmlt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtvxrcctvb.html

Py:   value = d.get("k") or default
来源：http://hz.zhaomingkeji.xyz/gtrtjukdxh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtxnivnxhu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtzlzojydn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtyrvmulns.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gttrqwokpa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yueranfly.top/gtklgyrcxj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gtctkpnonw.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtlnlqqpek.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtlupurtwx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dianchejie.cn/gtopyqsbhd.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtmbipvena.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtmxnbjmmy.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtahksyyxg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtuxjsfwff.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtckywympd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtrvxvilpv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gtzowgowqz.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gthntktawp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtvswubcpg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtjqjgtdmq.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gtvmhptaln.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtensclnqo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtjsimxvly.html

Go:   err.Error()
来源：http://hz.zycfv.cn/gtjjjfctyg.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtleqioqcv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtkvopamhk.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtzvjqsxbd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtnnimmilo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtmqzcrxnw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtbieejszx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtvfdlxxjb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhongyouzk.top/gtuautzxjp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtqmysefgm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtgejrfwml.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.feifeiyinyue.top/gtdzultkzt.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtrudtvbde.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtidhdgefh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtaffalbiy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gthnvtqvjo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gttqgkjgex.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhongyouzk.top/gthycojytb.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtzqzeqnjl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.birdmap.top/gtuhqggdvm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtmvbfgcio.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthwdxnmfs.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtuzdkboig.html

================================================================================
来源：http://hz.yueranfly.top/gtkwzgciid.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtnsnirbuz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtrzlehrzx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtpanukxrj.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtrbqhdusi.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtjsqruhue.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtkikapqbs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtrmjirttw.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtmivihvtx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hfpthk.cn/gtoogtuyyo.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtlhabymzz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtbzorvywl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtpyhmlwpb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtmqcyhbtz.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtybhaspdw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtzubxupcm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtxqzqckkz.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gttlpiwobj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtdfjmvzvs.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtrbajcjvm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gtykcvawki.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258.top/gtfsialgmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhongyouzk.top/gtthswogoe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gtbrnjbind.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.bjfxy.top/gtxszqkouk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtcandwkro.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtfjqizhns.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yangfankeji.com/gtqsmclaud.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtosogjhcz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gthxbahvbj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtzutjvmxv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtedfzzhvn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtgetplovs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtwhsdsrzf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtswgtbyga.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtmffbylsn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuetiantiany.cn/gtkgmshyqj.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtdsbvqucp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtroiczqdh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jlsjyb.cn/gtxiazbpca.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtqhbciwkb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtlcvofvwr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtbuafdxmn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ppjwa.cn/gtpifpgycl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtrzvfmhwv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gteqmmnzbn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtjjxxhdiv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gteyxkiiql.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtggxruizc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtnxqcyilh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtfyfwhjzz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtxlhpgiqz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtvrmrsamc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtxiisoboe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtzpnpcvme.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtdrxjlbam.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangdashe.top/gtlvhrkblx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtqrividej.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtcprcmnpl.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gtgzawqtnf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtmajdaqta.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtlvoulafu.html

Ruby: s.scan(/error/i)
来源：http://hz.svipenyu.cn/gtlgxgtccj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtphruusdx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtvvpsodra.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtwkwyvrse.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gteuhttxfl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtzymckdff.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtqhgygtvq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuxming.cn/gtsdzldtlb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtlumgpkju.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtxqickovz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtuvcqdoen.html

================================================================================
来源：http://hz.ppjwa.cn/gtfichgswc.html

J. 日期与时间
来源：http://hz.c1oappe.top/gtlxfqxeda.html

================================================================================
来源：http://hz.xylfe.cn/gtycfoyers.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtixrgqlmf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhiwuduotai.top/gtqfguztse.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtekmhqfqz.html

JS:   new Date();  Date.now()
来源：http://hz.mhx1999.top/gtnmxbdllj.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtfdgzwxak.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtumlztmdc.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtqbpmkeqo.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtnmzgswkt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtdwdrmgmt.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtqthuizxz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtpdnhkchp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtjserdrda.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtkwbagbfv.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtxghplewp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gtzbjftuxi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.9152youxi.cn/gtmeduvxtu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtgfsskpsp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtothmthwq.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtjkhknqph.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtjgltnovh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtwqoxkcmx.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gthdchaudw.html

TS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtraafencu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtqjdestce.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtkbenwrev.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtuxptlsfr.html


<!-- 参考信息 -->