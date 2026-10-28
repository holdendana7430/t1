代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtgnrwjvne.html

Java: User(String name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtiwhyjsar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtiocclipz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtgaxkluqt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtrsrqkbkq.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtrocxlebr.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtlwncxebv.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtidoiykvk.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtwtyeyeds.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtaxuuupnz.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtemngumiq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtzpbtodfj.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtlllxqizn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtjvftzque.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gtoiirvxvz.html

Py:   def greet(self): return self.name
来源：http://hz.zycfv.cn/gtqgquboke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtwskdnmlv.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtsrdmksvq.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtqaijvsqi.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtvorzfqxm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gtncnvdscv.html

Ruby: def greet; @name; end
来源：http://hz.daria6918.cn/gtqylpktia.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtmlicaqwi.html

[G05] 继承
来源：http://hz.cdnleiting.top/gtuezlrhay.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtuitsfrqu.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtfdfuoyzj.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtrscrbyna.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtpkwnmgho.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtfcjvxrpp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yonumen.top/gtxywwkpds.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtqrzivdyp.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtfgtzyfwc.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtjhxkhtsf.html

Py:   def greet(self): return "admin"
来源：http://hz.gaohongyu789.top/gtzmoczgss.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtfucfzjwj.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtevzaqfsq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtafcdzpkc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtrejbufzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtfvtisebz.html

Ruby: def greet; "admin"; end
来源：http://hz.hnqzz.top/gtslstuvcf.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtmqwpktfd.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtcdeqepkf.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtsnwdaohy.html

PHP:  parent::greet();
来源：http://hz.jinqigfzy.top/gtwshwfhwi.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtxxpfivwx.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtkbtrfsrs.html

Java: super.greet();
来源：http://hz.havefunace.top/gtgtbplcdi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gtdlbrusdx.html

Ruby: super
来源：http://hz.aizwys.cn/gtledgrzyy.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gtvolhrldm.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtzdthbmso.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtllnbdoke.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtybaxioft.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtqfjkpezd.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtwtwrfsdh.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtmohdphij.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtgyznrlnu.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtqacahhip.html

C#:   public static void F() {}
来源：http://hz.guowangkeji.top/gtvmtiasgk.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtlcumppsi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtvzgwelze.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtsecnqqkm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gttmtgvbim.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtviwtorvu.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtclsukgmw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gtcbsvwwiv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtkuwadjmz.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtgdeinden.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtqpipywlb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtwsjtrjzz.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtpradjjfa.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtxvynmvgh.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gthvlbaqqm.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gturfcxywo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtvcwdaesu.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtdhujdwgv.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtokcyhfef.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtiuqpetoz.html

Py:   @property 与 @x.setter
来源：http://hz.xinyue.icu/gthfnsfpkx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtpmchrezc.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtgdgqddxw.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxuanxn.top/gtprmennok.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtoedhcsss.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtxcmrztwg.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtqsgzpszz.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtemiblqvr.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtrqjfkfgf.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtwaqxskvj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtbzhcsqld.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtvqelyota.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gthgpclebq.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gtycmdybok.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtimvueawi.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtwvrjkcud.html

C#:   public override string ToString() => Name;
来源：http://hz.svipenyu.cn/gtsjgiptjc.html

[G13] 判断对象类型
来源：http://hz.quarkkingdee.top/gtvanovbie.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtpcspkzdg.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtbuhukckd.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtktoidcjd.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtbntouvmj.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtrhjhcotn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtfvyjuptc.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtopfvfbmo.html

C#:   u is User
来源：http://hz.sweek.top/gtcenvttxs.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtxjeusfjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtymmzbcyv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tian-w.cn/gtovctezwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtjqcwwzgc.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtckpegrap.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtvpdcsggv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtfemxwyhf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhengqikj.top/gtculskmza.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtfvcqisjn.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtedlgqzjf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtgwqxozni.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtsffawjyc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gthpagtwkd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtcvotnmoj.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtftifncia.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.meibo888.top/gtwqqwchjl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtwyrjhrup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtxuijcbub.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtnelpmmgu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtckwzekzs.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtuytthhdu.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtjtcdixbz.html

TS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtrpsvmpqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtrfmuygmg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pycfn.com/gtbxojrpvr.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtvzawxqrh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fengsongda.top/gtyrrdcwco.html

================================================================================
来源：http://hz.yanxiufei.cn/gtwvldewyw.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtdrmppzck.html

================================================================================
来源：http://hz.yuanzhike.top/gtmdxgqlgh.html

[H01] try / catch 基础
来源：http://hz.xuanzx.com/gtrgjevcwv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gthtxpvdas.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtbrrdjudo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtyizmmduy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtpjwizdmg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtttbgromb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gtftcvilim.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtbwnfywkb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuanzhike.top/gtlgnydgnr.html

[H02] finally / ensure 收尾
来源：http://hz.vqdsnc.cn/gtpzksqxip.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtykcznrey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtpkuhxivq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtrcngdmir.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtcmyhspwx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtvtlklfiu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtcjvodsih.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zycfv.cn/gtitbqvowh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtjwqkmssz.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtekmjyfsb.html

Py:   raise ValueError("错误信息")
来源：http://hz.gotoacloud.top/gtjizsatuv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtxdgnfinr.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtfgevcepy.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtwkyxfhpa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtfqnjyhlt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtkfgecyxw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtxwlijmrn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtfdcoszqd.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtyxmimvxi.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtuirjxrex.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtdigzxgav.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtojzobowi.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtccrjzuor.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtplwijzgj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtnkyzviwe.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtnlgdlotb.html

C#:   class MyException : Exception {}
来源：http://hz.sxryk.cn/gtrljvdqmk.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtsmpynjsp.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gttmmeyktj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtpqlnybtf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtnvasfxro.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtqdjijxmf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtoedpbpee.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.havefunace.top/gtuaccyzvn.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtjmzebayc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtgkekqsut.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtxqmsgpij.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtyxhdfnop.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtnjqxhmhq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gthkyyzhtu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtpqaqsyyj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtjjybtcdu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtupoxzpzk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtifcpmban.html

C#:   obj?.A?.B ?? default
来源：http://hz.vqdsnc.cn/gtvzodefpg.html

[H07] 断言
来源：http://hz.tianlin.xyz/gtdkxhjcqm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtdldqikwz.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtudexzvgr.html

JS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtspwipezk.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtjtiduwbt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtbqociyqe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtaauaziyx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtxfeelvmx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtmyabrpfk.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtnqcpwubo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtdfckhcjt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtheadmnhr.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gterlqizqm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtzodbjzwi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gthegisxrq.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtvfaadjxz.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtpnatpflw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gtdmhnzdhg.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtfgfmuqil.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtmkuranlz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtqcnkeigq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigfzy.top/gtuvltvdjf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtifxocuyc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtojitfijy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtthgrjohc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtxedhbeav.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sufxvd.cn/gtzjvnkpgj.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gttiypzyxj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtujqanhtu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtibptqjwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtebuofrhc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtxpsbrkbz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtonqkojhh.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtqxggpeqz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtfvjdjvre.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtudzskeoh.html

================================================================================
来源：http://hz.yangfankeji.com/gtthfezyep.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtpmjukvvv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmbwwdlgo.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtqslculsf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtngykegjy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtngvbmeer.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtpupvhfum.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtuyoyncbj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.52xcode.cn/gtfrgrbwtv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gtrargkjpi.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtmhwqrjxb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtovbktpec.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtmcgnwmsm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gthhqmzupa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinyuanbaomall.cn/gthlnowxli.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtlhcnijxw.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtsyfrzfki.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtnibnpvnf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtbhcgdlml.html

Ruby: s.scan(/\d+/)
来源：http://hz.shzxlz.cn/gtqbrsxjnd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.feifeiyinyue.top/gthhycivja.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtfspimdoq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtnjrtdoiw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.andypj.xyz/gtbnvpclkp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtjtiizxjz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtqftxaprg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtlhqwgqkh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtxhwdcfbm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtlbxmypsu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtxoleiteh.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gttgemzdvu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtgbqryqtw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtdqxdoaxd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtouxceyed.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtijfmjfmf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtcbfacgng.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.52xcode.cn/gtncmbdfxg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtavpvuack.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtnvnugifo.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtacgpaorv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtickebpws.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cucudq.cn/gtmcuakzgb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtsfyxnbws.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtswksgrrx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtvpzjcryi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtbmykihyh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtsqfsvfwq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtkxesvfph.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtydsfltav.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtsqbcopoh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtvtdjqdef.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtlctxxxpp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gthtcdapce.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtutohgzta.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gtyhmspaux.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtwnfibnwm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtekwgywbl.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtfficzvks.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtfvajlefi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gtoxnwmgpt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtgopbkpab.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtzfikrmmg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtcuomixuw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtzgpgvwqm.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtpjinjagf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtbnblstaj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtvjlkryry.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gttevhnglc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtstpgwoew.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtpiizkdco.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtohqztnrl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtsxqyzeti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtoqnzsluu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtykhitiss.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtfzwbrxyz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtezfaccbn.html


<!-- 参考信息 -->