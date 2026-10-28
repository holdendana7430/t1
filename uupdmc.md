代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.kuanghao11.cn/gtcuuazhvc.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtvyjzspey.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtfloulhqw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gthphwawrm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtiztlsset.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtwhpctzik.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtywaalnmi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hammf.cn/gtgqypsonp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtinthzrpo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gtubwfxmux.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtovqcgbrj.html

[F08] 遍历目录
来源：http://hz.chenlongwang.top/gtspigcyas.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtlypugnno.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtxsvgokli.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtqxoufapo.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtrrajkoxy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtonqczyzj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtefiskdbq.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtybhdrahm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtwzcttqbt.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtniiwpzcu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgufenzy.top/gtaxaljqwg.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtaqxkmarn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtfwwdreab.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtcpnxeyvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtvqbuefqt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtaiuquheg.html

Ruby: File.size("a.txt")
来源：http://hz.hywenlv.cn/gtesomomvc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtudyahafj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtwamlilay.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtdwrrygbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtbqiirfoh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtsqrchztc.html

TS:   path.extname("a.txt")
来源：http://hz.cashguo.top/gtiuylhand.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gtjzgemcts.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtffptbafe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtcfunryhx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtjvmxnzvf.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtbcoescra.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gthtlbujkn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cashguo.top/gtvflvolqi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtcafixngw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gttsabkgol.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtvojjxhpf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtlgwnvtjq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtqjaktfuy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtfcactcjr.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtmzxgaqzf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtufulppxc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtpwxhaokq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtdyoywpkm.html

TS:   // 同上
来源：http://hz.tian-w.cn/gtseilpwdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtybqfopvy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtyddidmcu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gtkgudqezi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gthfhyurwj.html

================================================================================
来源：http://hz.yj20258.top/gtatbmlmyk.html

G. 面向对象
来源：http://hz.zhiwuduotai.top/gtgknyyeil.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlhfxqtiv.html

[G01] 定义类
来源：http://hz.cheryme.top/gtixvptoxo.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gtrntdhcmc.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtcbwjbkgv.html

JS:   class User {}
来源：http://hz.havefunace.top/gtovaefxxx.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gtcfgotsxk.html

Java: class User {}
来源：http://hz.zycfv.cn/gtndmpxkqb.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtuzdnewjg.html

Ruby: class User; end
来源：http://hz.yueranfly.top/gtsinpszyp.html

C#:   class User {}
来源：http://hz.meibo888.top/gtvhlscvvl.html

[G02] 构造函数
来源：http://hz.yangfankeji.com/gtqgykfwfq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtiptfyiwz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtzsxqfrdm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtjjujvlhd.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtivqqfftx.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtudqzavwo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtvyxeajak.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtnrgvzoay.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gteopupsxu.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtmkgbjgrv.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtpytcsujr.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtkdetcglp.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gttxwnxnml.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtxjybtnpm.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtftkngqiz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtgypyltvk.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtwrmaawvg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtsuhjzeyx.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtcrrrhtgv.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtbazulyro.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtojmcfuer.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtftijyjzt.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtrywhmhsi.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtwwpdwcws.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtwckyrmsa.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtqdvmvdpl.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtqtealpll.html

[G05] 继承
来源：http://hz.ybcxt.top/gtahyaxkca.html

Py:   class Admin(User): pass
来源：http://hz.zhixingplan.top/gtgwucxcvl.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtvzfehfiy.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gttuelorst.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtenrlyjxc.html

Java: class Admin extends User {}
来源：http://hz.guannengcc.top/gtcycgevcv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtemolkdrd.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gtolzvhkcn.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtyugvjeva.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtvtfddgls.html

Py:   def greet(self): return "admin"
来源：http://hz.zhiwuduotai.top/gtwufzbgoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtpstsolrp.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtmpmmaybk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtpclgyxis.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.havefunace.top/gtsssvmyfi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtokctpxwl.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtklmilhnk.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtncwlpwfb.html

[G07] 调用父类方法
来源：http://hz.quarkkingdee.top/gtdnwhvsed.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gtvnkorxnh.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gtfmciyqtz.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtyufthtsm.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtgzydxvfx.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtoudkehzv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtgerzzdtn.html

Ruby: super
来源：http://hz.shuidangran.top/gtpayrzfbw.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtpitzrwvc.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtwncomkww.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aibaodan.cn/gtvchgcxrn.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gtygbmbett.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gtocbqtehr.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtkphzdlgf.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gtqisxmlfc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gtclkssent.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtpaygoegn.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtzagkgnfn.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtfpycdulw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sufxvd.cn/gtgdxmjydj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtpujurbax.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtelgjhwpx.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhijiandao.cn/gtntbcsmse.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gtkedstngb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ywan-chungtsiang.top/gtvuqsdybs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guannengcc.top/gtbjsluqpi.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gtvwktsoyp.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtxngwawuk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtzfwlbndf.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtttscfhxc.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtsswkwjig.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtevorcqbc.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gttycdimtk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtsqfkegiw.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtsageyrqk.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtmoxpwnyz.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtncnywvkd.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtipukayba.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtstpluoie.html

JS:   get name() { return this._name; }
来源：http://hz.ydzc1.top/gtsxjwvbaj.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gttvhipmbx.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtpfzbjaqd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gttqvcdzwc.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtewcjdcqm.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtpbuofpkw.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtruxjhelp.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtgzizfamj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtnnnececs.html

JS:   toString() { return this.name; }
来源：http://hz.nanxinkj.top/gtszclxjxx.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gtvrxeapye.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtdtgcbdxi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtashrecsc.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtphnieufz.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtkdsvfsxq.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtetecdpbf.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtdroixiut.html

PHP:  $u instanceof User
来源：http://hz.yuanzhike.top/gtbokzoyyh.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtxtadabzw.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtmbmmceqr.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtgkoecesv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jiagoushi.top/gtphhwcbqn.html

Ruby: u.is_a?(User)
来源：http://hz.yj202588.top/gtfjzxtavu.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtwdtejwom.html

[G14] 数据类 / record
来源：http://hz.cdnleiting.top/gtdarmarin.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuxming.cn/gtvbnjikma.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtieudilqz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtgmopqarw.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtltyqyhoc.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtsfkxfghl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtxicderus.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.havefunace.top/gtbdigpmmm.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gthlumvixx.html

[G15] 枚举
来源：http://hz.cashguo.top/gtugtbfqja.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtokilkplt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtznmgbriy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtfdswiolw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gttxyjqryn.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtqdzkjooj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtmrdmcftf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gttzsvrdmq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtxirqqgtc.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtykoxvvlp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtnuhgippc.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtmgfpgvip.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtnndqptqp.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtwxqjxgwo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtxswbfbro.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtydwqpaat.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtjxpkhbyk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gtflyettpj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxcafcldp.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtfwynyiby.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpouigbsq.html

[H01] try / catch 基础
来源：http://hz.chenlongwang.top/gtohdcknvq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtqzailvip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtfaaxhyqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtepuxedzk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtklzqgifm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shzxlz.cn/gtcegipsfy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtmqhhehsg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtnqhhsvsl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtjanxniit.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtjkkqdpat.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.52xcode.cn/gtpugwuxlc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtqsokwbwf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtvorzlvkb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtujpuktqg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtldqpyetp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtsbeazrck.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj202588.top/gthxgfpbld.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtebczufcv.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtyftwyxem.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtatsvmyri.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtbkytknxz.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtrkttflzq.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtdsatzxhl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtoawwonhu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtvrdtrmor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtsfzsdlog.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtgsurcapl.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtpaeoojdi.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gtvzzljogv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtjivluhop.html

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtsyhxfchc.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtszfchmzb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtibcqjtlc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtvzplsoua.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtixaiebtm.html

C#:   class MyException : Exception {}
来源：http://hz.hnxiangtu.top/gtqvvfkide.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtihmpcfgr.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtarfwfsbn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtqodzttxt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtholucupk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtpzmcmfzk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtkdosatxo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtpkcufaxr.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtayprmcjc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtktksazlm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtqxgmwyho.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtctwwyemr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gtqztyjufz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtfsznxbrb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtdccljsgi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtmwvkuwyi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gthppmugaj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtwolnppfh.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtzqrlfsfe.html

[H07] 断言
来源：http://hz.birdmap.top/gtmgidwuwl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtemzyqvnz.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtvsktysas.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtowjgljpq.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtzchkhfwt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtmuaxkuam.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gterlzgafr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtpafhhzqn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtobirviut.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtkzpslbsk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtazgvletc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.haohaochexian.top/gtbmpglryo.html

JS:   e.message;  e.stack
来源：http://hz.chenjidiqi.icu/gtdlgkgubn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtyidhrpbm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gtlguphuhe.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtksikzofo.html

Ruby: e.message;  e.backtrace
来源：http://hz.52xcode.cn/gtjoxmknux.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtcplazsyg.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtnplemrlg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gtnvikatpg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtvirajgux.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtwmcctmjz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yueranfly.top/gtqbzstedi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtvhahpvph.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtfaornfva.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gtajuzfixk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgfzy.top/gtgavpztmj.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtgbmmzrma.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtblitqzsl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtdqtalqnm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtiamkoarq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtkvurrwhy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gogol.net.cn/gtczcajoeg.html

Go:   defer f.Close()
来源：http://hz.cucudq.cn/gtrhvihzqa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtmqfbxqzy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtuqmrpimq.html

================================================================================
来源：http://hz.tianlin.xyz/gtikwcdzqf.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtjsiqhxyw.html

================================================================================
来源：http://hz.guowangkeji.top/gtdmahsvpj.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtiznoelct.html


<!-- 参考信息 -->