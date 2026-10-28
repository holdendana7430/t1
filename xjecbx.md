代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtbrrgnsnd.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtzhtbqdng.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtfwqcyncd.html

[G05] 继承
来源：http://hz.shuidangran.top/gtsjigkbgq.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtzulnjyjj.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtqmbveykb.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtaofbvxav.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtprvweuks.html

Java: class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtqkqadpqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtbrratfiw.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtyfnyckwk.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtdwhtdcuv.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtnqcdiqqp.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gtftsayhxd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtrdsdturj.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtlmugixlj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtnxigqbxn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtrqchtekc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pycfn.com/gtkzfkssrx.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtpfunuech.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtzwevsehn.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gtegstnnzb.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtfhfvmqfj.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtmlbumtyw.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtakffxkcf.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtaasmbuwm.html

Java: super.greet();
来源：http://hz.c1oappe.top/gttojwdenz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gtgpkyjfzi.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtdrrnokqk.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gtvdnwjzfu.html

[G08] 静态方法与属性
来源：http://hz.gaohongyu789.top/gtigujvkiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtnmivrepm.html

PHP:  public static function f() {}
来源：http://hz.hnqzz.top/gtbqvedzhl.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtgvsaviwr.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtaseujsvd.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtzpuuiozo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pycfn.com/gtvowdeous.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtnucalnpt.html

C#:   public static void F() {}
来源：http://hz.c1oappe.top/gtsqywynqm.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtfbvbkpcb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtcfpvaaur.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hywenlv.cn/gtcrsbrgby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtclsxbmyo.html

TS:   interface Shape { area(): number; }
来源：http://hz.sxryk.cn/gtvahoqgck.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtfnfdgrjq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtavkgkdam.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.iojbl.cn/gtlrwlsqok.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtexestvnf.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtoeysnaem.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtclpxvntx.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtivcadxkz.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gttbrjwenm.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gturrzcjil.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gttcatnxid.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hfpthk.cn/gtpavsmqxt.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtsfczhijs.html

C#:   public / protected / private / internal
来源：http://hz.tanke756.top/gtcdnoazki.html

[G11] getter / setter
来源：http://hz.havefunace.top/gtmbqnrvqe.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gttlgbxire.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cheryme.top/gtgugzeubv.html

JS:   get name() { return this._name; }
来源：http://hz.ehwqpu.com/gtlnllxcvj.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtzkwioniy.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtqofyhykg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtbasqubwd.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtzgloiiuc.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtxglidfdp.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtzjevgkmk.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtsztpeact.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtqdcoaqhl.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtzegdxjwj.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtvwbsxwzo.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtqhpiekys.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtshnxijuq.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gtfjrwpfdu.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtalaaegwy.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gtdorcrgxu.html

Py:   isinstance(u, User)
来源：http://hz.0kj1m.cn/gtktpqwexy.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gthlumipsw.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtxxfxqzxi.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtaefunhba.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gtswgpriqb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gtqkelnjtq.html

Ruby: u.is_a?(User)
来源：http://hz.hywenlv.cn/gttuqvmjip.html

C#:   u is User
来源：http://hz.yj202588.top/gtvrjgmgrm.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtuhpfgyln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtdwrdsvcu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtfjlupica.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtfefhlyxp.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtxpvrleqo.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtaxmbpbcw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtytoqnsqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtnqwgqmdb.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtoqgjfkdi.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtoykrnjdl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.feifeiyinyue.top/gtgsxnzxpj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtsflwdliu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gttlbkjktt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtrvgtxjpi.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gtsidncjav.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gtcpvlsynn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtdkmhhwpp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtmhwfwste.html

[G16] 对象转数组 / 字典
来源：http://hz.aizwys.cn/gtsidudcrg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtvftvmxmm.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtmmsercvk.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtyiqbsaxh.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtsscosmus.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gtqgawgawk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtxpeqqjqq.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtkwrbkbck.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtwqbwhcxi.html

================================================================================
来源：http://hz.sufxvd.cn/gtgcrditwo.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtzrfvfhyi.html

================================================================================
来源：http://hz.gogol.net.cn/gtgjwvqcou.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtgxcwyyxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ywan-chungtsiang.top/gtpooiwswl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gteeintwaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtaichtzxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtjojdsaal.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtbkhpmmxa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gthajfotgu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtipftorui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtbnpkymsv.html

[H02] finally / ensure 收尾
来源：http://hz.cucudq.cn/gtvoauaipa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtjroepxii.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtkjrpyrps.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtmkpgbzpu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtibyoudiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtgqopduyb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtsbzeoeyi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtdunzwgiy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtqgtnhbfq.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtdvmzmpmq.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtnfkohopi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtgyuxorxa.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtzzhhsttj.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtrfjayydd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gthyhqpaer.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtvzlifqjy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtyosgkeac.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtglinwzhr.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtfwegzuyd.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtebakqnju.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtgpydfakr.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtfhxkytkz.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtlmnjydvz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtetbpzfcg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtfgdtoxoa.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtmmdalljd.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtoghfhpfm.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtzlzzjfjn.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtpujjqkdn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinghuilouyu.cn/gtuxuwommc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtjwoztvls.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtrdizghqi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtqrikejve.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtizgdvwmu.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtqoxvdztd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinghuilouyu.cn/gtuzuvhrja.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuanzhike.top/gtvdcmzddu.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gttnekwdqw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtmqoyjqia.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtjvxehfts.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtiklcehzg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtuvplxngg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtpncnbatj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gttijnslck.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtnulruzax.html

[H07] 断言
来源：http://hz.yj20258888.top/gtstrhuidb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hongshengwenyu.top/gtujzqparz.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gtsggbuxjg.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtslqwfwab.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtntcpxdnl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gteactdwkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtwtnpdsig.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydzc1.top/gtcmqcoxqb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtmwrtncsv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtszblgvte.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtmprxjqsz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnxiangtu.top/gtokvaeqlh.html

JS:   e.message;  e.stack
来源：http://hz.quarkkingdee.top/gtjfunerev.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtccsfzhhn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtotuehwqm.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtphllhter.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gteihsmyjs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gtzckmmagj.html

[H09] 带错误码的异常
来源：http://hz.guannengcc.top/gtculiazwc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtzypbqvxg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtzoxrlyuq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258.top/gtrelnpjdd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtmesffbjd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtfwcdwriv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtlyvodhmd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtwcmdsydq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtanvivnem.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gtoglbrtkf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.meibo888.top/gtjvcbcfty.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtbfjagyxl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtpgkemsqg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtzoeqzdas.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtsmphtdmd.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtvdonrljn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gthecsgqxj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtdrlzbqxz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlaelqxrs.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtaqborjas.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgefetpjz.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtcmfajjam.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtxgmikksy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtattodvri.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtrdzjaqep.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtfijsasue.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtxkmsutvc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gtlqmoveza.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtjcxpafgp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tanke756.top/gtpiqnmnbm.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtlfcdrvbz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtdkxdtogg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.vqdsnc.cn/gtmwofhpxf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gttgfglblj.html

TS:   s.match(/\d+/g)
来源：http://hz.feifeiyinyue.top/gtfsexgkrq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuanzhike.top/gtqnqwaowm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtepfvriim.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtxzyvsfkq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtqfqpnvni.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtxeinhevc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtoxgtavih.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtoakgaccz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gttfkluhtz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtkghadhft.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtxrwjfilr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gthpiaqluw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtsxioxsal.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gthmwxnxkl.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtigkfcflo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gtuuudexvh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtqcvkilbx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gttcaerwpu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtaigmtjuu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtheckjmqk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtsgubynxy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gthhyonhuw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtoatwllyc.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtxnrfgann.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gteapnkuya.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtszrytpdr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtdzvobfuy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtqbqszxyl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtpczsjqiz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.0kj1m.cn/gttfqvoajh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtpokbwnhw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtunjadoce.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yongpay.top/gtenovcptq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtkzilrcyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gtofrkatmc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtithknjza.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtolpvfxgw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtnmfaismi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtdhmgdnrb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtcgajcuul.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtpwplhvsq.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gtvgpmnacl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtumbpxvyf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtymnnbbcy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinghuilouyu.cn/gtrqkvknyq.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtxdqvntrz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtyixtgnrx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtvuztffdb.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gteohgioak.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gtvewotzkg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtzmucxcxh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtcxoflght.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xylfe.cn/gtuvevgnyw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtvdpvnhuh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtuzrwynmu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtlrzjtuzf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtvlznjnwo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fzhhl.top/gtoqctaojx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hongshengwenyu.top/gtncilkprv.html

================================================================================
来源：http://hz.nanxinkj.top/gtopddvnyv.html

J. 日期与时间
来源：http://hz.52xcode.cn/gtwosynntd.html

================================================================================
来源：http://hz.cheryme.top/gtyipagrfz.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtwvtczolj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhongyouzk.top/gtomqzwjtz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtmopohkvp.html

JS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gttgarztyg.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gttjoxxjwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hysaishi.cn/gtuleilbiw.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtokxcxqxi.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtdyqrplpi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtzeynsjxg.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtgpnnniiz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtdgzghecy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtcenzkmcr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtaqmjuyzv.html

TS:   d.toISOString()
来源：http://hz.nanxinkj.top/gtdsjxpmtz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtoipffowz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gogol.net.cn/gtbzmyttew.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtkjwakcrg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtovirhrbl.html


<!-- 参考信息 -->