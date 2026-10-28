代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtlcgpbrsy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.havefunace.top/gtoizprkik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtlozxxskd.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtmattwwxa.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gtxylcjilb.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtpogsdebk.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtcxadyzzo.html

PHP:  parent::greet();
来源：http://hz.gaohongyu789.top/gtutsgvzho.html

JS:   super.greet();
来源：http://hz.tianlin.xyz/gtbtvuuquf.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtrmacghrm.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtgqmgiizq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gogol.net.cn/gttgbzznau.html

Ruby: super
来源：http://hz.yj202588.top/gtjpcwolow.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtvfrdiydq.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtplfhnipj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtyzaumdaw.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtcrdcpgjh.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtguetdzno.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtwpxrqvbx.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtyhfvupaq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtwwhzyhos.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtidoqksac.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtnguctjqb.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtrdcsmzdm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtwwrdqebz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.c1oappe.top/gtkhpcyohs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtlhmvzdoj.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtdavyboil.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gtmmbvwvkc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtvqnsxgdb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtwqgjdqnq.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtyycgkcym.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtzacyilqp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtwrdrffzo.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtvbwgisnf.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtgmwumjwf.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtjlhxelbu.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtixwkzvxa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cqqwz.cn/gtuizwjxfe.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gtdkuuydwa.html

C#:   public / protected / private / internal
来源：http://hz.shuidangran.top/gttmevusso.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gtlrqjejij.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtplpvsoeo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtzcqdgbtr.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtnpfwsavs.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gthbxztypc.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtcnxxphxc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtwwgviljr.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtnlqdivqa.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtchduucfx.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtnqeueydq.html

Py:   def __str__(self): return self.name
来源：http://hz.dianchejie.cn/gtoaiocssu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtecallgoj.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtanitjytv.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtuogenslj.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtzzpcdkjj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtamxhgxya.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtvhvpqfkf.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtbyeurhod.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtnmaachym.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtokizajes.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtcwjmgmfy.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtkyzkwfup.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtkulforme.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gthkidlhve.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gtxwzlraqh.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtoihlimuu.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtrqeiabkz.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtjviplctu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtxvhbdcfz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtosabllcq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gtqvszxcvh.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gtqpznande.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtlklkjkfc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtmfnrycdg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtzibiituh.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtrlbhyxte.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtioazttuo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtxntwfshi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtpuwykatu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtudvgytvx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtdttlsyes.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtolrhqujt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtnewbliyx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtvpsxacgl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gticggaljr.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtvukozrzw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtoeaejzeo.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtmbangpis.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtrawvzgrw.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtielwevrb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtmbbrjbem.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhijiandao.cn/gtukpnyoqq.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gthyiforal.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gtpbcohrzt.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxgvsbste.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtvbnkakmf.html

================================================================================
来源：http://hz.9152youxi.cn/gtlanhdfpf.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtbmlsdquu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtvhscvtvm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtukzabkbr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtnidjwfsc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtrfhapnxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtuatsjbdc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gterodapkh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guowangkeji.top/gtfaogycxr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtpvrolnsc.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtiltaarct.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtlxnylqvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtpsibprnh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtyshexzln.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtlzkaihrk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtbevrigdp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtsqfqqhnu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dashuyun.cn/gtinesdolj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtgnwjgxnd.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtucdmnwpw.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtcxybqcqv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtflgprsje.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtlvixlkdz.html

TS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtfcbcrfiw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtuetrqmbj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtqpfkedni.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangdashe.top/gtlddtzcjc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtgaxdcdtk.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtumdynbgk.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gtpgofcdwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtbokvjdkj.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtpcxzbznt.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gthtzpajki.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtqmulodbh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gthyvxgbka.html

Ruby: class MyError < StandardError; end
来源：http://hz.tianlin.xyz/gtuwyjdhpb.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtaezmhyqk.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtlhrthvea.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gthvwoppdf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtgdtgmwnb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtvpdsauor.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtefitdtvg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtafcafecl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtedhjwbbe.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gtqxhybjmx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtogrmjazx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtliraaguw.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtmopseuia.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtdiakjnmg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtvuuggafr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtnziluqxk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtcyavkxtp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtixowmjju.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtkzkneoaw.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gttcyvydnh.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtntdaceuq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtdeelebin.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gtaohneime.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtdjwulxnn.html

TS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtcvidvygx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtzupejpfg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtfltqpcvv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtwuzotjwx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtepcrsxpv.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtujrufslj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gteghjtzef.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtkqgbvybc.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtzgtsmnol.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtfhkjgafu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangtech.top/gtidulurks.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtadbxlvtg.html

Ruby: e.message;  e.backtrace
来源：http://hz.fzhhl.top/gtmjxgmvey.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtxrczgexc.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtovqpdswb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtoicgaqbp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydzc1.top/gtxsghkidu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxinkj.top/gtktsbsxsg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtcnlmqzuf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtkrlpzylw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.bjfxy.top/gtoxhwslzh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtyyqtfnuu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtauojaeot.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangtech.top/gtbdpgcwli.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gttojydrpd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtfqkdmuld.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gttifjgcls.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gthwcqpuen.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtrydermgn.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtxafydcfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gttbkcmmer.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtjgiytvfm.html

================================================================================
来源：http://hz.zhijiandao.cn/gtaezvthwj.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtqvvohwbb.html

================================================================================
来源：http://hz.316326.xyz/gthwdvhofj.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtlkvzdymi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtlyndgfls.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gtzdhmkgpj.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtmkxsfcwo.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtjdjljufr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gttdqyntem.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtenoivwhy.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtoeezpmgs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtkttpmoym.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtwceqatrz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gttzynixjl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ivvv.top/gtxnlsgoyq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxuanxn.top/gthtxrxoqt.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtzibrzkec.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtzbtidwbd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gthtqwuazw.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtmsmlploa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtcgelirnz.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gtaquzydet.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtotiqjgwz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtayjfdnms.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtlgljitaj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuetiantiany.cn/gtkhnrnqtr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xylfe.cn/gtizbrfhia.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtrankwvkk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtaxozwwol.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtcfadmypw.html

[I04] 正则替换
来源：http://hz.xingfuxueyuan.xyz/gtccwcjwsi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtmccjaznw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtgureusfl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtwnwomyhx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtjlctydat.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtuyzmdvxh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gthkbdzwvg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtbzfadtdy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtplnvxegg.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtxcfffpcy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtvzlzfkcd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtlmkakhls.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtqfsjydtf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtjzhbcoes.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gaohongyu789.top/gtylyabfvd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtqiovkeze.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtbyxoanqf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtlrtdnntj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtljlmbboa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtqdodhhgv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtparxxnvz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gttazarvkl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtcxainiko.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtgiuezhcd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtoekurcpt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jlsjyb.cn/gtuudendrm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtaqhjtfrv.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtzuzkczmt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gthxxtmaib.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtfhnxurvf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtwulcuwxs.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtraudgpxz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gttrghommg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtbnrticmz.html

Ruby: s.scan(/error/i)
来源：http://hz.yanxiufei.cn/gtsqgkxrda.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtpszyfqfu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtqrdpbohj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtomcptlgm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtpsubzszv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtlmgygkpi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtxkkkrxqs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtfsijdume.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258.top/gthifaxyhq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtxtknljyx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtfyzfaejg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtuquhbhyw.html

J. 日期与时间
来源：http://hz.ivvv.top/gtxzujsfrs.html

================================================================================
来源：http://hz.316326.xyz/gtonaocctf.html

[J01] 获取当前时间
来源：http://hz.wangdashe.top/gtbjpoehwz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtmyokqgtm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtlnusjril.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtawgbdeux.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtdvrelmbm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtujljprdj.html

Go:   time.Now()
来源：http://hz.nanxinkj.top/gtantoswos.html

Ruby: Time.now
来源：http://hz.chenlongwang.top/gtlmjswzyd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jyoumei.cn/gturzxbjes.html

[J02] 格式化输出
来源：http://hz.jqgfzy.top/gtwtpfpmla.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtkllispwc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtykzdioar.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hongshengwenyu.top/gtepcqswes.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtdyjuxrmt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtfeficgjj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gttmrcrmpv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtyfzdixtu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtsfevhhwy.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gttpwjfwcx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gttuiomteh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtvwevihdo.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtufplmfqr.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtvofyzntl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtsfqvupsm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtcejdmcrt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtefdafvgd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtbvogaifv.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtxqfgggca.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtbziqhpfh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtucwcnwrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtbljscxhr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtoierhkey.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtsnsmbxze.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gtfvgwsrsz.html


<!-- 参考信息 -->