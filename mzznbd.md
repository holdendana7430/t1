代发 wailian999

JS:   this.name = "x";
来源：http://hz.zhongyouzk.top/gtdydidolj.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtblrcuysh.html

Java: private String name;
来源：http://hz.birdmap.top/gtzagfcrge.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtjexnulgp.html

Ruby: @name = "x"
来源：http://hz.0kj1m.cn/gtbomxxmhu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtsdijeqaz.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gthscuiulw.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtenyjldtl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtlmaxyhjk.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtlqbxccmp.html

TS:   greet(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtcktdamkc.html

Java: String greet() { return name; }
来源：http://hz.daxiang520.top/gtyeqjdidx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.daria6918.cn/gtoblxxvia.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtnztfzvaz.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtqujjaaue.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtoguvlpnz.html

Py:   class Admin(User): pass
来源：http://hz.pycfn.com/gtiffcqpkb.html

PHP:  class Admin extends User {}
来源：http://hz.aizwys.cn/gtgsewnmup.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtzgeaaqag.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtkpbmltst.html

Java: class Admin extends User {}
来源：http://hz.daria6918.cn/gtkgvwazse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtrthjftse.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtcxskonfu.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtzekljdyo.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtxkivapxo.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtuaisfukx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtakcoflow.html

JS:   greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtwjxqlcwu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtafjbplou.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtlhujyeps.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtnqvchkox.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtncucfkyy.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtafysofyp.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtotnkleab.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtulzewybf.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtxdvvmyqz.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtmzkphmlf.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtaucznizt.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtqcxvxehp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtwuhmtfoc.html

Ruby: super
来源：http://hz.sufxvd.cn/gtwhanvqyy.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gthlwfvres.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtlxqtxfek.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtclggjgey.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gttempztab.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtbyldzdci.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtfvvezgcy.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtqkxposoh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtquivrprc.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gtmevloanr.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtsgsxizod.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtamvpvddn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtfstloxom.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gticfizafa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtvcxgcdqz.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtqekobrpv.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtkgvdgmuk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtpyyjujua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gthrbhxiuc.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gttfoosnxc.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtluzairrf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtrdczgcol.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtxckhemhj.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtmrrogavd.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtvzqjqpzd.html

Java: public / protected / private / 默认包级
来源：http://hz.yongpay.top/gtdowfbqxb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuanzx.com/gttikapfoq.html

Ruby: public / protected / private
来源：http://hz.sweek.top/gtaptzjzky.html

C#:   public / protected / private / internal
来源：http://hz.9152youxi.cn/gtpdknioxs.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtkrteetdl.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtkfzewwkc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtvnsghekm.html

JS:   get name() { return this._name; }
来源：http://hz.chenlongwang.top/gtggmzhlck.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtllybxckr.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtbcgpuxey.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtdzxwfctc.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtbclmhrdl.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtqvhivchp.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gthfyugfhe.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtusgilndd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtulswmpjz.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtqsdydvea.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtuosukqdt.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtqzkumxou.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtaodbpsiz.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gttrgtqhfp.html

C#:   public override string ToString() => Name;
来源：http://hz.hywenlv.cn/gtswddpxaa.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtcvkqafkd.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtdmofrtky.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gtjntzkikn.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtjdjanpos.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtstbmgtsd.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtjfnsjniz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gtxpxffmxc.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtqouvbwyk.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtkxagtfbr.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtpcjsbwqw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtpyiolzfn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtwlpsaput.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtyzvldpgs.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtjwchnooa.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtdnoxxutq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtyqgumwkd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtznptknla.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtufdatenh.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtqevgpvpr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtzkanqlmp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.haohaochexian.top/gtboictfyv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtvqauyebq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtvogqfzje.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtylfojwau.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gtznxzhhlp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gtrzqkffem.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtvzrwnlcl.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtfrlmdwyf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtafcqnvpp.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gtvjiagihq.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtbaslobdw.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtdbuugkog.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtipcflvfu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtqrqdvpku.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtvztiigjq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtwqsiweuq.html

================================================================================
来源：http://hz.xinyue.icu/gtwcatovdr.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gttnclvjsb.html

================================================================================
来源：http://hz.ehwqpu.com/gtzyajexmf.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtxsrxjbvo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dianchejie.cn/gtogudxsts.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtsqjtqpjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtedmqafdz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtnfckjbid.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jlsjyb.cn/gteptsjhto.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hammf.cn/gtcimjuawl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtbzdfvldp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtucdqopww.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtwmeslvce.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtfthoaava.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtvhajajmt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtqmanapke.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtvekndred.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtdhjnrawa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gthlyrrkwr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtmbykvoxq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtxomgmumj.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gttyazfsaq.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtguukfvhq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtckypaqks.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtnxhtwqjm.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtipklvydm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtwmkyhuoc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258.top/gtwyvrhpzk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtjtpkmugx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gthaozlyzz.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtscdvtomm.html

Py:   class MyError(Exception): pass
来源：http://hz.hammf.cn/gtrpqkuwda.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtmabnbfzw.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gttqxhomnd.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtgnxyayty.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtuuzwimko.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtkhxxfvcz.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtfwwzixmp.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gtjjczxynm.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtsdfsqanw.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtulgmmbcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gthvduziso.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtkygsslxc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtawickbff.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtqywfngxu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtehhzsbag.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtfmtnbwup.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtltqotseu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtyryyyfru.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtxrkfymho.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtbivomjyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtvdgwozxw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtdhhkquyt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gttkihfcnf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ybcxt.top/gtyxjwnmok.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yongpay.top/gtqkrkzevl.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtuwybhzol.html

[H07] 断言
来源：http://hz.yj202588.top/gtgjjptvba.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtoadtcgfj.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtxbhoqick.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtutyqntxd.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtfsmslywz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtkvtdrsvu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtwczrqopx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gzhubu.top/gtsgihalae.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gtsuipmctf.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gtrfdnsrdn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtlbuvzdvl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yanxiufei.cn/gtxjgynohm.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtnexnthca.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtrehbfskm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtvtnfrplh.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gttuskalnk.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtkxlfpgre.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtyermculu.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gtqeaylbaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtvxbdsvrz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtftpluizo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gtitjktqnr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtwujrqqse.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cheryme.top/gticacnjkj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gtskibwccr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtclktuijh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtveoygklp.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtsjjdrjch.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.wangshuangyany.cn/gtjxnuzise.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtgdbdskvd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtheadfhqw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtlhusivvi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtpsjoqcai.html

Go:   defer f.Close()
来源：http://hz.haohaochexian.top/gtdnyvwcfp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtaqvacksd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtemqcfriu.html

================================================================================
来源：http://hz.gzhubu.top/gtynzgyqgj.html

I. 正则表达式
来源：http://hz.yongpay.top/gttqxwuqol.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzxnuujds.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtzxsqhren.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtlydjmqul.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gthrkqgxgi.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtzbrcxzsc.html

TS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtrccrtria.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtnullmymk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtaqoydeep.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtfxwwlwel.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtykiifihn.html

[I02] 提取所有匹配
来源：http://hz.zhixingplan.top/gtinkrjrwc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gtfjkdpfbv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtnemvwpho.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtrgeygwvw.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtfpwppreo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtefvazdur.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtlfmiyphc.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtvgwyxmxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtqsnvmyld.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtwswjbshy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shzxlz.cn/gtlhsixmfn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtvaifgioe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtyvmvqowc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtkrffjwpg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtmwsrxphz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.c1oappe.top/gtujuakosr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtrzoibgcn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtkxbxnwrd.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtpspwlkgv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtkfvtowec.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtwiqeupjl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtitatjjaq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtfygdbtag.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtubylbwlw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.feifeiyinyue.top/gtzyocyamn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtnopsyltf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtqitrmoye.html

[I05] 按正则拆分
来源：http://hz.hnqzz.top/gtqdldocza.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtgcqxinoe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtjwfcurvq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtjcrkmkmn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtsapvxbbh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtqqdlgwav.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtgymminsm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gttvnjohyb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtuetuxcik.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtoznladvx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtixapixul.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtwsobwnxw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtartmebmj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtkfewijau.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtlnsgppfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtopqjbmdd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tianlin.xyz/gtevpmakhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtbsezmzqu.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtrvukvder.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtnjodncma.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gttqxwlyzp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtsscbnnfc.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtbyyipzux.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtcykfvuod.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gthsscyrdy.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtwsszflxt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtdpgumcje.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtijhcppdj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtfiveiign.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtathproqd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gttvvwfpww.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtybgpvrdp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtigmyfoak.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtxapqpxse.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtruyrytep.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtzniynedn.html

================================================================================
来源：http://hz.gzhubu.top/gtwdmzzuto.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtzfeiqgch.html

================================================================================
来源：http://hz.sysykeji.top/gtlbnfherm.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gthumviexu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtqpqkfcvk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtavewipma.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtzqedvpxb.html

TS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtzmphavtf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gtoyhkgvlz.html


<!-- 参考信息 -->