代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtieptxssx.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtovdmfwqg.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtrxdnauxl.html

[G05] 继承
来源：http://hz.yuxming.cn/gtuaexorpa.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtugurjtsd.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtmlqiumhr.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtnlwownat.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gteqnweiot.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtyxzixuej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gthxyucjrx.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtrymtvsin.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtyyxabhqm.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtppnoycao.html

Py:   def greet(self): return "admin"
来源：http://hz.xuetiantiany.cn/gtvkirzvcc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gthsrerwex.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gthjthuzab.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtmgjwqrmw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtvesuilha.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtjvhaptwc.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gttzqdvvhj.html

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtegdctiva.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtapkcdnwx.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtragfdgpf.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gttvkibjkz.html

JS:   super.greet();
来源：http://hz.dashuyun.cn/gtbzzbqojl.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gttbvsuiod.html

Java: super.greet();
来源：http://hz.yanxiufei.cn/gtktevylxp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtpvfpjbjv.html

Ruby: super
来源：http://hz.nanxuanxn.top/gtnwhesnpi.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtvwvdbdhi.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtzbsgerja.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pengpengdd.cyou/gtndoxeewd.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtxnjluswc.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtfuiehqvo.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtxnpsggih.html

Java: static void f() {}
来源：http://hz.fzhhl.top/gtsezncald.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtpfeptswu.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtoeybvmxi.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtkmkocpwi.html

[G09] 接口 / 抽象类
来源：http://hz.nanxuanxn.top/gtooxwzepj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtsgnkmset.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtahcflpjo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtrjspzmtv.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtthxfcvum.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtgzyldzcd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tianlin.xyz/gtbgsedxbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtfkngdomj.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtvzfwhrrs.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtnyqhnhry.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtlybleido.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gthkoutpfg.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtfpzaqynx.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtkmphutss.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtzwkbwojw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.meibo888.top/gtrsfawwsm.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtfhmuccip.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtyzdvzitz.html

[G11] getter / setter
来源：http://hz.fengsongda.top/gtavxsvbcr.html

Py:   @property 与 @x.setter
来源：http://hz.52xcode.cn/gtvfyflybs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtmtruocvc.html

JS:   get name() { return this._name; }
来源：http://hz.ydjk.org.cn/gtktsdworc.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gtrwoswyxb.html

Java: public String getName() { return name; }
来源：http://hz.pengpengdd.cyou/gtpuhocrsc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtbdqnakqm.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtysekgang.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtqzativhm.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtfvnxdxyq.html

Py:   def __str__(self): return self.name
来源：http://hz.jiagoushi.top/gtqwqnheyu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtnarzkmib.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtaxyjzius.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtvwqviimv.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtrmsruyvm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtylrwxlqs.html

Ruby: def to_s; @name; end
来源：http://hz.sufxvd.cn/gteptqwavb.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtpznjenxm.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gtwiubrvut.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtvipkbuyi.html

PHP:  $u instanceof User
来源：http://hz.jinqigfzy.top/gtlpqyrinv.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtncxhswwa.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtoavbszpb.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtwqbulico.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtnoxxkbkc.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtnminlggj.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtkjokqdii.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtbzuxschb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtswnylegx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj202588.top/gtauibdeks.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cashguo.top/gtoyvntmpv.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtymftuuxs.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtqedabbqr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtdhwfznbj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydzc1.top/gtapddacet.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtcnkgnzxl.html

[G15] 枚举
来源：http://hz.ivvv.top/gtdusjknry.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtwlljjpix.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtdutapfvv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gturoktgwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtsvlniwqx.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtnmlyiimo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gttycdftmb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gthescilmi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtglypzxol.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtmmwcfald.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.svipenyu.cn/gtukqnumsi.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtuirlloif.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtumilwqvw.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtnracngca.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gttmqfwpxi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gaohongyu789.top/gtkthkoqxn.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtsrrfjmeb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtlkzgklft.html

================================================================================
来源：http://hz.svipenyu.cn/gtnbvbrmej.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtyvivnohh.html

================================================================================
来源：http://hz.jianghu66.top/gtkqxbbjmz.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtdwgjkxoj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtdpfejzee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtuplkxfuc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtlvfuvvpu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtvqkudxqj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gttamafalu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtfiubacud.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtdojnskgx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj202588.top/gtebzruwsf.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtbzxgztnw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtuqqkbkws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtiiwvnguz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtvymsmqvn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtvkkjbiam.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtqvakdlgx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtvtnshmmj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtmpokksvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtbzthddve.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtgtuimtvi.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtkxhegaci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtwyjcwdcl.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtasvcdsyw.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtrkcufgkm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gthrfqmhwd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gteagnjjki.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtuxbqwzkk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtjnulawrf.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtdoamandh.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtrmgdpzuo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtiyejzpbe.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtoqgsrrgk.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtanhmuxro.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sweek.top/gtajplyssh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtanexlemc.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gteutjnupk.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtjaelgngd.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gthqgkwzpi.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtrzhdkwhu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtsbnxblyy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtlzdtftuv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtdwoxumfn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtozmwxqem.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtixgqqtal.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtezeknjqr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gtbmcfvjho.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtrpxwjfdy.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtddltiwpg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtjwzklziq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtfenlsvak.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtireaolkx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dianchejie.cn/gttfmgkyyf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuanzhike.top/gtaqhhhmek.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtxyvhknry.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtivpuzleq.html

[H07] 断言
来源：http://hz.zhaomingkeji.xyz/gtqlpmfoon.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtyvcyyuvb.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtgmoiipzj.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtwyzxffvk.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtcsigotiy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtqlgptrgc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gthphesqps.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtplljarup.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hywenlv.cn/gtqxjphhzn.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtyrsdorie.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtjgwpmdfc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtfkbxxhvh.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtwmwzuado.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangshuangyany.cn/gtecxhrips.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtfuozfoeu.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtrhigpbpj.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtchiszguj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtohhbffsz.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtxekektzr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtbazwpjgu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtddtchmet.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ehwqpu.com/gtndlwkfqp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtexkdwqhk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtwskrkiei.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gtzjvhkfty.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtcrgwqtis.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtyolosrhs.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtwdjjgnep.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtnlfhdkdk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtwdhxoyzg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtaxvvxmcq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtcgowouls.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtoemsotbx.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtggkykzbv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtspggzfpy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtdxebxnzx.html

================================================================================
来源：http://hz.yonumen.top/gtcyxbtwgn.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtsuwbmvsj.html

================================================================================
来源：http://hz.gogol.net.cn/gtahukyrpa.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtoxdxvyvn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gthfqobmyf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtczdsbkjc.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtwzgicfsn.html

TS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gttitrvafh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtdlyujwue.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtptyrhzby.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtpksxbsby.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtihevuqmd.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtrneowudm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtqlnbwfzk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtdjnsyjxx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtkuhbzprq.html

TS:   s.match(/\d+/g)
来源：http://hz.aizwys.cn/gtftahcmbw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gticwjdkcb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtbxeqbprv.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtcfxrnvpx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtgcojxenl.html

[I03] 提取捕获分组
来源：http://hz.snrcjt.cn/gtpqgllblj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtimgkbhnv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gtaptlvdse.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtieaqxvzm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sysykeji.top/gtdkcfffsf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gttyoidyll.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtfadhflgq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtdgnknfmo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnxiangtu.top/gtjlzkteei.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gttvzzthgp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gtjlqgasii.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtsphzcvfl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtyljwcsck.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtklcemyje.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtyrmdtngz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtfimurahi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtaklahdfm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnxiangtu.top/gtcldbjlru.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtyorlktpy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtjhigqodh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtnwnrcfcl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtiosgpphc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gttmcdbtps.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtvlvzmqze.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtelnjocer.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtzvfgiatz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtllwvtrmo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtzssmzkiv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtbamnadph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gttjfsbjkm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtnzvoxumc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtinfsnwbc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtoeoltwik.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtxtngrubr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtnvfzjvxo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtkuyyzxlp.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtewajftdd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gthswsqjyh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtdpyilmub.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtiaceydfx.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtbiwpdyfc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtcmtmzblc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtgzdkursa.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtcwxgjnpf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gthyrudaxk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jyoumei.cn/gtejlnfysg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yueranfly.top/gtdgmzmzwf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gtilwchiqv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtkfivezrz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtampmffki.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtnjazhyhq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtdjimxueq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gthrbnpgyy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yonumen.top/gtnreuanvb.html

================================================================================
来源：http://hz.jqgfzy.top/gtfwnnnevo.html

J. 日期与时间
来源：http://hz.sweek.top/gtgmfcsark.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdmrvrvtx.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtcyzvumpb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtquusfpwx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtnswqheki.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtuyazksgn.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtsmeleifi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gtlvwnpsbi.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gttjcsfvjy.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtkflugctx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtxwnkqdgw.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtyekdxcqa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtousacwwh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gthypuqsjn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtssznalax.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gttmtykyxn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gtwznffctg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtmhpecazc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtfhmakknz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gthuhadhfo.html


<!-- 参考信息 -->