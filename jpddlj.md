代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtjzkzljwx.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtslqobeyb.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtlqkftdkk.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtybknrgzk.html

Java: class Admin extends User {}
来源：http://hz.52xcode.cn/gtfvgccbhp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtoemijktf.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtpkftgjqe.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtffxebbcg.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtoezvjusx.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtcnqxuhgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtkfyshytt.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtrivbjqkr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtvammawbj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtsqmcsjqv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gtpkbabykd.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtjvkusvah.html

C#:   public override string Greet() => "admin";
来源：http://hz.fzhhl.top/gtkweraurs.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gtuojlnrjf.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtnfcjwijy.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtziawxeah.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtmdcpbzjj.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtxntchdai.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtelagqnji.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtvxmshvgn.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtvwdxkuwm.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtfweadotb.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtfrmzjcss.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gthnhcukil.html

PHP:  public static function f() {}
来源：http://hz.yangfankeji.com/gtjpppmbuf.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtyeezeafs.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gtikxjirtr.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtbjftzncl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtbcysvnty.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtwylwelwf.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtzyzothee.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtlgmylfpx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cdnleiting.top/gtmoctkmzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtvrmkqtgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtnicnspxt.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtugdjissp.html

Java: interface Shape { double area(); }
来源：http://hz.ydjk.org.cn/gtupmowxtf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.birdmap.top/gtddctvpnw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gtebhgnafy.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtpxuszjkx.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtebxoatjd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtydslebhj.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gtvxyiileu.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtgaqnowag.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtymbvbcps.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtvlduppfw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gthucbaudj.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtjdivaasq.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtchctwwjg.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gtaukuqxpw.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtlycnlupu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtsmlaaijh.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtsjnwdqab.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtyensngmc.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtvmepeoec.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtzkfkyemd.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtaqfzgfcp.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gtyuoixfyo.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtpsofzrez.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtnvnhtwov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtzungkikw.html

JS:   toString() { return this.name; }
来源：http://hz.haohaochexian.top/gtbphzmrfn.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtnmkspiff.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtbaqqcrrb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtzyyjempd.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtiznvqbxc.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtbdmsryff.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtdkoymogk.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gteljbwvuu.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtcgetsale.html

JS:   u instanceof User
来源：http://hz.guowangkeji.top/gtydzrwcjx.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtwvptidgi.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gttbxfoenu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydzc1.top/gtrixoohxp.html

Ruby: u.is_a?(User)
来源：http://hz.zhongyouzk.top/gtnttvlesy.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtevfgqnjg.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtombsunqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtypktfgjh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangshuangyany.cn/gtsqmzcmkt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtacyzbbsp.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gthxfhcjma.html

Java: record User(String name, int age) {}
来源：http://hz.daria6918.cn/gtldstcorg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtsmnkmsbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtanvgyhpi.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtbcxeepeg.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtvqlvbtow.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtmcakdhek.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtvtbyompa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenzaomai.com/gtjvnwlnjl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gttwuwliwm.html

Java: enum Color { RED, GREEN }
来源：http://hz.cdnleiting.top/gtqdeuifdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gtcxntzcnh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.svipenyu.cn/gtgikcjdqw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gttoiffxgy.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtbmnsglck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gtjqxgmxqn.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtsrecocfe.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtqgkortok.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtlxzkidyj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daxiang520.top/gtozshrquh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gaohongyu789.top/gtugamptuk.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtsciulypb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zycfv.cn/gtkpramnbl.html

================================================================================
来源：http://hz.jiagoushi.top/gtvlusjpdx.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtlysrhfeq.html

================================================================================
来源：http://hz.zhengqikj.top/gthocanyko.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtrxqerztg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtgakvcirb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtzlcnzvev.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtrclbkjqt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtfksdosbb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtxerltxgo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinghuilouyu.cn/gtuhwluguc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuetiantiany.cn/gtrhbpfgup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.iojbl.cn/gtisnezaic.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtvvqqgppl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gotoacloud.top/gtpoyvqdtq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtxcdwhatd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtvazsdlki.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtimtwdcgs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtfppaecdp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtxhzmhtdi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yongpay.top/gtsrykwjnh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.bjfxy.top/gtzgiprjtp.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gtwlsfjyso.html

Py:   raise ValueError("错误信息")
来源：http://hz.xinyue.icu/gtwokfoxmq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtfgasjbaf.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtdeuuqvly.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtjcthgdsk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtqlntvucy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.quarkkingdee.top/gteccrugyg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258.top/gtdikhclky.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtmbxkamnw.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtafpbwujz.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtxwzptwsw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtiyjpcpgl.html

JS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtqubdnlzr.html

TS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtnknygbul.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtuhlhyhpr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtzsxtaelj.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtjskavvoy.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtyewdvdlq.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtwndunuoc.html

Py:   except ValueError as e:
来源：http://hz.0kj1m.cn/gtrccroqqg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.bjfxy.top/gtbvopjjxo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtfbthsmtp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtxkgelkcr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtrhkqibgp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtqlikuozs.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtefwfexlv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtnnuxduhe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.c1oappe.top/gtpsujnipb.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtwruxspkx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.meibo888.top/gtrtnmdfhd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtujifzfvl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtohayxmju.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtrhvsiycb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtpofpbhpx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtezjfzxeb.html

C#:   obj?.A?.B ?? default
来源：http://hz.bjfxy.top/gttxuxcsvh.html

[H07] 断言
来源：http://hz.yj20258888.top/gtokoidvqf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtokwcoexk.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtizvocsgq.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtqagibyqn.html

TS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtivrhodft.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigfzy.top/gtqidjjbar.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhengqikj.top/gtfrryskbd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtdewodddy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtjjrdjbzz.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gttazkaset.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtsmomospz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtrbldhoax.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtramnkxrw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtzfrsltri.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fengsongda.top/gtrgzahpab.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtkalcjmoo.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtxguxmgks.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtcnerkmil.html

[H09] 带错误码的异常
来源：http://hz.zdqjudy.top/gtxbdffunn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gthtnspdom.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtbvwugvis.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtildcpsuy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtclgfwuqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtfaykfesh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cqqwz.cn/gtfwmmmaau.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtludqgrxl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtmwxpwkqj.html

[H10] 资源自动释放
来源：http://hz.quarkkingdee.top/gtryhkqajl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtcweibjev.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtnlxdoqku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtixyxwokh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtlncacmyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gtdpukwroo.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtnfzzsxze.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtajcibrzv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtjxeplmeq.html

================================================================================
来源：http://hz.ivvv.top/gtfswusyew.html

I. 正则表达式
来源：http://hz.jinqigufen.top/gtvogvmjbi.html

================================================================================
来源：http://hz.yj20258888.top/gthqtpnfjr.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtmfgbgkvn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtpnydytqj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtwdjnfcag.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtxnrpsuhy.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtvcagpuzx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtorjeuxqm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jyoumei.cn/gttuyqdsph.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtguywoygn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shangyingyoupin.top/gtueuqodhi.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtmeptmljw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtjzhzjpip.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtklaovakk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shuidangran.top/gtqypqrigz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtorsjgnvv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gaohongyu789.top/gtxbqetudt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gthmagjzwq.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gttldukoei.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtgupilceh.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gtfrkjthdb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtjcmtlofq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtrqqxwvko.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gtxybkvttg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtckhfhwrb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtaxwaqhxj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtvvflfpsk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.havefunace.top/gtlpybghgc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gtfluhjgqh.html

[I04] 正则替换
来源：http://hz.sweek.top/gttzjzsydq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hongshengwenyu.top/gtxxucznac.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtlfoulxmm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtrzqufity.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtowgmofaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtgibpjqkb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtbmclgzrh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtkwrgpfpl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtesdcfcil.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtbotxmvss.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtpxykebon.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtijegezge.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtbdefxgzg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtrcisbopf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtpxomoonf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtjebmdjlz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtuuihiiac.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtatyhuiyl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtipzfakgm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtlnyqrdse.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gthvzmwhiv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtjrgfbydq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtkybrdnvu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtvwnobaii.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtrlmmexdi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtivuivkpc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtnujyoyrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtouuypibu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtzcwdlotk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtzozgehxh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gthxcrdznj.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtiesdiuje.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtmwsxltsx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtxdfkpagz.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtzlxtpvgs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtuktsdhso.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtqoflbiuu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtsetbvqba.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtcugnsvpj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtczzolvnp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtkdvshupf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtuxmjwldy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gtgtuoiozc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtcsmbqvty.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtlkinslax.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gttplkicab.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtgrsknvck.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwcjwmhjy.html

[J01] 获取当前时间
来源：http://hz.hywenlv.cn/gteqccgnuc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtdbfrcenv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtazvlkeam.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtdzcldyit.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtuqgubuqr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhaomingkeji.xyz/gtmlpkesuv.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtkhwjgvku.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtiztivfzl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gteasxunwx.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtcrghbhur.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtjmlhlsgr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtdbuenobh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtrhvbunly.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtbylwdyxu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtnxpmghaj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtytwbyvfs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtdjojeawo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtbcamslxr.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtiqwdclcf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtzihwroxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtldvhjegi.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtxqhfksxv.html


<!-- 参考信息 -->