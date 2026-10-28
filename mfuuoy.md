代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtkmrrmzfv.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtyyfnrugz.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gthfvflftk.html

TS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtfdjbbjkb.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtwvbjlntc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtxgwkjerk.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtcgrxvivi.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtriinjqfo.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtmykoikwb.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtydqkstaw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtbpnrymll.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtmfytammc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gttydgcusm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtfwtqgoby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gteywuqpti.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gtppebyteu.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangshuangyany.cn/gtpboensny.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtnpjvcllz.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtkccuhwpz.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gtjupkfrgu.html

JS:   super.greet();
来源：http://hz.xziqi.cn/gtzthwpvxb.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtwcangyya.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtalpyqfnc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gttrqrwckl.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtcufsicgw.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtjzopdzhm.html

[G08] 静态方法与属性
来源：http://hz.gaohongyu789.top/gtymfppxpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtappxxufk.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtckmduvad.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gtrpaxoadh.html

TS:   static f(): void {}
来源：http://hz.yongpay.top/gtagjmfddo.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtzohyauas.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtptefyrrf.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gtbmbkpvji.html

C#:   public static void F() {}
来源：http://hz.zycfv.cn/gtcyulvatc.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtmvevvfsh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtxajtywlb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtiyozmrba.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtonsemlpx.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtxtuqstle.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtpgwxvaqs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtbkyzrmrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtxejqenql.html

C#:   interface IShape { double Area(); }
来源：http://hz.cheryme.top/gtxtfvazae.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtutqcpntf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jyoumei.cn/gtyaomgkhc.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gtgqpyrwba.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtdbqqciwt.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtaldtfdyf.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtdutebuce.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtnchsdcjl.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtlqdzcqwc.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtwqjrniib.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtfyqohtij.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtpfamgnvo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtsmdsxryt.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtvcrhhnar.html

TS:   get name(): string { return this._name; }
来源：http://hz.yangfankeji.com/gtwxnbrmzl.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtdxbdvtvj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gttoyynlix.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtxbqarwoz.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gtdmptgtqy.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtpughandz.html

Py:   def __str__(self): return self.name
来源：http://hz.daxiang520.top/gtbyviuggl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtwaywptmu.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtepgbvdzb.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtbyrotvkx.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtlputjmxy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sweek.top/gtqrnfrtry.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtkkhmyaui.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtkdtdxhyl.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtqdyqozbr.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gtlbbqyctp.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtzinfmond.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtvwgdqlbv.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtbxtbehqn.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtrssxangg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sufxvd.cn/gtpfkxlevn.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtkdknrdjl.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtpgmkftxo.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtncobapkw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtrlgbhlni.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtddgjbusl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtunfzotbz.html

TS:   type User = { name: string; age: number };
来源：http://hz.fengsongda.top/gtleidkjhh.html

Java: record User(String name, int age) {}
来源：http://hz.iojbl.cn/gtjsbajhfx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dianchejie.cn/gtfohhrmnq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtcganyjaj.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtkbxfnkjd.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtxfauvfek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gttotepubp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtylfivlaw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.andypj.xyz/gtykqphnyj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtccqvowlh.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtdmmilbhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtzjveeyfq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtcxhuhjbc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtomxjdmrg.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtwdvrpnou.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtjdkgwski.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtyansrjkv.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtckbgkcux.html

TS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtzpxsvnhw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtxhnpneuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhijiandao.cn/gtprxgfuxn.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtxdwayvit.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtzdnewurf.html

================================================================================
来源：http://hz.svipenyu.cn/gtzouinoml.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtyysxibbj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtjzozmsps.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtfzwjbqmz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtngqmhdnl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtzyrqtfsz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtqrksrhqk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gtrrttrdwi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtugxlubfx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fzhhl.top/gtnjdzbmrk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtheimdvdh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtcrrpfewu.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtlhdfciko.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gteuxebufm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtgbnnuhss.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtkeqsuukq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtjvdbmgrw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtkmgwpipz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gtialrkkxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtcgqtsyrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtsibitotc.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gtqfmdghuy.html

Py:   raise ValueError("错误信息")
来源：http://hz.cashguo.top/gtwxixvqus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtuehowufa.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtzuzghdcs.html

TS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtgxxhekrn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtgyjbivvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtctemuqax.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtrtszwujb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tanke756.top/gtirsuatif.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtmqntfwoy.html

Py:   class MyError(Exception): pass
来源：http://hz.vqdsnc.cn/gtgobzumhj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtwojmsbmf.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtsnpcaosd.html

TS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtbozjruxk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtccjooarr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.quarkkingdee.top/gtbuzmmgkt.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtfzglacvv.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtsecrvlhr.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtqemngxkw.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtyxnkytoj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtklhbbyed.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtzcbaahix.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtbigddphx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigufen.top/gtkaaiqpha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtvxcbbvil.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gtljjdxbaa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtwgvarlfk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtvgnxukwn.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtqblarpun.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtdjquziog.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtdchcxzau.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtkkrbwxkx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtonfwlrwi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtbwgnbbps.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pengpengdd.cyou/gtjjpstene.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtcdbndpgz.html

[H07] 断言
来源：http://hz.xylfe.cn/gtoetjnunt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtquosaczj.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtrzffwyqn.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtamrfaiwk.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtrpmdrtdr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtlczykhlc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtcwuqkgxg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtvisvkcme.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtkqlhtfip.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gtvptibnzq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gthrykuwmx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtlffyqfge.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtrzjyoacl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtcvmwlwcj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtefixckwq.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtvhwcwjod.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtazirjzyw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtwjtrgjtk.html

[H09] 带错误码的异常
来源：http://hz.sweek.top/gtnpreumxi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtedvahovx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtccjhlnbt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtiilgxhit.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gtrxjlzxta.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtkilhdhed.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtysypmadf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gteblotpgu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtdiwbklqx.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtcgpdggyj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtrvephukq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtibladucj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtdkajquif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtfidwqrof.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtgqgzlzcl.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtpzkydipg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtwbocmnnw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtjeduemop.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjiysesbh.html

I. 正则表达式
来源：http://hz.jlsjyb.cn/gtvhjugxcp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtroxccnaa.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtuccpxjcu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtdujbtecn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gthsivcvam.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gthplalbpr.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtuvefgxcv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ywan-chungtsiang.top/gtefhtlvfl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtkyotvvdn.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gtogxkweds.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hammf.cn/gttvnwajti.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtcptkqjoj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtbsizzpve.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtqnggqhre.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gticoaqmnz.html

TS:   s.match(/\d+/g)
来源：http://hz.yanxiufei.cn/gthihhdyuu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtmzyvijni.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtpoqftzbx.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtyrenulhy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtzegyxzpc.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtbfknwpwm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtrisanoka.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtjkrlzwzp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guowangkeji.top/gtnwushafu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtlksvryby.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtfvcxfoan.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtjzcbsoal.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtfvssuguv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtvcxkeaxr.html

[I04] 正则替换
来源：http://hz.hongshengwenyu.top/gtnqwktzpj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtsgfxbskp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtveokicts.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtzwsotuih.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtbpjdybaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtgrljabmg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtwmoyumgg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtczcobenj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtvkcctfck.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtxrnmjodl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtzapptwur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gaohongyu789.top/gtassxkmpa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtgotqltoz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtdpkriwyr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gteblsniox.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtlsdoegfi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtsejpqysi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtrmccxagj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtiaqyurmz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtygkqihcv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtkuythkfn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtwwdnvemj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtxylglhys.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtvcgzzplx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtnudwtslp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtpyreyrsl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtmcjfugkh.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangshuangyany.cn/gtktbmrqop.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtbnypedid.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pycfn.com/gtlvcsydne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtaecsgyih.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtzrudfkvy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.bjfxy.top/gtpwyfbmgu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yvedp.cn/gthtpwcaio.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtgmazfjue.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtpsdyxbqj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtxfztjhhu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtrinbtlgv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhongyouzk.top/gtxxohfjks.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtmstszzny.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtdfmfodpe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtesmddyhi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtkhmyyiyz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtidjgvsjn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtnycaadmd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtysjkfkit.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtfnqypcek.html

================================================================================
来源：http://hz.aizwys.cn/gtdvwlfaii.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtxtxjixlh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nwbrower.top/gtqyungpfs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtwbiwnaix.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtbnbtlmhr.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gthvmdqcyp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jyoumei.cn/gtywijuaid.html

Go:   time.Now()
来源：http://hz.jqgfzy.top/gtxdclrclz.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gthuapdqxp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtqrhodojf.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtxlvjagku.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtpcnqzwoy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtowxkdjkc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtuysgxcxt.html

TS:   d.toISOString()
来源：http://hz.haohaochexian.top/gtkrreodyu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtjpkzjhky.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtdlexwhzi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtgovpnfnw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtovigsfqk.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtftvsehfe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtwgrpcjdq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtwkihbxvo.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtfnbqxbpg.html


<!-- 参考信息 -->