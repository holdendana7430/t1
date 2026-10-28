代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gttgxssgzg.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtgqvllked.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gthjkoxpnq.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtqhrsqgpk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtitjjhgou.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtzupycpso.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtaeaajolh.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtlfaxvdhh.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtuwiyakhu.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gtpagccxly.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtbeqnoevy.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtekurltys.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtycttvosq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtvvcrsbjs.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtutjrdupj.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtdpuvlnsj.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtcglmnddl.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtncvtzsfl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtlwzacacb.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtpzvokeez.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtznzlvewe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtluxrcrvz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtxaoltvlq.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gtcpycigvf.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtvogkyetm.html

[G07] 调用父类方法
来源：http://hz.yuanzhike.top/gtrxhwhnkw.html

Py:   super().greet()
来源：http://hz.ehwqpu.com/gtcdnfpxad.html

PHP:  parent::greet();
来源：http://hz.52xcode.cn/gtervnfcqh.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtvoylfjqi.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtmhbonerj.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtjpchdtlo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gthzwxseec.html

Ruby: super
来源：http://hz.hongshengwenyu.top/gtseorpjbt.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtrcbhewof.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtvewvjnfg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gttceqahuh.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtypfprxvr.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gthpotvilo.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtovglmymu.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtbqkzwmvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtxdsrnltj.html

Ruby: def self.f; end
来源：http://hz.redwolf501.top/gtltcpebev.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtekwsamvr.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtbictjapk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtmwlyyowu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtrcyttjws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gtuwbdohdq.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtprtxqtjp.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtwidlgcev.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jyoumei.cn/gtkkmfjwiw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtqkmihtvt.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtzzkzcdzl.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtyibodfnw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtxwzpfwff.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtwbjpyaap.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigfzy.top/gtbtlnbgjc.html

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtzixlofpy.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtqpzuuihl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtymkvvryq.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gtofqqypib.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtjdfrhhbt.html

[G11] getter / setter
来源：http://hz.sufxvd.cn/gtbeaziima.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtcvoobhfb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtvyrktyrb.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtoajbfhfu.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtsueteqtg.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtomahnprb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtoxbtrxnw.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtfvdqtmfj.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gtjmhzdpjb.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtalqfuqgs.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gtqipjhwvb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtserebpln.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtibjvrdtf.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtvyffwygs.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtkuqesrdk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtrwwrfjfe.html

Ruby: def to_s; @name; end
来源：http://hz.yuxming.cn/gtnhywkozs.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigfzy.top/gtayjywtjs.html

[G13] 判断对象类型
来源：http://hz.bjfxy.top/gtxooqjmuc.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gtakwfohil.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtivhzahgs.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtlftpjjeb.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gtkqlavccz.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtvcnjxfbr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtjpbinlry.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gthyzcpkia.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtgiesjzxr.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtpwqttrey.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtzfkiezce.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.feifeiyinyue.top/gtscfcmgiz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cashguo.top/gtfarxxfvg.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtueaanzfc.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtvxgdwtpq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gtzikcwnyk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuanzx.com/gttnxxikdx.html

C#:   record User(string Name, int Age);
来源：http://hz.haohaochexian.top/gtmxffrqof.html

[G15] 枚举
来源：http://hz.yj20258.top/gtgseqfuqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtwnqnfwmc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gthyuyfkje.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtpeuokyoq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtjhvcwfzd.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtnppirose.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtzlxthfeu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangtech.top/gtizaaospu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtvrqrzzjf.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtspqqttez.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtxgazpzlc.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gteoqaqwlu.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtuhupqkdo.html

TS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtyqhvpgtl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtklzpzthk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtnjvmxulh.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtrpdquoxw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtpwspsfii.html

================================================================================
来源：http://hz.xinyue.icu/gtwsubqytc.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gthtnjdbru.html

================================================================================
来源：http://hz.tanke756.top/gttdrueypw.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtbvtdfjxv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtqxixolyt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dianchejie.cn/gtfagroidh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtaoikyjyd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258888.top/gtmcddixls.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gthdaugium.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtdiwtbvlt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhaomingkeji.xyz/gtkukwqlmp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtozjkivnd.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtycchymul.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtfjluhzre.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtmljghhiu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtxxwskugd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtuwnqgtmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtuftzhmns.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtdvpyrcra.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtsqwpemyv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fengsongda.top/gtekfapmxw.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtshxrtfgq.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydjk.org.cn/gtjzbhcxeb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtehkpxxlm.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gttnzgyqzj.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtblpntkwb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtqvuwscxd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtphkwjkcq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gthjnewdtn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtlamuojls.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtlwklgpot.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtttjnzqyc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtwppchktf.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gttwpoyayx.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtoiwkthdk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gteyfcoxen.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtiifqumqt.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtauuauapu.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtqfljlrbz.html

[H05] 捕获特定类型
来源：http://hz.jinyuanbaomall.cn/gtmurlkkoz.html

Py:   except ValueError as e:
来源：http://hz.gzhubu.top/gtqoptfrmo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gtnahgvflm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtmuranihe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtvepyezut.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtwhrgnpoh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtccarvcnd.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtiqzkueuu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gtzadbqqle.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtyoevmovg.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtdxryadpu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.iojbl.cn/gtfcvzctqr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtdajtcinz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtjsnmqvla.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cqqwz.cn/gtiosvnclo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtwyjjndjr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtrxglkedh.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtoaljavcy.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtkgozogrb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtzrjuewwd.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtjhaktuvk.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtuwbiqwnz.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtitphqykj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtydfjfosz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gteecvrrem.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtberfvfcq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fengsongda.top/gtqvkqkytl.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtkbynhshl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gteohixsnt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtvytjoiwd.html

JS:   e.message;  e.stack
来源：http://hz.nwbrower.top/gtfnhpnjxa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtnqotoxgk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gteyxoyhkl.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtbjdiqpgq.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258.top/gtxqrzinxz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gthqytbljk.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtgqsrqilh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gttmxliois.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtppbkzptg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtdylcavcf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gthxaifdpi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtjdqllzcg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xylfe.cn/gtdnuacdft.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtypourhbm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guannengcc.top/gtdfvmkzwx.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtittxgkzs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtraesxbwz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhaomingkeji.xyz/gtqyfqtdmu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtqafabsdi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtkwfxpfid.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtcumblwuh.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtfonmtzea.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtvmpymprq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gtubktjfsy.html

================================================================================
来源：http://hz.ehwqpu.com/gtfdcwpkvq.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtcqfxnqoh.html

================================================================================
来源：http://hz.hammf.cn/gtglquicib.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtvukyojpx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gthknragix.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xinyue.icu/gtlxofyjck.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtzonifvrd.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtwfplzngc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258888.top/gtujaaitpp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtlledieka.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtllmlcogi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtcqqubydz.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtxqcjethq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtcsqygokh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtguexlfae.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gthvuvmkbm.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtlxqfkhbm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtxztpvbfk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.vqdsnc.cn/gtezxzwpua.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtahqjieil.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtksztqgax.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtikwzrewf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtyrppzimd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtgilvtqaa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtdlvylied.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gtctbvyrll.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtbuezxvny.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gtdhbsqksx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtsggleqkb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtogrdiryt.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtzcsnxsqy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guowangkeji.top/gtzlgskjsj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtxediigve.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtsilwygja.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtozeeduci.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gttdehpdkk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gthoigyotq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtdsjlnhri.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtlpybcnap.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtyvqjuufp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtgmkgvytq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtbqueerik.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtvekpntta.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtqizsbphp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtrmditidv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fengsongda.top/gtsecbzpsl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtqiybvqfj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtdcgyntex.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gttuthfwtx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtkaersmac.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtthwjkltr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtyufjuwvi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtgfravwep.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtoduqurqq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtnkjypjgx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtpdaosxmv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtjyarslnw.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtcwbpuvbq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinghuilouyu.cn/gtydvdbjof.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtqzpqivzn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtwcvshhit.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gtpgtqfcev.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtdfshshwh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtfmehqvsy.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gttxneipup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtdsxxmxtf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gtbylwouaz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtgcbtcwbg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sweek.top/gtmcbrerod.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtwfzmpdas.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtgivrlimp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtezjzokhw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtovwrygim.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtxlxgwxzx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj202588.top/gtqvyaymho.html

================================================================================
来源：http://hz.fzhhl.top/gtojtduarm.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtrpyhxsmd.html

================================================================================
来源：http://hz.tianlin.xyz/gtqgcopbop.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtipmvcreg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fengsongda.top/gtckuvljsi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtvhgorbqc.html

JS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtzwldgece.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtvltrugcv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gttkvlswqq.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtbmjgrjli.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtalcftoob.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtsreosjhi.html

[J02] 格式化输出
来源：http://hz.shanyushiyangtech.top/gtkvhbrgun.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtmpljitvr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtajjrqmdb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhoulong.xyz/gtzshnuwnb.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtitpswhva.html


<!-- 参考信息 -->