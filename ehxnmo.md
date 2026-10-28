代发 wailian999

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtlvooseml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtcjlrufqp.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gtllxgyiqy.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gtryiqrdst.html

[G06] 重写方法
来源：http://hz.tanke756.top/gttivabpti.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtnunewpxh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtkkjlgurk.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtkuvaxtyw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtiexllvls.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtvszzayqd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtiseqvxyl.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtlzzdriow.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtaeynkwwb.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtlhhvrubb.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gtrnutftuu.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtkpkmhgyb.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtmjfwklcx.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtylededxm.html

Java: super.greet();
来源：http://hz.svipenyu.cn/gtanhczdue.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtpcrmgbon.html

Ruby: super
来源：http://hz.xziqi.cn/gtlcygviuj.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtowyhwbuc.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtnxgjzauc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtpsrpixtu.html

PHP:  public static function f() {}
来源：http://hz.jinqigufen.top/gtsrnsuwzt.html

JS:   static f() {}
来源：http://hz.vqdsnc.cn/gtprmqujat.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtjtccpkkm.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtjghjzska.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtifkzokhj.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtsgeuveub.html

C#:   public static void F() {}
来源：http://hz.cashguo.top/gtyllytcsh.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtakgbxelv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtjqpcourv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtmnlsfrul.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtugmbbzir.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtxfpqdsaa.html

Java: interface Shape { double area(); }
来源：http://hz.havefunace.top/gtcfbhiwor.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtllbbwufg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtmkemzukz.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtvhoiuvqi.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtgaxwjzsy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtavfiqljt.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtjkhkxrmo.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtblicbmnp.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtzgdzcrse.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gtiscxwxrk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gthkzgvauq.html

Ruby: public / protected / private
来源：http://hz.ppjwa.cn/gtzberhkri.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gteseivnlt.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtjtybseqb.html

Py:   @property 与 @x.setter
来源：http://hz.xinyue.icu/gtpanmjnnm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.meibo888.top/gtemyhnyzo.html

JS:   get name() { return this._name; }
来源：http://hz.ivvv.top/gtrcioatgu.html

TS:   get name(): string { return this._name; }
来源：http://hz.shangyingyoupin.top/gtnbkaajaz.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtrcxkidkr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtsonayfjp.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtdozfwbms.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangtech.top/gtgfawcxek.html

[G12] 对象转字符串
来源：http://hz.guowangkeji.top/gthzkvnuba.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtcadvkfsa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tanke756.top/gtluhifnwa.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtnoebvfjw.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtlovyaphp.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtykzccqul.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtsllwqzhc.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gtkzuzyaea.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtnntiqwfb.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtvzuenguw.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtdtcruvst.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtdkycrkqx.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtjtjhoole.html

TS:   u instanceof User
来源：http://hz.cashguo.top/gtrsydyspr.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtugbghvau.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtifibjwdo.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtwvagxdex.html

C#:   u is User
来源：http://hz.shuidangran.top/gtyxqyujlj.html

[G14] 数据类 / record
来源：http://hz.yuxming.cn/gtikzppjln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtkvnrrpnv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tianlin.xyz/gtcmawjcnm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtzmmdfaqg.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtzudwdfim.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtulhjwiuz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gthpgmtyij.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gttctdxyde.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtlanxehkw.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtdwolbyxv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gttavlyfcy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtfdjulanw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtonoykdrr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtbngkkbwy.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtaexhuttm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtajwsucsx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtwjewmvyk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtiwrqsynj.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gtkhgayugb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gtjtnofzun.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtsvflyxod.html

JS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtdrybxxdy.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtkecbbczh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gticlnlttl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtkcmiwtuf.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtposfbusz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gtcslogwur.html

================================================================================
来源：http://hz.yj20258888.top/gtfbmskhkw.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtonaqgrjy.html

================================================================================
来源：http://hz.cheryme.top/gtzpccbqmq.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtipmpptuv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtkhdvwuui.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtkwxhdsgg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtcowdpgiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtslvbrtuy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtmmervffy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gturqeljll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtikmizscb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtdtnpjaos.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtimnnsjmy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gthdwlibyr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtkoiamlwp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtlnjiamrx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtxwomqjqr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtrkzgdcna.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtccmemipi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtrguzdpac.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.havefunace.top/gtnjfmaqjn.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtsgcjkpmu.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtucgwtrqq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtkhxqomal.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtbluuqgcd.html

TS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtmvjndxqd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtxtvteyso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtvmbsdsuu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gthgsobcix.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtvhmstbsa.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtttkskeuy.html

Py:   class MyError(Exception): pass
来源：http://hz.yj202588.top/gtzadqprsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtpctgvwhh.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtduumdbsv.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtrgphfwbw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtgbnaswhc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gterrwywmn.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtdlxsmdow.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtrnhxeimt.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtqtfzyirl.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtntszqkfa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.feifeiyinyue.top/gtwzvyyduh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtzrcileco.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtgffngrra.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtzebkdlnn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gtxjqvcyah.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtvjwmpzse.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtimatmxpe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtcciplsin.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtlbpkkilx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtwnxvtfzh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtgpusndik.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtpbqetdye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtnstivwyr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtuefaztjk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gthpufutsg.html

C#:   obj?.A?.B ?? default
来源：http://hz.quarkkingdee.top/gtthzwzyoc.html

[H07] 断言
来源：http://hz.xuanzx.com/gthcglgxwl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtgxitzhoy.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtgunudilv.html

JS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtnteknzyd.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtznbpfhyl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtuhqtjbhj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gthaqnawyp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gtencpvbby.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtyuvutfut.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtuljtzfxv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shangyingyoupin.top/gtkinlhxgo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.vqdsnc.cn/gteixtyudl.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gthaueehon.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtfgahxsjd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtgneszqkb.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtdrwhluvr.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtnxaaalpi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtcoemwhnj.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gttsfskpdo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtazqmsite.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtjimmlmiw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gtfsspxpke.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ybcxt.top/gtfsfbpvsz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtfhsqahxy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gtdyhxowxg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtqdltxbyf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtzxoslvkl.html

[H10] 资源自动释放
来源：http://hz.0kj1m.cn/gtdbilkpst.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtosgtzgex.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shzxlz.cn/gtrtxenrdv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtxcpicmed.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtyltukjne.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtznejiabi.html

Go:   defer f.Close()
来源：http://hz.ywan-chungtsiang.top/gtjcdlahsg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtbvvuylib.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtbxmphnwf.html

================================================================================
来源：http://hz.gogol.net.cn/gtwrhtjzfn.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtuykpavxw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgmwaugom.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtwddhqxxo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuanzhike.top/gttlihooxu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtkekqeajv.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtgbxwabsr.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtefqthswe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ppjwa.cn/gtmqcjqflc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gtjujhqrte.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gttsgjxcwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtwsmwthba.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtbejifkjj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pycfn.com/gtzyswxbji.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtwuwnkzva.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtdaihrqbx.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtsmanjybv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.snrcjt.cn/gtnnwyrynz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtmfrmclyp.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtwrtakppq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtliqucwcz.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtnpojyfpc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtzaetlctn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cqqwz.cn/gtfwntthll.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtsfyaqqxg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.andypj.xyz/gtuqftzyce.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtxvmiokgi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aizwys.cn/gtbeyzbzgx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gthdafejfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtisqxctuo.html

[I04] 正则替换
来源：http://hz.fengsongda.top/gtplxzcgyg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtfjydjedn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtogyclgkf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtiajftmwo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtsklsjyeh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtcmjoaqzx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtsdcxzary.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtypcbdomo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtpbwykhgb.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtgsfdaeil.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtwniyhfun.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtpjftvumo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtvnzsguos.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtodxjvmzm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gtbyysplxf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cqqwz.cn/gtuleiwjcp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtsbpwneun.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cashguo.top/gtlpibsocl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtdgtiikao.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtyyyotptc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jiagoushi.top/gtbxfjottd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtykzcrynp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtavjvpfte.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtvzecrxwx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtybqcuopl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtzfmiqybw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtlatmxztg.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtaqyheakf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtbztwltvd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtepxkkuql.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtleevvtrj.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtbminnoax.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gtqmrcwolr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtivuzdthu.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtgupqncjw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtdmaigimk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtpzaslqsg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gtqgvtsmlw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtqeyirpgi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtdzgzrqpf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gthqljwwhq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtscgwifcq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gtocmmivni.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gthurygugp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cheryme.top/gtrymmucql.html

================================================================================
来源：http://hz.xylfe.cn/gtmkhdrylx.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtwqjfspbr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjtmspvaa.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gttmeaeydh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtypjciyzc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtztvdruiu.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtzugwjdby.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtmijiotqt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtfvknycov.html

Go:   time.Now()
来源：http://hz.sweek.top/gtfstsntbl.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtawlsvtyg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cucudq.cn/gtujmtcerp.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gttdhohvek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gteszndhbs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtuwupdsfh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtmplaymlf.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtuhajwezo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtpdvsdagt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gtgyvvjdvm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtletgdbqy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtmoenznta.html

[J03] 字符串解析为日期
来源：http://hz.wangdashe.top/gtdmnrovvp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gthxrluxnf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtbiifowrq.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtrojltjuw.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtfdoidhoe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtstrzvtul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtrudmgclg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtbffbglri.html


<!-- 参考信息 -->