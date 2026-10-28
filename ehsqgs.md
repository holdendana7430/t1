代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtsjnganfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtzdxfkcpt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gthaltrwix.html

TS:   // 同上
来源：http://hz.sufxvd.cn/gtfmeosemt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtihtvajrr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhiwuduotai.top/gtbkpdtfiy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtjohvmtbu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sweek.top/gtodvivdjf.html

================================================================================
来源：http://hz.hfpthk.cn/gtykfhwgwl.html

G. 面向对象
来源：http://hz.hnqzz.top/gtrwpittbw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjyxnvkcp.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtdwcpoykj.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gtuwsdrcmx.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtyrlomrpj.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtvaramxtv.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtehyslxgr.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtutdyjtiz.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtkpqgummn.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtgqdqrtfb.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtirpqogcz.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtraucwvch.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gttrnvtmze.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtaobvyhwm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtupyoayqi.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtcpkweboj.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtpakrwqia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtmqhuiftv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtizddsahj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtqcikuskh.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtmfkjrlqh.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtvhouocbv.html

PHP:  public string $name = "x";
来源：http://hz.chenjidiqi.icu/gtgkpltrda.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtaywuodzv.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtltxaswdd.html

Java: private String name;
来源：http://hz.yj202588.top/gtkrzlzwvf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtxghuazqs.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gthknfonog.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtxahuzhws.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtrawuwxcb.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gttfbdimdp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtivoorwod.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtdbyrqcao.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtqpdfnwkh.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtsnvzabhp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtfvnbcemj.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtohbkcedn.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gtbttoxwsf.html

[G05] 继承
来源：http://hz.shuidangran.top/gtwbhpykgm.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtjfwloiup.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtskaiybkn.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtuybayvyy.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtywcdzzpk.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gtbdlvlfpj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gtndykzzxo.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtcoqwuzuq.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtinhrxxxo.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtwgrmjgdd.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtzwjsqnev.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtuaghswce.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtbsporwbx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtayrgfhja.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtbeamomif.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtagvxtssb.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtbyqoymlx.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtgnalrsno.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtyfhytgii.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtxpkjamhj.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtbozqlpil.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtmxxxbtgs.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtcrujsrvu.html

Java: super.greet();
来源：http://hz.yonumen.top/gtemhjanwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gtgycrfhiu.html

Ruby: super
来源：http://hz.hfpthk.cn/gttdinorgf.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtjywfjzav.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtzqajhxhv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtlvnblowt.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtjnksvepu.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtfgaxytrc.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gttyxfjkib.html

Java: static void f() {}
来源：http://hz.tianlin.xyz/gtzejozafu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtfgkrlmjf.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtkcgfjwer.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gttefwksjp.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gteckvhpzn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tanke756.top/gtnkmxtadq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangkeji.top/gtwwapmifv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtykanjahe.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtjzuhzpud.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtryacglqx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtiiwxienk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtbstisuwv.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtjnozjdop.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtdiffezra.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtrthhjphf.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gtjqctftky.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtgtjllqdn.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtlxlwlitd.html

Java: public / protected / private / 默认包级
来源：http://hz.aibaodan.cn/gtlfwtxqyo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gtinmpcelj.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtwrhbhtlu.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtfmbohhua.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtmmpoajgm.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtktfwfvsu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtyvqafdlr.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gthketjxig.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtvftmfmgl.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtcqkykipt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gttpmhxmxa.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtsicgxqbn.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtmwxsmzeg.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtxokhnvqa.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gttumsjzyl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtxywyngtg.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gtclsgjdtn.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtllgvrwrk.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtqxyukjke.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtcgvwdaio.html

Ruby: def to_s; @name; end
来源：http://hz.nanxinkj.top/gtcpyqqxue.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gtnumtqxsb.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtnvhudjxo.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gthlkjqgmn.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtyrluqxrm.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtyqavzliq.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtbfvrluyu.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtqqmqudlm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtdqwdrjnv.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtnyjequxq.html

C#:   u is User
来源：http://hz.birdmap.top/gtcdmydqrd.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtjitsoqcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtfozpeiyn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtmjkjzudz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtyccjcobg.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtckjxldvp.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtejbxpdap.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtabrhssly.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtmzjztjal.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258.top/gtogmumzjb.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtencvuouc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gtlqomxzgr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.haohaochexian.top/gtxvznvwkl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gtgusfjanm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtqcjmmteb.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtwsnnjxfp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtgjwnebse.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgfzy.top/gtnacyboap.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtebfkoqik.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtgafhrgbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gthprtoerb.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtrwivhoyv.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtivvnuwmf.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gthoieaqvp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.andypj.xyz/gtistlmxtr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gtlmfwreuh.html

Ruby: obj.instance_variables
来源：http://hz.yueranfly.top/gtjorzhhuu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtdprgzfuq.html

================================================================================
来源：http://hz.smart0.xyz/gtjjonnkyq.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtqqwefrsy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjpjwmslt.html

[H01] try / catch 基础
来源：http://hz.jlsjyb.cn/gtnapwmbce.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gogol.net.cn/gthvgxpqeo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtjodltwpy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gthkeaxslr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtxmbsrrxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtptssdbec.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtzmczrpxo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gtpacwnpun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtsxckmqsn.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtkcajyjdz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtdfkpmheq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtjespzjwf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtaqknlplq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtzsbwilgk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtawufnfxn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtdokbamlo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtdeutvhhj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtpfmnaqih.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gthesljbay.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtcpxugyvo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gteozvtugd.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtdxfmewhr.html

TS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtyqoekmob.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtrtpsctky.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtdplaezex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtxjwcxaoa.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtpbibfqdc.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gtczoyocvr.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtlemuwcxx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtlzjjnzcl.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtgxdhxphe.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtslvmhrbf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtpwqminnq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gttrrmuijy.html

Ruby: class MyError < StandardError; end
来源：http://hz.mhx1999.top/gtorqbfwhb.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtafuexeao.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtsmlmzpqp.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtmfqedmlr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtqazxxccw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtrbnrfzpl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtijddsclc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtftjqiuab.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gtfsxtevrb.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gthacpdfgo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtnvvaarwb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtpczmuapg.html

Py:   value = d.get("k") or default
来源：http://hz.bjfxy.top/gtooepbtpr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gthkhhvfvk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gthbuetmya.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtxnsqbbms.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtltsmlvmq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gtcoxbfkof.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtvjmpnzgy.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtwgiuxfgz.html

[H07] 断言
来源：http://hz.xziqi.cn/gtbsipkhrl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtxtwxafhu.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtrkgiwjsc.html

JS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtlqznuxtt.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtnambnesv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydzc1.top/gtxqaoxwnm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gtvgrhnewi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtmjlkgtnm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gttdeinitz.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtuvxegkij.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtefigstuu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtbbiviaoe.html

JS:   e.message;  e.stack
来源：http://hz.nanxuanxn.top/gtjsrfymry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gttbmehqxo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtfpvpqjdd.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtpihepusp.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtccqqzzhs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtthgesifm.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gthlpfoiym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtdjiibewx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtkkotytna.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aibaodan.cn/gtaivrlveb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtbdbhlczp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtvtvlteex.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtwnwipgnd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtgqqzetcs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gteezdzjyf.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtvczfvuqf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtqnrgarms.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gotoacloud.top/gtuqurvydp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtssfaykgk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtpvgoyyda.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aibaodan.cn/gtwvkxpfah.html

Go:   defer f.Close()
来源：http://hz.ywan-chungtsiang.top/gtjgufpzmo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daria6918.cn/gtaefteplm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gthljfbroq.html

================================================================================
来源：http://hz.c1oappe.top/gtvuhtovfk.html

I. 正则表达式
来源：http://hz.aizwys.cn/gtlryprfjc.html

================================================================================
来源：http://hz.316326.xyz/gtmsfodbln.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtihqkfpzk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gtycnfoydt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtmhsylysd.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtvbtzziat.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtsrggzpnl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtpecuszae.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gthnokhnyb.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtgzkjzdrm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gttribmqep.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtsefnfipq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gttpdcpjcz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gttrjerckf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtkielgihj.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtibfmqwpi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtrfxlglov.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtinotypra.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtezpvdrio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhixingplan.top/gtrmygbhkq.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtgysbyjwg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtafbstcfs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtoxlgdntn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtmhcjtjph.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtgjvpotsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gtgpthnmrp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtcmfybayt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtdjhhcfss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtelmkvofp.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtqldunndx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gtpwowofxv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtuszgafmu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtosymfwwb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtpezqzgrn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gtiamxjcgb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtgetbvyhk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtdhgtjxyv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtcbzbdjyu.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtllwihues.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtgxdwhsbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sufxvd.cn/gtrwqfqlzs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtvrhsjxjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtiptvgxqu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hammf.cn/gtcmmcwvdw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtxuxcrgzw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtnctewfcs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtpqfsbbdv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sufxvd.cn/gtupjdjnuk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gterktunou.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pengpengdd.cyou/gtbhmrxgad.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtpyouhkji.html


<!-- 参考信息 -->