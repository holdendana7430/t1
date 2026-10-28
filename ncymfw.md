代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtrzzdngfu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtydrzudvu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtagbtgtst.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtpreionpu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtpzmxxypc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuetiantiany.cn/gtjdushhcq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtslvzulop.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtngcwzhej.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtmzqdcpwc.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtdyixxskk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtdkmtfzxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtheabyolo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtvzbusqul.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtocrgqoxg.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtjefpncgq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtlrfvqiqi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtrirtbaeg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtruiksxwv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtcjgjumcl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtjzhhzeex.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtsxdvtiry.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtnnjiuilk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtwhixhcju.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtlazsvzln.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhoulong.xyz/gtpqhywbgr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cdnleiting.top/gtqxhhexdm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtysmhfzbd.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtrsrneicl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.vqdsnc.cn/gtlrsjobxi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gtfyrtbdyh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtmqlvcwpc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gtmovtexww.html

================================================================================
来源：http://hz.hywenlv.cn/gtphndcpje.html

G. 面向对象
来源：http://hz.smart0.xyz/gtzmjzogen.html

================================================================================
来源：http://hz.c1oappe.top/gtirnwwgqd.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtgnzuzkuf.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtctbtefxf.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtrlxynzib.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtlzafxxnj.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgufenzy.top/gtjpobifzb.html

Java: class User {}
来源：http://hz.cheryme.top/gtadrcctyl.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gteyypefzg.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtcgatdogn.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtfjqakjes.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtpogznwcp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtxugjnsma.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtmmwftfrh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtejftfhjf.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtdpbahbna.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtlctfzzjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtprnpyqyv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtixrqusep.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtalakswxx.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtgcerxdoa.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gteticpsii.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtudmclwdr.html

JS:   this.name = "x";
来源：http://hz.52xcode.cn/gtivllyfqp.html

TS:   name: string = "x";
来源：http://hz.sufxvd.cn/gtcxalliot.html

Java: private String name;
来源：http://hz.316326.xyz/gtwlrqqdxk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gttiepokfm.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtvinhclvi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtvsmbnlig.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtbqjwfegb.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtbzdjqkmo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtzewtvcms.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtanhujupw.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtsdoakvhp.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtsyxxxbqa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtujcxbghj.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtjsmciasv.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtjbqnispu.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtaiqvtyiu.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtujkhjrlj.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtqaounasw.html

JS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gteptkflbn.html

TS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtifxrdccu.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtmdqejwrr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtbnfqvytn.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtadbejmcn.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtzrejudvf.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtgbagfyjs.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtdkzzghcq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gttjvaqelj.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtmkchlnko.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtcmoksoit.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtsarscubk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtdxyytjgn.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtoszsccph.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtrwopnpqb.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtphuxvlhx.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtvfefshxo.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtoglcstkv.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtifdwikks.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtqnizznht.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtysbjahra.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xingfuxueyuan.xyz/gtocbkolmd.html

Ruby: super
来源：http://hz.aibaodan.cn/gtidsjhnik.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtnluqbwsr.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtodmkitej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtzoiopgxa.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtpnpcirzq.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtkgyroztt.html

TS:   static f(): void {}
来源：http://hz.feifeiyinyue.top/gtwxuoxkba.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gttrqxalcw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtzybilbpe.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtmmykftyp.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtfpjctfdf.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtanuxisfb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtqmadnwbb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xinyue.icu/gtcmbnaafn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gtnhpmphlj.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtlwbpbplc.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtzbbjguyd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtryjrujha.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gtagpyvagd.html

C#:   interface IShape { double Area(); }
来源：http://hz.ybcxt.top/gtmdrkaxez.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtuljmivzk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258888.top/gtolriqxii.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gttiklzohb.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtvrwcxknv.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtqfvcyklq.html

Java: public / protected / private / 默认包级
来源：http://hz.sweek.top/gtdgepokvj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtvuahpbws.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtfytpirae.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtiwiqhekz.html

[G11] getter / setter
来源：http://hz.cucudq.cn/gttaaizrlo.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtvilmnyqh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtpyfgjuhr.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtumzeaaba.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtiepguzuk.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtnomcmviv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtiacnmcrg.html

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtddcrbumr.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtcljksqds.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtjhpvzacn.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gttcajgpwe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtvbwfdcpf.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gttywyzwku.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtunerskof.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtoyyzdibk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtqanjikju.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtxnulfryq.html

C#:   public override string ToString() => Name;
来源：http://hz.hnxiangtu.top/gtuxklfrpy.html

[G13] 判断对象类型
来源：http://hz.iojbl.cn/gttnntmvyd.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtuivmslrp.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtrfolvuit.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtdviokpbs.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtswmkckeu.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtzladqanm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtbxccqdjs.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtvsvbrieh.html

C#:   u is User
来源：http://hz.iojbl.cn/gtykgkqtfb.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtkippdvfu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtozyuitla.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtxlueigyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtjfpfrgru.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtekfxflua.html

Java: record User(String name, int age) {}
来源：http://hz.havefunace.top/gtlxedivdy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtixvhbigu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtpmazmurf.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtvxwpfkuk.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtvyqbhvbj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sufxvd.cn/gtzcxmpqfv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gtoyatpoyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ppjwa.cn/gtwyrhcssc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtvbfilcbk.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtyjkhuoqu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtilnntvaj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gthvzejhwe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtlvbsjgqe.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gthzuhnevz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yongpay.top/gtgokhdzpq.html

PHP:  get_object_vars($obj);
来源：http://hz.gotoacloud.top/gtkovbbcqf.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtldydqbci.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtnyfdyjkt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtwetgfpav.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtjxhunlvd.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gthngdfgcq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtrmyzljsw.html

================================================================================
来源：http://hz.chenzaomai.com/gtqqetrchc.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtlxjixzdk.html

================================================================================
来源：http://hz.hfpthk.cn/gtcufbhojh.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtsdqkaeee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtspnkfsqv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtxdafkpyc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtuzfpeeke.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtajrsezog.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtaktmrden.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtmfakxyjn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtfgmxkeho.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtopdgaqla.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtwxlcnfpu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtknstyrfl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtooyfibss.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtqdvwnczj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtbzycvvqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtkdsrngfz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtstqfbqoq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtwcyprgjo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtfxleglkg.html

[H03] 主动抛出异常
来源：http://hz.chenlongwang.top/gtmhpslnku.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtqsckkjpq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtakgdtanw.html

JS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtnvqxdzis.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtwseaywam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtseuqpipz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtzrfgoxhq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtlgbkljdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtqmpjanna.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtidkkikae.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtfeoxnimk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtbbgwmngc.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtoqwqfays.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtfrrmzdjj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gteboxsnct.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtkckwtmxs.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtpyqmlusz.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtbgdzqbcc.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gttjprvpeq.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtcdnvtywb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtijjawwti.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtdgelmcpb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtjysuphwl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtndxquyhh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtvoshxtlf.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtssotttqn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtgvcfrttj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtrcvbddaa.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtnelgwify.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtdolbqtva.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gteamxrubv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtqfvpcsou.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtltfgpwgo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtieewuxym.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtvbzhsejb.html

C#:   obj?.A?.B ?? default
来源：http://hz.hywenlv.cn/gttwqoueos.html

[H07] 断言
来源：http://hz.zdqjudy.top/gtumxiofbq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtryjceucz.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtxdwusjei.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtbuquhpcq.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gthycgefmj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.bjfxy.top/gtqvbgqafd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtuzlxhcmt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuanzx.com/gtwxjxmjpv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtscvcejlb.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtgammvylu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtbwalcalv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtquflrtqe.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtvrslgkjm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yvedp.cn/gtuuigvvrm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtoxpioqrm.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtaktnjqrk.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtzhhtgnrd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtlqdnsfao.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtkjqscdaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gthubvmzzn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zdqjudy.top/gtezphqown.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gteakewgwc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhijiandao.cn/gtgitzlhzm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtjcfzprud.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtvwvaenpg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.bjfxy.top/gtkcwdntfw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtdhgqnksh.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtjcnfgtwz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtxtgjcgfk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtkedasxcs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtdgmzpkwu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtnneycevy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtrztvrsvw.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtqsabixzi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gtzcvcwlyb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydjk.org.cn/gtblxbtzdq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtspllenyv.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtavedsast.html

================================================================================
来源：http://hz.cucudq.cn/gtimbvjgzw.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangkeji.top/gtlhkfrruu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtqjnqnuof.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtpukjrmiv.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtveowrbpp.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtekfdhkef.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pengpengdd.cyou/gtxksvigtb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtwqajozno.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gttgyuzoat.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dashuyun.cn/gtvaqejjlt.html

[I02] 提取所有匹配
来源：http://hz.gzhubu.top/gtjtexmrzc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtolztgwtg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gthmrsosdp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtymmmlcfv.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtgllicbvz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtaoyxizdo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj202588.top/gttarazios.html

Ruby: s.scan(/\d+/)
来源：http://hz.kuanghao11.cn/gtvckhakbz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtkrlsvdqp.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtleokhuum.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtdzssmpps.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gtutczisop.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangkeji.top/gtzlsdgrrp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtssotpepe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dianchejie.cn/gtpqltqsms.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gttwxzawgm.html


<!-- 参考信息 -->