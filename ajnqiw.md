代发 wailian999

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtnpiqgnlk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtdmwjfsqs.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtekhaftac.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtgighjwiv.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gthkvgbegd.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtrjfpmbbi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtqwicuvwx.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtpwraeyne.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtbywnjpwd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtwdiucbns.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtmnoivnrq.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtmnsbhkzj.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtcnskucnt.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtqvfiofig.html

Py:   super().greet()
来源：http://hz.sxryk.cn/gtvjrmhgyn.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gtiipftkjv.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtaiiexfac.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtpxeyfaxy.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtodrkvcwv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jianghu66.top/gtmzppzirg.html

Ruby: super
来源：http://hz.shuidangran.top/gtzcsxsgeh.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtsndmrzrv.html

[G08] 静态方法与属性
来源：http://hz.ydzc1.top/gtzebyeazd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtdndwoaar.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtxmnanytp.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtadqwzthg.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtujfktnph.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtkdokxpgf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtmisisxra.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtvtbkjooy.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gtmfnejiip.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtjpfwpxwr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtmxcyojfh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtlnrvyfqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtnlibrjnh.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtejijipyy.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gttbddaiyk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhengqikj.top/gtdobrpjyp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtmonlzjib.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtaggssnfg.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtkdtbeapm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtdhrusdcm.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtenapeano.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtlvoereee.html

TS:   public / protected / private
来源：http://hz.gogol.net.cn/gtliakzoos.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gteusctahy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tian-w.cn/gtqweatrep.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtnyhugxpz.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtwcttaaje.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtgtvcddje.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gthytbqdyx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtzrxotfmy.html

JS:   get name() { return this._name; }
来源：http://hz.yuanzhike.top/gtgwocyqfv.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhongyouzk.top/gtxuqrueul.html

Java: public String getName() { return name; }
来源：http://hz.hongshengwenyu.top/gtgnajswgm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtdvuonmhi.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtzcognkdm.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtsdknaczx.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtblxpcogf.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtlrfmjidj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtnnxxbtvq.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtefykhqgi.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtyhwivdoy.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtsaywdbyj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtwxkdofdg.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gtumhoxfyu.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gttrywsxde.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtsucbyukn.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gttuhbdutu.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtiusywcnw.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtehfqrmxl.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gtqffegkpa.html

Java: u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtrppedlbz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtwlsvefkv.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtypigvstv.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtvimyxcdm.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtlgedtbvf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtfxnojynu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtrhxmklvz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.feifeiyinyue.top/gtinoegkqg.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtzhwotbnk.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtmzemxsve.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtxeoecikb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtryfajpgk.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtxisxxxzm.html

[G15] 枚举
来源：http://hz.birdmap.top/gtkppiciyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtlepytmip.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gteeqkdped.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sufxvd.cn/gtcbfjdgcd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtdtxruuhh.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtztafbbsf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.andypj.xyz/gtwphcvpdf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gteqcqhqtt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtalqllwtn.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtdukqdibn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gtleyetgmv.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtaikieitw.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtknuaenpt.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtomtbzdjq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sxryk.cn/gthvdlloit.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gtgszrfqma.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gtjsgsjxfk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtqrsfythm.html

================================================================================
来源：http://hz.smart0.xyz/gtpgeobtqv.html

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtbjxuwkiv.html

================================================================================
来源：http://hz.snrcjt.cn/gtjesrvnfv.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gtdsovhutt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtawegouhb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtowmaptyd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtoaopdqso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtntpvubyc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtuqmapdlz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sysykeji.top/gtbquwrfek.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gtqdpgzekm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtvmgyubsj.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtpwrwjdhx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtanqxmrdv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtidhbhepu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtpymrvfmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtrbobwran.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtdjopyyrq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gturhydavf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtcziffeev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtbvjguabu.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtrmypbofc.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtcrrtqmei.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtguwkdani.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtjsihibne.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtqpukhvtr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtebxcimxp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtfwptilts.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtzlhubxvh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtuucyogey.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gttjusmnsc.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtpsuihmro.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gterovhjmz.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtutcssjxq.html

TS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtumuhdetk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtswcxhxdq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gthiexvltq.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtmmeywrxz.html

C#:   class MyException : Exception {}
来源：http://hz.chenzaomai.com/gtkowvozvb.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtingqpyqn.html

Py:   except ValueError as e:
来源：http://hz.yj202588.top/gtjutfdsur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtgjwdxjjm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtmozbtbyf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtmbducwsl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtmzkvryns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtwrmaddpl.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtzsdtnkxb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtpttsdmuc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtzwplumbk.html

Py:   value = d.get("k") or default
来源：http://hz.zhaomingkeji.xyz/gtbdkrwxga.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtnwppikfe.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtzusgttnw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtcoxebbok.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtejnpkrml.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtbcgayrzf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtmqwyrddg.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gtxmgfsipx.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtxcucdvss.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gthmkgicjj.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtymswwmbh.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gthgwmeqka.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtxspjiiui.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtbhkyxfec.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gtauqnqzpq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gtwsfiyuud.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtbnpiqhur.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtzniestjn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtgjtixlbb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtzorwwvmi.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtxgcyywdz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gtggcccdpe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gtnrhyjvov.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gtxqkwxuhz.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtquyhsryr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zycfv.cn/gtzkwxyece.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtjupsmjrx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtohdkrigw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gteqvrcjav.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtdxecfkza.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtjkzxevbw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtppmqygnb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtxeocefim.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtrwgfvdgn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtyinecqri.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtjpfkrulx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtmyyrkkie.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gttifoxigx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtngknkbzw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtdvunfcvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtiphwofin.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtsvamiusa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtnwpdlwhc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtviokfick.html

================================================================================
来源：http://hz.sxryk.cn/gtsnrbqlij.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtgxkacwbd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmhkltqkb.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtqjjicbqx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtwblmugbx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtcvlopnpu.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtqmogteim.html

TS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtluqfrgph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gtnxbudqdl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtipykebrl.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtgnpspvmc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtisftdnfd.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtnrfzmkbv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtdzegvshn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtynutxnqh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtidrfppvx.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtrdyedfvp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtrnajujhg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtajfsvijn.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtcztrlnkl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtfcqlvpun.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtjdbyurca.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtymfnhmmz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtwkwlkacc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtdjcbfjkd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtfwbtwqqc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sufxvd.cn/gtmljljlkz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtvelnomaa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtnwjfdjqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtcrdyqbfc.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtxaozgiut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtybbcxedz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtzsdwtall.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtwybbjwby.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtuteewqqd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtoxscglzo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtnwkzsdoh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtacerklrw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtthfpthkc.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtffacaycq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtslwvybil.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtaqxfsnaw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtrtslwlbo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtootoblpm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtqevxopvt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gturdsqqos.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtuxupsyjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtfbkewvku.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtovakxgzz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtxjpuvsty.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ehwqpu.com/gtjxqkryjs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtjgochdzo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtllqybusn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.iojbl.cn/gtxstbdazk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.haohaochexian.top/gtickuxlpl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhengqikj.top/gtfmmygzlu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtdsnkzuhm.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtxyuakvhi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtimdetuxz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtefbcsmso.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtskxiadbz.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtiaadkgyv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtzcmhrlxd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtaxwdxfsj.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtnuhrppuo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtwulakjws.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nwbrower.top/gtrwaabddc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtsaxhzyia.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuanzhike.top/gtdzkohziq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtooyqqfbw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtctssxscs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtndlyptyv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtknidcakf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtdeiuosgn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj202588.top/gtqsvcqsry.html

================================================================================
来源：http://hz.jyoumei.cn/gttyyxeyam.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtahqnmdei.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjevfnbsv.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtisqzpxba.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhiwuduotai.top/gtgusgexbg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtecyiuqch.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtznoizxvm.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtizaulwvq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtfxsvsvha.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gttygraouc.html

Ruby: Time.now
来源：http://hz.aizwys.cn/gtxhlzcjlb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gtsivitndj.html

[J02] 格式化输出
来源：http://hz.hnxiangtu.top/gtojmitnik.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtxhlsvoyi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtgsqfcnjg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtrzfqyynp.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtnnzxrwtc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtiqdrksqn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtliahxpjg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtfsennnon.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtceelzoss.html

[J03] 字符串解析为日期
来源：http://hz.jqgfzy.top/gtiwmzvkop.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtrlurtizy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtraxbhntk.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtecqfqypg.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtkwfuhjpe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtkkqwbvjy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtbktxezow.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258.top/gtrsdkfnlg.html


<!-- 参考信息 -->