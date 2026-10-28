代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuxming.cn/gtbwzdygne.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gthhhmkxem.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tianlin.xyz/gtlmbakxgs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtuunvvehm.html

================================================================================
来源：http://hz.yvedp.cn/gtiarbodiq.html

G. 面向对象
来源：http://hz.fzhhl.top/gtxxithhlb.html

================================================================================
来源：http://hz.haohaochexian.top/gtqwefgqjd.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtdulwumrr.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtxekztcoz.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtxuvrpers.html

JS:   class User {}
来源：http://hz.jyoumei.cn/gtlsbawkpp.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtrorissqg.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtjwahzull.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gthusdvrgd.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gtlsycamlx.html

C#:   class User {}
来源：http://hz.sweek.top/gtdhubjsfe.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtdkekyurs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dianchejie.cn/gturkydcro.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtjjzdmbcb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guannengcc.top/gtkgtljssq.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtbaurxkcl.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gteicurupi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtnjmfybzw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gtcofjnefu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtsvwdzvxi.html

[G03] 实例属性
来源：http://hz.xinyue.icu/gtvnztjdot.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtjcqwupgr.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtwzckzmhh.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtlhtfojoh.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtsddztsew.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtuftchtij.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtojgwdejq.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtyuvsloqt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gtssdehmlp.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtfhihiaqq.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gthxekttlj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gttdiiwisu.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtjmfgkcel.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtewobskvz.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtgdyjcesu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtutpqjaga.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtispmlduc.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtamstuexa.html

[G05] 继承
来源：http://hz.yueranfly.top/gttjvcygbp.html

Py:   class Admin(User): pass
来源：http://hz.cashguo.top/gtmzrfcycm.html

PHP:  class Admin extends User {}
来源：http://hz.gogol.net.cn/gtmeirqyya.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtacyctnsh.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtdafuagbd.html

Java: class Admin extends User {}
来源：http://hz.fzhhl.top/gtsmelknvh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtfglayxel.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtkctkfmov.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gttbimychu.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtuwstdxuv.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtuhlgelym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtgnmovdzk.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtdhydlyyy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtyxmhdebn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtiihabrid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtqjsfenti.html

Ruby: def greet; "admin"; end
来源：http://hz.ppjwa.cn/gtiwwfyack.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtlojiderv.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gttpccyasg.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtbferyduo.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gtuqvuffjy.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtyyxdgukt.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gttmmbtqdg.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gtlwistyax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtlwuzmebn.html

Ruby: super
来源：http://hz.haohaochexian.top/gtppqjckwr.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtswcyqhxb.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtbymdmzjn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gtgmsnshrd.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtryvrdmnu.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtgqilklqj.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gttlxmakio.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gthcqyqeny.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gthuwyogkq.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtsfndygmg.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtfmwaeuvp.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigfzy.top/gtdirabhpr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.haohaochexian.top/gtzzahxnhx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtdrzqjtxi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtmbxoeawy.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtbvrzcwou.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtsrttgouq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtqifahxtn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtdauodwsu.html

C#:   interface IShape { double Area(); }
来源：http://hz.quarkkingdee.top/gtzqzthlqg.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtudgqibev.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtpbexwfnr.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtaaooxlac.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtciargint.html

TS:   public / protected / private
来源：http://hz.tanke756.top/gtpcwvuipk.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtdwoccnxv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hfpthk.cn/gtrhujnjag.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtubhxnvce.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtiswijjge.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gttxlbkqii.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtgvlfjnpq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtymshfnky.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtmosvanwf.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtqaetqhhr.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gtrviuzrzn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zycfv.cn/gtvgswjuws.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtjqppevub.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtjlfuwzau.html

[G12] 对象转字符串
来源：http://hz.cashguo.top/gtgrjismhx.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtvkuyniex.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtoiknxeqx.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtzhcvxnqb.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtduqtenxw.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtcfqvktat.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtctvokvkw.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtlycuozqb.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtkzmcutkr.html

[G13] 判断对象类型
来源：http://hz.yongpay.top/gtmyrntnra.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtbqmbviif.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtkdqtbswu.html

JS:   u instanceof User
来源：http://hz.yj20258.top/gtlpkxnvdw.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtwdhljoyp.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtpyqxiory.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtuurejcwt.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtbsiteatb.html

C#:   u is User
来源：http://hz.cashguo.top/gthzoattao.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtcyihmjes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtzyiisauq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ehwqpu.com/gthumkrirl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtefvendzy.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtrqgfpvma.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtcxnqzptb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gttaikbecc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtfbaodhmf.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtcsbvolyx.html

[G15] 枚举
来源：http://hz.sxryk.cn/gtoumutxaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtxkhttneq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtpoxkcadt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenzaomai.com/gtbkdrcppz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtscrldhua.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtvoivjwmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtdppaqrqw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtgjvwsyhx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtjkphbzul.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtojpmybzq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtlyzknwdv.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtdkqwwspn.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtpeeuvujq.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtuzhzhaut.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhixingplan.top/gttzjsczzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zycfv.cn/gtuzdjouna.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtlruwffcj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtrxbcwcye.html

================================================================================
来源：http://hz.xinyue.icu/gtwqngzaun.html

H. 异常与错误处理
来源：http://hz.cheryme.top/gtcmkupzzd.html

================================================================================
来源：http://hz.yuxming.cn/gtuwpltfwg.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtifzosprm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtkjcwvdns.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gttzjkudje.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydzc1.top/gtbhdvrlxw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtthbissic.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.andypj.xyz/gtxajwbida.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shuidangran.top/gtzgnmeexn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtgwqamqtf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtjbmuktey.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtnqlxbngk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtnjvgkfdp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtcygsithj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtspevrpmp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gthgjkekhm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtzwhzypti.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtgtictijw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gtoernwqyt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zycfv.cn/gtcaoeawvj.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtfvcgbgrq.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtsrsezfdu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.316326.xyz/gtaltlecjn.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtndyiyxxe.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtrjgupbfl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtrbdshlxp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtbazqdfdn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtkgjiwlze.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtgneeavxx.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtkrhefayk.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtmviuptgp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtxyeavjkb.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtzxbqgjqo.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtlnmzbjfe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtnoxumpsj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtkrqvmfmv.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtgrnszefp.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtxbhymitk.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtnkppcvfh.html

Py:   except ValueError as e:
来源：http://hz.bjfxy.top/gtzkgfnvjf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gtytrbalpe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtbvkkfwre.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtwzxptytn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.snrcjt.cn/gtfllxawdh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtzirjyxkp.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtyngktzco.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtbubgvdcf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtstkqbxvz.html

Py:   value = d.get("k") or default
来源：http://hz.jianghu66.top/gtnoyfgebf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gtzrxnzifd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtnonyppqa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtsuucywot.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gthzwivred.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtjemgjaxg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtaonosjjn.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtjpsiqyfl.html

[H07] 断言
来源：http://hz.cdnleiting.top/gtzucofhpc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtuavznfuu.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtnxaasuoo.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtuqgapqjl.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtlswsrkzo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtfbexdjen.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.bjfxy.top/gtmekueccv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtdadrxssp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtpbucztmk.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtehgslhyt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtqjthokgx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtastbztsr.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtbvouqtfe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtadufdryc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtdvmfhiem.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtghgdwnrb.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtgnhsrvvj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gtdwecloco.html

[H09] 带错误码的异常
来源：http://hz.ybcxt.top/gtcfjhqmwr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sweek.top/gtwfzcmlkn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtrxfjzwse.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtpukvqxay.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gtkceyzfkz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtgqutcxxd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgufenzy.top/gtwrcojmla.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtpjslgoib.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtfgbxofby.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtjwqjfksm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtlzxquvxz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtwomfyvvx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtuaugkvwd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtaqiwgdcu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gttafrwuaf.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtpxayxnmv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtjiedgsht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.birdmap.top/gtegutaspu.html

================================================================================
来源：http://hz.hysaishi.cn/gttkuwykwf.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtgbfzddhg.html

================================================================================
来源：http://hz.gzhubu.top/gtejhrtccj.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtbloutupt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtvzmvfesz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cheryme.top/gtpkvbewse.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtlgqlaoec.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtbgqahoev.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtcbwvlvel.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtjnnftidc.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtxofalpsr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtmkbbiwlk.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtzpbqpiui.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cheryme.top/gtliqkeixo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtrklhjoos.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtnbcaxeug.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtzwweerpv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gtzttneuuw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtbycubdmv.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtazgtsblk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtjhjnodfr.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtzaxrmoaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtsvunjjzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtuxlcqlqr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydjk.org.cn/gtrlulnycd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtxlajhbgq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gtffownjgv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gtomanxjaf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gtjfrtcqny.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtapoyxmtn.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtzoxelolo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtrsfzzxkf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtfrgcfink.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtbmoyfkto.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtfjzyhgqf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shzxlz.cn/gtqbvvdweq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtmeasltds.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtwdgitlkj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gtlhcwteci.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gthivcbnpw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtlbrwdall.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtakraajrp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtbcadipfv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtkuyzobur.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnqzz.top/gtoodoqaxe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtgynbmksr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtpiqbkczt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtcjabieej.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtjfhmmtwf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtrzopghtq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gttdkkydpr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gteeomxntz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtyciquvkb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtkqekeife.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gtarpnlgiq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtdlcymlwo.html


<!-- 参考信息 -->