代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhijiandao.cn/gtdnwcaytf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtcompmxzi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtmczejrgu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gtilcvvuhh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtzjedeuqf.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtdaslqery.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gogol.net.cn/gtjgazpcta.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtbndtkjwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtejagbzxr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtpfggofte.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtghqbwjef.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtltgxaqoo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtitlgsyke.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtvalaidjh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtqvnniqvw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hammf.cn/gtbsblonsg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sysykeji.top/gtqtngrqxe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtyabrnxnq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.svipenyu.cn/gthivewyzr.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtgfoodvcs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtkypdgkhk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtabhdctii.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtgdapdixg.html

TS:   // 同上
来源：http://hz.daxiang520.top/gtznaakqci.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtmziwapuo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigfzy.top/gtgkfxxbgw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtwkdsgnid.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtgxgswtfx.html

================================================================================
来源：http://hz.sysykeji.top/gtqfjnsanc.html

G. 面向对象
来源：http://hz.dashuyun.cn/gthjdrggwc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtknegxonc.html

[G01] 定义类
来源：http://hz.ehwqpu.com/gtiqwpgnrk.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtnokifbjl.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtqrsqznlx.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtnvsxqhvc.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gttjkhmwbl.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtdhcdztxq.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtnfktadms.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtuutiylpm.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtjbrljbcs.html

[G02] 构造函数
来源：http://hz.yj20258888.top/gtudodcynx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gttshjbnyj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtyygwggjw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtixhoffhs.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtvsallvhm.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangdashe.top/gtxekzxmqt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigfzy.top/gtheggoewg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtqzmzxdaw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtwryaplfd.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtvevmffyg.html

Py:   self.name = "x"
来源：http://hz.hywenlv.cn/gtghehvxau.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gtngxmkqfa.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtumjxmrgw.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtrowosvlq.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtqyoqelxw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtvlzwvsuh.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtlcjdpown.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtmoibgwog.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtmsbfqlqb.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtihjvvmci.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtddyhrqmh.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtbfiuezvp.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtxlfdfmiw.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtpvigpixr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtrbuuthpk.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtnlopacmy.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtwejzswxi.html

[G05] 继承
来源：http://hz.feifeiyinyue.top/gtghgzmips.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtjcbztfcz.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtsnifrlgc.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtqiyoaykj.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtldivqhos.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtotzwjkin.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pycfn.com/gtbpyuxgcl.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtmovlkmkl.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtzixtieau.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtjmgkdqxp.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtctqigwzn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtptjwtekr.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtpjclvlae.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtvodsrghw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtrztovupu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtukicwsam.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtcofbwxii.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtdhimcpau.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtahnnzqqh.html

Py:   super().greet()
来源：http://hz.yj202588.top/gthdflhnio.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtunicprsj.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtssymhdyp.html

TS:   super.greet();
来源：http://hz.9152youxi.cn/gtabuxfjht.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtmxbjgabo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtknouxlol.html

Ruby: super
来源：http://hz.jqgfzy.top/gtcenyrxxm.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtkbdfrbul.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gtacakbpqr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gthmzrplsg.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtlrmjhbid.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtqxztbtvf.html

TS:   static f(): void {}
来源：http://hz.shangyingyoupin.top/gteprfbyzc.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtbhcduhvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtxbdqlcgo.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtjclpgrqa.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtzgmaybsz.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtkgtcthbx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtllazpmca.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtxkoxiabu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yvedp.cn/gtgriivhyz.html

TS:   interface Shape { area(): number; }
来源：http://hz.0kj1m.cn/gtlsqccdxy.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gteyfhnwct.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtikoumvbz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtikmbinyt.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gtylalaeom.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtxnhxtouc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gthonsejel.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtfgroqrve.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtwasanahs.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtjnafijzf.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtuwjxgzlr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtaeksghzn.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtteiutyso.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtnytrbvle.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtgzeapblm.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gtwulgredm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtiftbmuuh.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtzcnnknkf.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxinkj.top/gtyqibdniw.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtzytmvsfe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtryvxircn.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtotosqhop.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtsobsgvks.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtlxecivjs.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtqmmizfbb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtqajlfnms.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtvlxjnvxc.html

TS:   toString(): string { return this.name; }
来源：http://hz.ivvv.top/gthmnhekgp.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxinkj.top/gtxnqwocdo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydzc1.top/gtydndzpqr.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtjzfranbw.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gttxtfngss.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtqbobatjo.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtnfdkemfl.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtrjmtldoe.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtmdtsebug.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtkmrdgudo.html

Java: u instanceof User
来源：http://hz.0kj1m.cn/gtgsarbdsi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtrifqpqcg.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gtqusnuhvf.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtrdgczszw.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtcwmdqvcs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gttfddwnmn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtonetflwn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gtrzqhmivg.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhaomingkeji.xyz/gtxvwpgxub.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtdqgwfqqk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtlnetghfh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtefgbtlsv.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtpxseyrju.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtckcxypzg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtwytyluyc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtmjoezhtc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gtgglvixhl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gttbqrmzts.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtzjkizhxc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aizwys.cn/gtxlwokkai.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtyxhsuujh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtudmykzqs.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtjulabdxn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtzzbihlad.html

PHP:  get_object_vars($obj);
来源：http://hz.gaohongyu789.top/gtvcwwvmir.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtvbebbwmy.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtomjvnoeg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtsepgeuyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtbafrxgsa.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gtrxddfqsy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtcarvriyl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtviliambw.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtafirwmji.html

================================================================================
来源：http://hz.yuanzhike.top/gtyetimplt.html

[H01] try / catch 基础
来源：http://hz.havefunace.top/gtmpuutaqx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtyjwdpick.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtudeqglti.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtkmkjyhum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hfpthk.cn/gtmanezmtg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gtymlgujfv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tianlin.xyz/gttzfuofas.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gttqdvpanr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtchiyjbjk.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtdnsxemub.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtbkqzcbzj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtrkpwuchi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gttzsxnrhg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtflednqrd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtjtnroabi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenzaomai.com/gttxbvvvyi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtuortqnhd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtrfvisqct.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gtgbkrymmd.html

Py:   raise ValueError("错误信息")
来源：http://hz.yanxiufei.cn/gtjcwbtips.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtxwpxpurl.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtyikeocvo.html

TS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtwdvrkhti.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtvjkkcach.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.birdmap.top/gtfnsojung.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtolgbdtex.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtnmqrcejr.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtfqfsdzbc.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtqkaziods.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtodsicybk.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtpzespswe.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtruiogdvz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtvgvqfobb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtijeagbrq.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtubutcarb.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gtnijksziw.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtcqvcfest.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtnaksthau.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtazhzucvd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtrzuwortk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtbyftsebw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtxhsnmhjn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtednygxcc.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gthfsbqywx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gthekifbim.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtvezorkmy.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtbyayxhdl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtvdbunltf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtzlwrtrie.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtlhpowkzv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtmqrlmnyd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtqtuzsppj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtatyhnndo.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtamnipuib.html

[H07] 断言
来源：http://hz.hammf.cn/gtdbipqpor.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtzhbkjrek.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtukpzrbhm.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtgqidrakz.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtlhpxhrby.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtxmgwmkbl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gtsgauhpvb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtnamwprny.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aizwys.cn/gtaesfuoac.html

[H08] 获取错误信息与堆栈
来源：http://hz.yongpay.top/gtodkeennp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtqboaqboj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hysaishi.cn/gtsohxajik.html

JS:   e.message;  e.stack
来源：http://hz.iojbl.cn/gtjsdlymgf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtcuoghdha.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtnnpvtmhm.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtrqoodcpq.html

Ruby: e.message;  e.backtrace
来源：http://hz.hammf.cn/gtxwjdyfdq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.redwolf501.top/gtfgmyyydz.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtbjeynscd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtpeibrfbw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtqoecwlyi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuxming.cn/gtozrzszwn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtvrmpyqsy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtqkvjbeho.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtlmnfsbpw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtgchzjufr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtapqkrrxb.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gteyksawki.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shzxlz.cn/gtxqshohqf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gthwldjuuz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtdulzfwax.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtgxqabowf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtpgyzwiub.html

Go:   defer f.Close()
来源：http://hz.pycfn.com/gtknujltlr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gzhubu.top/gtjphkigbq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtitnprpew.html

================================================================================
来源：http://hz.gogol.net.cn/gtmsvwazwh.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtfwljuctf.html

================================================================================
来源：http://hz.birdmap.top/gtxvvdmmbf.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtaqidlcjn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtblnyertd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gtuxitzxeg.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtmmvfqhvu.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtpohutdbn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigufen.top/gtsczkrevf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gtayupcwoc.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtnxhltfic.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenjidiqi.icu/gtrwpopfeu.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtxiilymhl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtpikcntnk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtrkshwerf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtxxbeiyaa.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtpgkloqiy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guowangkeji.top/gtswqhulvb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtmhwmrmub.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtasvhfkid.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtiunolobj.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtfefobrno.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtkmomlytl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cdnleiting.top/gtwrfwuweb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtelvvfqzh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtfvgsldqf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtywwfcuox.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtvntqpayi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gtarqbswaq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtpbbbjvpx.html

[I04] 正则替换
来源：http://hz.yj202588.top/gtqbavqfvt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.mhx1999.top/gtaptjhtls.html


<!-- 参考信息 -->