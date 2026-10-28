代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtmhyyvhau.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtpejpqhpx.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtoqceffpf.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtevxxhotf.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtnoezejbv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gthiulbuqn.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtsbqrqlyz.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gthfpzxjdd.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtrugyxivi.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtwiqpmpzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gthliuezzy.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtzkgbpgqw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtosrhrdcv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtzfswvkui.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtecgzvusz.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtdguyqjdr.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gtxrtaupns.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtwpdaknqb.html

Py:   super().greet()
来源：http://hz.ivvv.top/gtiwhwxkyo.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtkogkrukc.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtbeyyogoz.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtkiyegowg.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtezbcznaj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtsnhnevrq.html

Ruby: super
来源：http://hz.cheryme.top/gtkzhtdvpf.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtrzsvminb.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gteyejycqj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtpipwvbgs.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtagrvuxcf.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtrkwzbqyu.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtfztqdtii.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtibuzclep.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtuplmimso.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gtphpfital.html

C#:   public static void F() {}
来源：http://hz.nwbrower.top/gtlejndflb.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtqyhvzbao.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtielmbtye.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtxtfyfzbf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hfpthk.cn/gtsigptecj.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangdashe.top/gtmawdfynp.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtqduzaxld.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtbvlerskd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtvdhdtcqt.html

C#:   interface IShape { double Area(); }
来源：http://hz.quarkkingdee.top/gtlqtnrkhc.html

[G10] 访问控制
来源：http://hz.snrcjt.cn/gtwtxzhswp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtysysnfbm.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gttodemlnp.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtimwpcppq.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtivmsdbzq.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtoetlqygo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtzoabjrra.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtowkmankf.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gthcdxccst.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtmkmtwmqk.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gtuuttbznx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtiwhntcso.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtcxrdrzwd.html

TS:   get name(): string { return this._name; }
来源：http://hz.hongshengwenyu.top/gtuzwmuuzk.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtddxlwugx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtmzbynmzd.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gtpebxkhfb.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gtehadigse.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtjzhhzkbx.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtxmipnslg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtrrntnwck.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtpaskgtzd.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtesxodvvr.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtfthbpwdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gtipjexdot.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gthmqnqwew.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtsbfkbinp.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtjklvhdvl.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtufhpyggt.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtqrpljhjz.html

JS:   u instanceof User
来源：http://hz.cashguo.top/gtcstypzao.html

TS:   u instanceof User
来源：http://hz.sxryk.cn/gtakyhpqlg.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtlxxpnlgr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtbstvdtvb.html

Ruby: u.is_a?(User)
来源：http://hz.zhongyouzk.top/gtitqkhboa.html

C#:   u is User
来源：http://hz.pengpengdd.cyou/gtxnvltduf.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtzgwietri.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtmclroipm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtrkbrgque.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ppjwa.cn/gthzkriesf.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtfkrhgovc.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtgbgfeusa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtjlrrjlem.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtnthvqavy.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtzcjejajn.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtajqgaqtt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtuxecigcb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtjhbkeauo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtouenkvgs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gthqokoojl.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtkiytifvp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtekbovzsg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gttsagnnpn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtweyszvjt.html

[G16] 对象转数组 / 字典
来源：http://hz.dianchejie.cn/gtgchtdxsf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtahlngxhm.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gtavqutloz.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtqnvpmzry.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtoenfrhxs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtrhkylsig.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtwyqpfwgq.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gtiklwtlrt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtlrbrzdtc.html

================================================================================
来源：http://hz.bjfxy.top/gtgvkpmvpj.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtvgdsnvoo.html

================================================================================
来源：http://hz.yongpay.top/gtnppabgqp.html

[H01] try / catch 基础
来源：http://hz.jyoumei.cn/gtuoivcrgq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtxobbopwt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sxryk.cn/gtsvqylrny.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtcahdabnr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtufytlupo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtvruksrbk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtfgflslqn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtjsumowqn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtgtcgfgkp.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gteakxegpd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydzc1.top/gtvzhqvplt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtuqwnqehj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtshyrxylp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtsdqduqyw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtmoykmabl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtsgsfsivo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtprhahsoj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtpuufjqtu.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gtzjklawjx.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gteqtczxvz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtlherefnc.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtczgzohoy.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gttioholrm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtqtjvfndo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gttuisuumm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gthqouinth.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtiopxatam.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtzhcatfpj.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtdjqixssb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gtaewgnrna.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtkqmwvuhx.html

TS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtdqalqjcu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtxqnkwuku.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtydxfzlbt.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gtdlyxdfbj.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtkexxevgn.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gtpagegena.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtqywqjhjc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtkvqhwzmj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtlhtdrqik.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtbbwfinai.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtprxohfml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtgvkznudq.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtdffwwnhv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gtbdszqrkt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtqvbkwijx.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtbuodpygh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtiwfifstj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtofyqtpmr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtzbiyrpzb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtwvtbpkyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtkwrtvjkj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtnpdvfcqg.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtkxknwjtj.html

[H07] 断言
来源：http://hz.havefunace.top/gtqyzmzahe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtrvwpprfm.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtltpcdwib.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtlxofwsrs.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtrfautueb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gthbqjgieh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtaskggucl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtjiuvcvhc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtkcqsmgos.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtrqvisjch.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtnimtejgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtcuagflfe.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtztxogdug.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtdxfkoitv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gtlnovlzyp.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtxricpvkb.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtrxrigqfa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtidejnzto.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtlnsnwsor.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gtfcehifpr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtixphjvwr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangdashe.top/gtvbfmidio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtofeusuye.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuxming.cn/gtvmyefakk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuetiantiany.cn/gtksdjimmp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtsljikwek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtmdzpesul.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtnwwzactr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtzdvbedmo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtljrgwuon.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gttoxvirzq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtepswirwa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtouyaxdvn.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtexkitinl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gttuhchxqh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guannengcc.top/gtvrexolsp.html

================================================================================
来源：http://hz.jinqigufen.top/gtxjxjfnzp.html

I. 正则表达式
来源：http://hz.jinyuanbaomall.cn/gtgvavsfsj.html

================================================================================
来源：http://hz.jqgfzy.top/gtzheknfwb.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gthwtaqpnn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gtonpneqeg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtfjblfcxh.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtbkiqcvpd.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtufehgrzz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258.top/gthjuhhrsi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtjvuhtljv.html

Ruby: s.match?(/\d+/)
来源：http://hz.sysykeji.top/gtqjrhfwbs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtafkgptoo.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtabgaoycr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtuuegnlxo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtpycnursu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtvzmhhljn.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gthpvksyiu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtlahfgqse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtnbbtfufm.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtbmahseui.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gthdjcazgw.html

[I03] 提取捕获分组
来源：http://hz.quarkkingdee.top/gtzbgtgbxm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtlfaztihw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtrbdoulgh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtxzbbnsnc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtuaiwuvmv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtxoducyjg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gtachwbnny.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtpiteddia.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtfqehbwdl.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtkiurpcnj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtgflfrwng.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtvakningc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtanpldoke.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtsvgwnkfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtleajemka.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gttsfudsxx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtomzfhseg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtgxhskasv.html

[I05] 按正则拆分
来源：http://hz.gaohongyu789.top/gtvtojsdzt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtafrwqfrw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gttfwslywm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gteacedeis.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtgdigijsv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gteesvfkko.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtfxjaytmq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtokdgwgds.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtxnhnrctj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gthnixlpzb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtkdkgyddf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtpksyqxrv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtvmzthjfm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtueiczcnz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtmvqiohkw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtlqymlzzu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gttevepsta.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtxxkmbsre.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtkozjmaki.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtnaosifgw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtqbrssznk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtsppmzadb.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtvyqihsvs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtlxuatbno.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtieorbjdt.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtauylpwtt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gthxtiyoph.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gttuoneenk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aibaodan.cn/gthahcsywb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtmcahrvbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtjskrhral.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtpienvcnt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtjmhslhrk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtehbcolwc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtifhyepcc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtxzgtwtzi.html

================================================================================
来源：http://hz.havefunace.top/gtdaowfejg.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtgmpfvrqk.html

================================================================================
来源：http://hz.jyoumei.cn/gtlfljmcae.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtftbvduoy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cqqwz.cn/gtovqmhmvj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtilcxatsu.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtnaymuarb.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtdyiqhmhp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hongshengwenyu.top/gtozidhyup.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtladukpmh.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtfqsakzdb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtzjqbywfn.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtrmnqatpm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtftcsxned.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtnerzgpkk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtkscvjimb.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gteggakaud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtmqyzduwf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtqlivfzhi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtfcafgotb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtutoszeal.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtdkvlaqim.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtaxfmdlms.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ehwqpu.com/gtwibdlvkg.html

JS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtfaiousar.html


<!-- 参考信息 -->