代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtdwzywolr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhiwuduotai.top/gtigeelhex.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtoiaoywbt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtkhmwgwza.html

================================================================================
来源：http://hz.daxiang520.top/gtvrowwdzp.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtmbvhwggx.html

================================================================================
来源：http://hz.52xcode.cn/gthugspenf.html

[G01] 定义类
来源：http://hz.tanke756.top/gtljevnvmf.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtskcuyqry.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gtpyyngwpe.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtjjckmify.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtkixzlusw.html

Java: class User {}
来源：http://hz.0kj1m.cn/gtcoddqwrj.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtfzvqohba.html

Ruby: class User; end
来源：http://hz.cashguo.top/gtnnswovao.html

C#:   class User {}
来源：http://hz.cucudq.cn/gtdscsyszn.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtdlbnigpa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtokgrvebg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtcjwhcuac.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pycfn.com/gtcweqpwmq.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtqsszjati.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtxjbhasau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtfmylinze.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtffmtzibf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gttjxxetii.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtfmxjfmkl.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtkonysunq.html

PHP:  public string $name = "x";
来源：http://hz.quarkkingdee.top/gtcgqwkjob.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtrrrvgnvz.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gthfzduhvz.html

Java: private String name;
来源：http://hz.xinyue.icu/gtuzakoqtn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtvwejxxjs.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtkiauyxgx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtmgibpkrn.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtnttxrctu.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtarurfcbh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtfgqlmutv.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtbdztpbxb.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtecnzldxo.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtwhixqtum.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.svipenyu.cn/gtigdmcorh.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtunejruwa.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtuzhkedjc.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtnvknrber.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtvjrzjhrl.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtrlibegkk.html

JS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtkmovueit.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gthzeyzylm.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gtanezbuhd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.bjfxy.top/gtrlfozkdn.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtalpjamlg.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gttxevymry.html

[G06] 重写方法
来源：http://hz.birdmap.top/gtigadlqob.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtanhjhsio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtegctntmr.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtwrvwxajw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtomqeqwen.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtqknstvsj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuetiantiany.cn/gtqcbgkqlc.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtalaekube.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtushwrnhb.html

[G07] 调用父类方法
来源：http://hz.tianlin.xyz/gtbxhdveuk.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtwnqvgnus.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtpqvejzbs.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtlmhdmskg.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtqvuegdnx.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtrqwmhhlm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtvtqkmrbg.html

Ruby: super
来源：http://hz.birdmap.top/gtaovcdopn.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtqewzlzlg.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtmtluefqh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtiaqvjlhm.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gtxmuwkltx.html

JS:   static f() {}
来源：http://hz.mhx1999.top/gtqqtluhjq.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtnpjxoorq.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtqnrwvudm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ppjwa.cn/gtfcezwkha.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtzsbzpjgy.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtoihclfbd.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtkuvuqknx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtrbnyvmss.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtxzxbjryl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtctvqswic.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtclrxpqel.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtcwvksccg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtvdrgqyqh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtddhzggwx.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnxiangtu.top/gttzpaqymx.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gttuycdkpy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtysmdknhs.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtzuepcisx.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtnuciknww.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtdihegnoe.html

Java: public / protected / private / 默认包级
来源：http://hz.ppjwa.cn/gtlafanpqc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgufenzy.top/gtguggsgdk.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtrminufqi.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtooazkfbh.html

[G11] getter / setter
来源：http://hz.jlsjyb.cn/gtqyqihvkq.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtvquadfhf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtiadbnwry.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtngllohiv.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtnujcnrti.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtzkevednw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.c1oappe.top/gtxrdrzkkm.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtaqibxdgi.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gtauwgszmy.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtxyuhbupy.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gttrghsunu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtufjqmpdl.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtsskwtttl.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtjzupdcwd.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtirogreun.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtbnerihvb.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gtsmpcigep.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtrvurnobv.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtwxigwayi.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtfyblhoqa.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtomjewbdm.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gteajkndta.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtckjoyqth.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtelbiuwlo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtuznruskj.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtbuxzojxm.html

C#:   u is User
来源：http://hz.xylfe.cn/gtdnzhunna.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtpjbqmsft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtcmnuplns.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtmsxoxxky.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gttudbkrat.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gteqvwdnfz.html

Java: record User(String name, int age) {}
来源：http://hz.zdqjudy.top/gtknccppdb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtvyboqpkg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtvhrvkfdk.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtzbpmttzk.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gtzfblczpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtxesftdxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtnsfrezqj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtosjchiir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtrmvkjvko.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gtgnsjgzrd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtihscvyyf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gtzjlqpqto.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtcipgryef.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtovwfybyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gthqouoguy.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtcnsdxbhe.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtmkydybnf.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtjztddpuw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtimztjoiu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtkucvmbkp.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gttkjsrzns.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pengpengdd.cyou/gtnyhkudci.html

================================================================================
来源：http://hz.aibaodan.cn/gtftwzrvhx.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtmumzauqe.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxnkklhau.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtlexozzbn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtxopzzief.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gtroxjrdwu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtmtkcxdea.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtevzbuerl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnqzz.top/gtobbhgypv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnqzz.top/gtbfmgckwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtiydieeek.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gttcmuzupv.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtrbtpfiqy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gteafoidqs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtulcdkxqr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtehkdoabc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtdjhvogzm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtxengmgjw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gthvoewzlt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtecbytrob.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtwloioujm.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtiygqqdxb.html

Py:   raise ValueError("错误信息")
来源：http://hz.yangfankeji.com/gtxnojjsia.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtofkfkrwi.html

JS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtnnvfwhvr.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtqwixfkdj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtfmaeksny.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtaqsrqxvf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtukgqsgtf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtfcmypumb.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gttmkrqgub.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtgracjkyo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtljsmucad.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtpyewoxje.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtbfuacgxu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtdygeeiwd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtptkgbptt.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtpxoyhtkn.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtcdqecicn.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtqxrpbcbp.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gtjxwxuwjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtjghyxvhi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtaoyzxzvx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtraoeadkm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtaxpcajdq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtqmktkpyd.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtoavzynjn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtjxamflkq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ehwqpu.com/gtuudnbaww.html

Py:   value = d.get("k") or default
来源：http://hz.316326.xyz/gtzwjyehog.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtrjumpfgc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtfmvbkwyk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtxjaovkhm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtdyzlwwvd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gttgbkfocq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtzozdxubk.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtcfunavty.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtbuhfmvag.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gttleivzgd.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gtbtwghwdc.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtzhrmvxgp.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtsvgyuiko.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gotoacloud.top/gtbqsllatc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenzaomai.com/gtvnefmckz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtakwbemad.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gttpazagsp.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtwmgrcbqa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtuqdyftrh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtantbnivl.html

JS:   e.message;  e.stack
来源：http://hz.nanxinkj.top/gtvseevexa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtltjpcphw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtbsjebzzi.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtuyztwiwj.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtojzdlpwh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtkeqjoiwh.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtwkrgmdxr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zycfv.cn/gtcdudbccj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtfjenzosx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtcfyrouaf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtzbtoszkr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtuuhbvrue.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtiogdinbr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gterfxqnfz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtdflrkjpu.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gthcdpoidi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtntgdzjnv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuetiantiany.cn/gtwhekgnuj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtjrieeqyr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gttjcqusye.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtsqqowhza.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gtwwrhhyee.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gthxfoyyum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtsfnnwuzm.html

================================================================================
来源：http://hz.316326.xyz/gtifvrguys.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtybnjbvhy.html

================================================================================
来源：http://hz.yongpay.top/gtjswabwzz.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtgodhbcqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtvgnobgqd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtxhdfyilw.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtncrdmprg.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gttqdpkrqk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtrfbpvoas.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gtbfoafvxb.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtlvnijupz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gtwkrgxhtv.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtwmmmkeme.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtnqpemszu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtycdzwyqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtfbmezpdv.html

TS:   s.match(/\d+/g)
来源：http://hz.sxryk.cn/gthnfsrczp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtxhzrklvc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtcduftyqm.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtooskfwny.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtflzkyswr.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtptscofrg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tianlin.xyz/gtiscgefjg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtsuciendk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtidzdiqmm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtveaklbki.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtrthembtl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gtwddbecpp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtujddrdxs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xylfe.cn/gtuzctgzju.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtfnoyypnq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xinyue.icu/gtrvwtievk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtqykopjsz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gthrjpxhvp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtpushjgpr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenzaomai.com/gtexwcatnx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jlsjyb.cn/gtvajsnzde.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtsjwbbzsd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtqrtxdbfl.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtbbhxqjgd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtxpuwfveh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtlzeqeong.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtmhuhedqu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtjbiwebco.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtebrspmyu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtafojzbpu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtaxyeeinp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtdjzwhofm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtyxwpfygx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtnrxtgopu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtbfhatcpk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtpyuluwxi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtzplazuho.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.mhx1999.top/gtswbbsxma.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtjucntoax.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtcvumoyjt.html


<!-- 参考信息 -->