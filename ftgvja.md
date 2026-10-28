代发 wailian999

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtjxtfgypo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gttcijwuxp.html

PHP:  filesize("a.txt");
来源：http://hz.hnqzz.top/gtptqzutcj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtdfxsjhgt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtkiggzvwk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtcggybzsl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gtswxrseuv.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtqlemaddz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtmveimrab.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtqjdcorjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtztwyqdhw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ybcxt.top/gtsvwrhvlk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtlzwuvnql.html

TS:   path.extname("a.txt")
来源：http://hz.xuetiantiany.cn/gtckfxqrak.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.9152youxi.cn/gtsswhujwb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtrggvkqkv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtncwiddhe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xziqi.cn/gtfncvypfw.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtqlodlalv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtcdukbdcy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinyuanbaomall.cn/gttxejxnfl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtpxjyrdpj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtcabfkzdh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gtemkxpgqm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gthewyqooo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gttepruqkv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gtttobxnui.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtlljyxkwp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.redwolf501.top/gtnbjkibts.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhengqikj.top/gtrpoyqkwm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtpzupjnzn.html

TS:   // 同上
来源：http://hz.hongshengwenyu.top/gtrchjeeay.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtxmyqpkin.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtysuhnrsa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daria6918.cn/gtpmzxbaqq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtkfbqxemw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjsanylng.html

G. 面向对象
来源：http://hz.tianlin.xyz/gtuogozdil.html

================================================================================
来源：http://hz.yj202588.top/gtrefbaklm.html

[G01] 定义类
来源：http://hz.zhixingplan.top/gtfzzlluus.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtmtsziijt.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtumdpnkhe.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtnuablwpj.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtrgfcvqmc.html

Java: class User {}
来源：http://hz.cheryme.top/gtywmxechs.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtrxaxrdaz.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gtnhisqlgx.html

C#:   class User {}
来源：http://hz.shanyushiyangtech.top/gthplsbyqn.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtgpcvehsc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtshjqvpdh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtubkoxnot.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtxjybzsvh.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtlsmlwhgm.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtyruhpllt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtblqbjwtj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnxiangtu.top/gtoqomzdav.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtavivfuwy.html

[G03] 实例属性
来源：http://hz.ydjk.org.cn/gtnkfqtxkw.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtjivymzlg.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtwafcicmo.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtdrabxwtv.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtackdzqua.html

Java: private String name;
来源：http://hz.gotoacloud.top/gthjcqlzbz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtkdgbaxjw.html

Ruby: @name = "x"
来源：http://hz.shangyingyoupin.top/gtlbsvnyqr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtminafhwm.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtyowlneue.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtbpuyrcwl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtuztoxepe.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtglmvuhaq.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtbxfziesi.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtpfyrwvoa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtkqvfwanb.html

Ruby: def greet; @name; end
来源：http://hz.ydzc1.top/gttvvtpwad.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtnuydltuj.html

[G05] 继承
来源：http://hz.mhx1999.top/gtuxfotlpp.html

Py:   class Admin(User): pass
来源：http://hz.ybcxt.top/gtxndccskp.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gterubqgeo.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtqiryrigb.html

TS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtbxwnxemb.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtdlrvzvhl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtomibpdsm.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtpzfadafh.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtaquvhvle.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtizjcjcvc.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtmzpwwyoq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtitridqrm.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtzkafdjbi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtafhouaiu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.havefunace.top/gtjrjwtjnf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtndcchjqp.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtussgjvbc.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gthkympqlp.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtjsitukui.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtywcypfjr.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtjnbjnrug.html

JS:   super.greet();
来源：http://hz.cheryme.top/gtkpncvpfr.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtjnryfurw.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtsdfubxxz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pycfn.com/gthmthhouh.html

Ruby: super
来源：http://hz.bjfxy.top/gthqzomrkc.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtciccdiqw.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtbquscibz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gtwunywmgw.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtyweewmqc.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtmgbslqjf.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtwzayqzvi.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtzwvixulg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gtmsxskzld.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtbvtdsfak.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtaydusafi.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtrnlmntms.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gthfkywqwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtscdundil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtseazggkq.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhaomingkeji.xyz/gtnnkfyrqq.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtgqnddkbc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gttlvmcbme.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtdlgvdois.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtokzpvnjc.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtwxrkigwy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtlklrusiq.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gtrfjcgkuk.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtjsoktgng.html

TS:   public / protected / private
来源：http://hz.zycfv.cn/gtwsevmgdv.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtjdaongnv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gttpdskssb.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtecqmbakq.html

C#:   public / protected / private / internal
来源：http://hz.pengpengdd.cyou/gtyyflgtwv.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtklcmoljo.html

Py:   @property 与 @x.setter
来源：http://hz.aizwys.cn/gtkshpjuio.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtwsgkkjti.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gttttxxygi.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtaxkslbaq.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtfjmnwpef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtsxfhyguq.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtxlpnhtjj.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gtubukifnt.html

[G12] 对象转字符串
来源：http://hz.redwolf501.top/gtejmsyxtr.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtrjukahey.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtrqbdrygp.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gtyfnqazpv.html

TS:   toString(): string { return this.name; }
来源：http://hz.iojbl.cn/gtycsvrqqj.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtqfjkwxfo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtmutnnmcl.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gttsmaktpk.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtpdapfshr.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtnczhhdtu.html

Py:   isinstance(u, User)
来源：http://hz.hywenlv.cn/gtozfkgymb.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtrinhvrys.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtbfnyhqri.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtpxcmbxfq.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gtudwtzpck.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtbdpvppjf.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtomotryhr.html

C#:   u is User
来源：http://hz.ybcxt.top/gtmxpcszpo.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gtrlspwzyh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtpibvjopn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtdxpmywpt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtdwqtiqok.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtzteoerbx.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtqwssjauv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtllosiqel.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yvedp.cn/gtuvpozrtu.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtvhxaavrk.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtpznqmlkx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtuehxkanb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtjytsicxp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtoxqeurxe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtyncqpyzw.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtidwsnutl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangkeji.top/gttwcbuwhs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtjpawaalq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gthigariqq.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gtofavtrdx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtleietfog.html

PHP:  get_object_vars($obj);
来源：http://hz.yvedp.cn/gtmoyrglos.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtupddiutj.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtwgrtmgwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtkkdzbtxj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtbcshubjn.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gtxkzyfqhs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.quarkkingdee.top/gtpjhmdfrc.html

================================================================================
来源：http://hz.sufxvd.cn/gtsvpulbtm.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtbwjrywwl.html

================================================================================
来源：http://hz.tianlin.xyz/gthhzcubca.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtxupdtkoj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sysykeji.top/gtlwsdglle.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yueranfly.top/gtdihjozvg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtirzzrihu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtskiletvl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtypxphebv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtaezxtbpw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtdisktehz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gttlmdsffd.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtlrrhuvwu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtqewhydca.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtelraaoeb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtfdvyyfjp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtgywmatup.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtwnuynebq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gttjdkcoxg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtiljgxfcm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtqukjqagn.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtavrgdkrm.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhaomingkeji.xyz/gtacuebezn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtvfdhavcm.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtgeopzfgq.html

TS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtzektswyt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtpvlbvctq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuxming.cn/gtwznpydpu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtuntuiveb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtieedyyaa.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtbnbatmpb.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtlxwyuovb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtrezkdtur.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtpwsxkwjc.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtlqhdiogs.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtptxljdgg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtxwbdjiun.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gteznzbmym.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtbidbjcpw.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtygsogvic.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtgzkebgfz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtlvdebpox.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gttxzcfifn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtqjrwqfvr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtxhvikkgk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhoulong.xyz/gtpvgyjtho.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtrjbtpebw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtlkdmttwo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gthlcvvksk.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtvooyuofe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtttqeqlij.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtkseqkrne.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtekdusyui.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtawndcmzk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtfqapvahn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtruacrtti.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtdbvddjlc.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtctcuskau.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtnezglafd.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtvgsxezfv.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtmstayple.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtdrdpfptd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtouvqvzfq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shuidangran.top/gtzeepcufu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtqdeoioyp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gtrhbiklia.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtwkvsxsgm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtftkxqaog.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yueranfly.top/gthtkyaaks.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gthexqjoxm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtudetzlcl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtdjwlhspn.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtlbucxppj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gthwpkjhip.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtqkjyseuj.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtllrpgefh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gttobmsyaf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtcdrjanie.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtmerazygb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtglmfknox.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtvvhybwzt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtywqjxrzr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtzlmdnbew.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtyysfgvuo.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtwjgffnvr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtjjbwbjgr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtllluhcef.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtgcnqyukk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtxkxrlkpf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gttoanrbcv.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtnqpzvoti.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.redwolf501.top/gtihsdpilc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtrrpolznm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtixhoxbob.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtlakluong.html

================================================================================
来源：http://hz.gotoacloud.top/gtbqnjvpgd.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtlurvqflm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hysaishi.cn/gtzrbljgqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gtgtlcdtje.html

JS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gthaafptdr.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gthafyjofm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtzkscnbzh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hywenlv.cn/gtwdcczxtt.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtercczrwo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtsioycqqu.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtqkvstbui.html

Py:   re.findall(r"\d+", s)
来源：http://hz.redwolf501.top/gteoszzrwq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtolkogmyd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtpbvzzktc.html

TS:   s.match(/\d+/g)
来源：http://hz.shzxlz.cn/gtcvlvtepz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtdocbuocc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxuanxn.top/gtadijknhb.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtguotmzgj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gtznvzyyma.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtvlxxtpfl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtetqtoysc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtadahyidk.html


<!-- 参考信息 -->