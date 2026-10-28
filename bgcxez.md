代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtsncktpzq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtjfyrtqqf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtaqmseqgc.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtuyjcpbmv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtadzdzdrk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtygbpilnm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtbvqbkhcv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtlqkchzyf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqpxapjhl.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtbzomdacv.html

================================================================================
来源：http://hz.ybcxt.top/gtybchkfka.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtegwvvyep.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtblihahtb.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtspkvoveh.html

JS:   class User {}
来源：http://hz.yonumen.top/gthxnwieae.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gtcrwzzxlr.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtcmeiaowg.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtbwbhmnhy.html

Ruby: class User; end
来源：http://hz.sweek.top/gtoxqoqbrj.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtguwdzksz.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gttzdszgxt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtwwfollnq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gttgcvxmjv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtnraxrlid.html

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gtexiawwgh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtjdisiyfh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtadbgrteu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gtavqrgsho.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhixingplan.top/gtaiwlnanp.html

[G03] 实例属性
来源：http://hz.ydjk.org.cn/gtbepemlid.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtvxwobkrv.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtghywfstm.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtvmopcmua.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtjyxcleeo.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtoogbuuwg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gttgyrexjb.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtcmlbfkjz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtpzglsypn.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtqnkaaeer.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtlkglxjxz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cheryme.top/gtpbnqvkwm.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtptqxcuhy.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtxknidzsf.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtmnazjimg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtampurnpz.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtyhsjpztf.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtzpnyezgi.html

[G05] 继承
来源：http://hz.meibo888.top/gtwtwzjghr.html

Py:   class Admin(User): pass
来源：http://hz.chenzaomai.com/gtlbkhpenl.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtrpqzunse.html

JS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtudixrzfn.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtkrdbgfew.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtqvtvdlwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtloekedcz.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtiqdvasxg.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtxrwtboij.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtepehucjf.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gtrudkzypa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtmifkcqpf.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtuocrlkpd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtyohoeskh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gthycabovm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydjk.org.cn/gtxhidptiq.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gtlzbdnnkp.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtxycnybez.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtwojryxzy.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtturkldhi.html

PHP:  parent::greet();
来源：http://hz.yongpay.top/gtwpqtfwfd.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtpzrmvolx.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtpoouerwp.html

Java: super.greet();
来源：http://hz.hammf.cn/gtxpzshniv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hywenlv.cn/gteevfcrog.html

Ruby: super
来源：http://hz.sufxvd.cn/gtiwkxsiko.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtgeqgylml.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtdvqvozjp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtvotcgkos.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtegcifcdy.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtftvxydxo.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtkewiwdce.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtyaredicy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtsmsgbhtg.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtlhayptck.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtpzkvdgbg.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtgnsizblm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gtddtfgaed.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtkdcxjrzs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gthnkkhrji.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtzfymyzst.html

Java: interface Shape { double area(); }
来源：http://hz.zhengqikj.top/gtpdrvvjch.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtmqrnpskz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtixpgihfj.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gthnqqqtbt.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtkbysokpd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258888.top/gthpzysjqy.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtqrysqsih.html

JS:   #private 字段；其余公开
来源：http://hz.quarkkingdee.top/gtzpbskgxf.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtqwwoqwbi.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtkcshgnwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cqqwz.cn/gtiaylsnux.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gthdqxhldw.html

C#:   public / protected / private / internal
来源：http://hz.9152youxi.cn/gtrwsuwoio.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtaeniudxp.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gtmfjvvodv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtudniwbbw.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gteqsdagvq.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtqyyrjzvp.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gtprpucikg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtablrhskq.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtfpqtljwp.html

C#:   public string Name { get; set; }
来源：http://hz.jinghuilouyu.cn/gtejnckfly.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtizcynajo.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtxtyzzipw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtzgpyyjgb.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtaaiiaoye.html

TS:   toString(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtcwgndlse.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtvbyuvyvm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtjwtucaes.html

Ruby: def to_s; @name; end
来源：http://hz.ivvv.top/gtuknyacwh.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtyujctgfl.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtfpnlffpe.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtzbkroldt.html

PHP:  $u instanceof User
来源：http://hz.hnxiangtu.top/gtwrfjnloe.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtreynvajj.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtpskehayw.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gttermgzny.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtopeqkrco.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtnbxfywqa.html

C#:   u is User
来源：http://hz.52xcode.cn/gtadfonang.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtjxnthhxq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtzdmgeirs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gtbmocsyym.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtjzftczsh.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtrmtjmkno.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtzwbrnytg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtlybjgilp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtmrtxoptp.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtceeftnnf.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtfwuzyjyq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtxxtzkhmq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtavafbqmg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtmuokgici.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtvwufygey.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtgvsshcuw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtezpjrxfw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gtvmgujkgl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtlgjegwiw.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtogljmtcm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gthexmcrbd.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtsgmvlitt.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtsmsjqzar.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtzgsoadlp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtpryhoquh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtfooxuwro.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtjkklhykt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtmtqhscog.html

================================================================================
来源：http://hz.fzhhl.top/gtvhdnggsk.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtjfdppvcf.html

================================================================================
来源：http://hz.sysykeji.top/gtyzapvjrh.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtilwycdhb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtmkgnhqeh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtolawatgk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtxibkrlta.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtnrgurnvh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtrsekzggv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gterufnrsq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtehagytal.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtzzijqexy.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtqsdaouig.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtpgddaefw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtfonfvxuk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtfjadyqzf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtwtqkrqcs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gthdxqtnev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aizwys.cn/gtxubzrxmi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhiwuduotai.top/gtanytyttc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtwicficoy.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gthllczqiv.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gthyjhmaaz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtqeasogjw.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtputxlbsk.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtcybbytjt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtthyogona.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtjxbfppos.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhixingplan.top/gtkusglkaw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtqufsgllq.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtxjdrxtii.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtbvxokhml.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtshzivwtv.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtsgjvnfdh.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtmtyxlqjk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yongpay.top/gtgqjrtvmo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtffjlywep.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtlvctltwy.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtzcwaommf.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtihvudmws.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtoupcbnyx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtaerxwoau.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtzbhxypfl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gteylfjxwt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtoegyhsyu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtukxzyero.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtbjgympal.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtketnhaxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtgyfjxgxt.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtyddsohue.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgufenzy.top/gtlbwicvjy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtnbifsyaj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtxexephbg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtcbjfojsa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtchqncaqm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258888.top/gtnbehswkz.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtpausemkf.html

[H07] 断言
来源：http://hz.sysykeji.top/gtntycxguk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtxugwkdjk.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtnamccqrt.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtuqkmjzlz.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gttvstaukk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtvdrrlhhb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtmykulzcf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigfzy.top/gtkinmrzzh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtlhgrarui.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtpggqnljv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gtmnpsgcey.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gthuksbzmw.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gttiwrczun.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtrqtcilpz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gtmpmzyvxz.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gtigoozfvk.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtmateilpk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gtwpiynsht.html

[H09] 带错误码的异常
来源：http://hz.ybcxt.top/gtarziahde.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gtxtbeshso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtyhqfqvhs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtonbidqir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtoqtapjlb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gotoacloud.top/gtcickutcs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shzxlz.cn/gtbbzpvvjr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtedtheipw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtqttlmhxn.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gthidkairg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtlvvwqbfk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jyoumei.cn/gtbcqalmzx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtulxjoiow.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtiakhnrue.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtsbyhznsl.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gthhklryvy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtalqekhkt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtinubwwaw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrknodwze.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtboedtahw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtikgyobpu.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtxjvurypu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtwllhjsec.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gthwhsncpx.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtkxwzeika.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtxpwammwp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hongshengwenyu.top/gtboqcdzee.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.0kj1m.cn/gtkhmdmdsl.html

Ruby: s.match?(/\d+/)
来源：http://hz.svipenyu.cn/gtbqxddzrw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.0kj1m.cn/gtlhddtgzo.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtnanktrze.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj202588.top/gtyhbpfhdy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtwigjxwhx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gttvqinxqm.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtynfvbvlj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tianlin.xyz/gtxhatqoxc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtpglycjho.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtzlkpuinf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtxkdevtcz.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtrdbajzgi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtwxtqlcxk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtuvtyjqqv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtzeuzmyrd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenlongwang.top/gtjmvzycsj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gteafhzvpe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtupaunvko.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtmzwimkdq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtlizvppcz.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtvtrffklj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtxgafpbml.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtltpchtay.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtfttxuwxb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtreloraii.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtuqeyumvi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtsgtefdaw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.mhx1999.top/gtoawkrshp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtbphtarfi.html

[I05] 按正则拆分
来源：http://hz.yueranfly.top/gtehrnwwbi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258.top/gtopheadty.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.smart0.xyz/gtrfszkhce.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtrinbfiog.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtduubdjdi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhixingplan.top/gtuqrxdyuf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtmsixavwl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtffljqdka.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtqkhifxmz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gtfzgbqiro.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gthbazzels.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtildbflgc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtqaxreuhl.html


<!-- 参考信息 -->