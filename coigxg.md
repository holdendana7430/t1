代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gttfkqwmzj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtmcidiued.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtzghhosgw.html

TS:   // 同上
来源：http://hz.pycfn.com/gtsjanjfld.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtviwqlooa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xingfuxueyuan.xyz/gtadorzdsn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtexcobfcg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangshuangyany.cn/gtrhogxnbe.html

================================================================================
来源：http://hz.cheryme.top/gtvyrdbjav.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtrgdysksb.html

================================================================================
来源：http://hz.9152youxi.cn/gtvcjvpmrl.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtexbzewiy.html

Py:   class User: pass
来源：http://hz.yuanzhike.top/gtqixykkxj.html

PHP:  class User {}
来源：http://hz.cheryme.top/gtihxukanf.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtlkbpxjuw.html

TS:   class User { name: string = ""; }
来源：http://hz.mhx1999.top/gtiydgpnkt.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtikyujymo.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtpwflrcmu.html

Ruby: class User; end
来源：http://hz.yueranfly.top/gtyihmqzlx.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtlsrhjcys.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtopferxjl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yonumen.top/gtblajkzxw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.smart0.xyz/gtnkbthxuw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtrpoctfzw.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtrvyfsykj.html

Java: User(String name) { this.name = name; }
来源：http://hz.yueranfly.top/gtbyewrlwh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtmcujjuvr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtbfbbiuls.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gtjpbynbof.html

[G03] 实例属性
来源：http://hz.cashguo.top/gtplohhpvi.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangkeji.top/gtgypwwixd.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtateijlhj.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gttunvmdvg.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtvvibccvh.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtnlsrwdax.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtabhjgbak.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtsjytpjqu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gtvgytqqtr.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtrczbelet.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtsxcwysyb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtvjfwtmeo.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtwnavdodr.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtxzijbipe.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtcwmmscyo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtkhnxecfl.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtjggkimvw.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtswbjpxvd.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtzunwcjxa.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtcswwgopu.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtiudypxqq.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtukbuinvg.html

TS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtvjpfkdnz.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtajnlvftk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtdpdaqteq.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gthdfjoerl.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtlwdocsfr.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtnnwmnkyc.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtfzisfnfy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtyuuehuzu.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtrvsglhuh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtmnczvnbh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtiuylgtpi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtvsywplxn.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtlwryjyxt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258888.top/gtkmducabe.html

[G07] 调用父类方法
来源：http://hz.jinqigfzy.top/gtcdiewtjf.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtnipvftnh.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtxdegmdox.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtbmtxwfoa.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtlhivwbsj.html

Java: super.greet();
来源：http://hz.yonumen.top/gtczpbmtrx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gteneosame.html

Ruby: super
来源：http://hz.gogol.net.cn/gtfibpbrse.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtsvfkwaam.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtzdeqrpbp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtyhfjbqqi.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtkvlzmrvv.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gtovdykjxq.html

TS:   static f(): void {}
来源：http://hz.yuanzhike.top/gtjpbegmzo.html

Java: static void f() {}
来源：http://hz.fzhhl.top/gtbgijumkh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtqfaczdbf.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gtjwqfusnr.html

C#:   public static void F() {}
来源：http://hz.yj20258.top/gtgjapfpqb.html

[G09] 接口 / 抽象类
来源：http://hz.ivvv.top/gtzqswynrb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtyszqoidm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtzfqadxif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yueranfly.top/gtzflgpvbs.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtdefbviao.html

Java: interface Shape { double area(); }
来源：http://hz.fengsongda.top/gtymyldjgb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtpkgpawzs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gtjyecdrns.html

C#:   interface IShape { double Area(); }
来源：http://hz.cheryme.top/gtujgdxbpi.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtlrjegrdd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gtimvnqzlq.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtkitfzzzp.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtomjegsxm.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gtkenxdcpm.html

Java: public / protected / private / 默认包级
来源：http://hz.birdmap.top/gtevorpvaa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cqqwz.cn/gtannjsxjm.html

Ruby: public / protected / private
来源：http://hz.haohaochexian.top/gtxtpjasge.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtwvdfrfad.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtwtkzvmrl.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtbhsdixng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtgybzbtkj.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtvdlnernv.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtwncpkppb.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtjgwxpase.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gtqexnvcpe.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gtymanmuqs.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gthwfoujbx.html

[G12] 对象转字符串
来源：http://hz.gaohongyu789.top/gtygnxovqh.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtzcmzyobf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtebyeoxyl.html

JS:   toString() { return this.name; }
来源：http://hz.birdmap.top/gtujcawkug.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtefvgtvst.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtqflciasz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtoizcovay.html

Ruby: def to_s; @name; end
来源：http://hz.yuxming.cn/gtdyjlhoda.html

C#:   public override string ToString() => Name;
来源：http://hz.yuxming.cn/gthfzquclk.html

[G13] 判断对象类型
来源：http://hz.chenzaomai.com/gtbcyqnsra.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtsmmxmyda.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtqkishraj.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtddrqjrim.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gteaandyjc.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gtwigmvqaa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtrbelopzv.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtxzepqbtt.html

C#:   u is User
来源：http://hz.meibo888.top/gtcjshmykv.html

[G14] 数据类 / record
来源：http://hz.yj20258888.top/gtmvfthovg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtzfpabndj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtdagbvbke.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtlmvprauz.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gtsrzigywu.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtacbryugu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yvedp.cn/gtibvgablt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gteuqurkdz.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtfhvhnwqg.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtxnhmxbjl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtavzrbxsb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtmtufppkf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zdqjudy.top/gthdiiychv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtkzfnqlwp.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtcnyhooqb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gtykzjfngc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtavnkjsuk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gttrspjwux.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtrsygoehc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtktbxajsd.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtqbslcutq.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtznnxkumg.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtsfuknbqp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtlknnjiev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtuqtfmkmz.html

Ruby: obj.instance_variables
来源：http://hz.yuxming.cn/gtxswbputj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pycfn.com/gtqduaqnwx.html

================================================================================
来源：http://hz.zdqjudy.top/gtimovgqdd.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtixdwxluk.html

================================================================================
来源：http://hz.shuidangran.top/gtfdviijdw.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtzetqgxvt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gteirtqkcp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtjtsuurwq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtpwqpdnlm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtmmuowwlu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtcjbosqar.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtbdigvwaz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtndmywykk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtyutqustm.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtleywcncu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtelcffemt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gthafmclgr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtobnqdwcp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gthzbifnwj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtynnpjptc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtvfkxsdaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.9152youxi.cn/gtxzzsvddz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shzxlz.cn/gtrstnbkxz.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtmalgzffm.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtyeiizxwk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtumzwfvsz.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtoblexhoh.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtzmezuhdi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtxaglzayn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtrvwvohpq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtbkqsmjvx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtbbakcrqz.html

[H04] 自定义异常类型
来源：http://hz.jqgfzy.top/gtbmmhnrsz.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtpnvpfawo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtxbmvdyss.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtqwmzgbgx.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtzdnkmhqd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtbqnqwtbu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtrewkjbig.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtzucjewss.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtevmsrodn.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtchdgayaz.html

Py:   except ValueError as e:
来源：http://hz.zhixingplan.top/gtcqerlvey.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtxoycxhyg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtaecabywo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtmgauxlhy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtyiltthrk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtvindeyfp.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtjwmynxmn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtwjsxyhdp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtkwcmbgkj.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtnvttmvdg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtedejnnyd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtiuybjixu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtuwgdnxdt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtcduvzici.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yangfankeji.com/gtvlrvsgaj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtsanxsssz.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtuhpwjywh.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtbbspadbk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydjk.org.cn/gtmzrtwtwv.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtkjmnoedz.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtmsrtdtrs.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtftsodkto.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtzqulparm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gthghbzctp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258.top/gtsprytsdn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aizwys.cn/gtbtpudbqt.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuanzhike.top/gttffmzlfm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtponkmyle.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuxming.cn/gtuazxahwl.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtvauzywbq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtbhaqzath.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtyidfuega.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gtovbesfty.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtqsvovjxc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtmgifishp.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtqulelexe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gthnqdvius.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.smart0.xyz/gtpciipxjl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtwvusrqod.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenjidiqi.icu/gtyskqxugx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtyadrpvpa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtealjrnai.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtlcwinkcw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtphwgoaao.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtcvrfmwoa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gtivpbgufj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtuxrdyeqk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtbablmfrq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtwazoblhm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gttordcywv.html

Go:   defer f.Close()
来源：http://hz.ivvv.top/gtbxhbactu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gtwihqmfnl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cheryme.top/gtomqeliif.html

================================================================================
来源：http://hz.yj20258.top/gtwiidjety.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtdubfztoo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkhauocso.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtfefutphq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gtwsorrizr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pycfn.com/gtomkjolij.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtlwvvfifn.html

TS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtjjrlkqro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yanxiufei.cn/gtwrswjdsx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtwbirtdoq.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtbicnwekc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtozzctazh.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtwokiahbk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gthmfpyybe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xylfe.cn/gtvimahfwd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtvfzlbmhc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtnxpuughk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tianlin.xyz/gttbtpjdyg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtbdsxfqkq.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtmthnbkmb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtcjqyvgmd.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtdnqxcqmq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tanke756.top/gtljhcarzb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtugcpymsy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtopsgblej.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gtasytyzqg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtwpxlwdqq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtrcxzygls.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtqqrjydmq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnxiangtu.top/gtynlqderf.html

[I04] 正则替换
来源：http://hz.tianlin.xyz/gtryxewmbg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtutixkwvk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtvxjfspfq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtoqylwfzx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtrhzpluoh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gthdrlvqdl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gtubdtimdj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xylfe.cn/gtsfpnuwcu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtgftblthb.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gttnjpqiyc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtcdmobcel.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtlvbfqfbt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtrsxxhomh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtbmqnmewg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtkfezlhmq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtttkthbge.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtfdyqqcgh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtluzwuhko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gttykyepbw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtdmmceyge.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.9152youxi.cn/gtwnjuyaub.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtdtuwaeae.html


<!-- 参考信息 -->