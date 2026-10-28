代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtpqpmgufs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtddmoecfk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtggtnffyn.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtodhwpwud.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gtezzbufgt.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gthgtdadwv.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtafxhpcwj.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gththnylhv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtcveuhizi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtnfzbnqad.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtpectblci.html

Go:   os.Remove("a.txt")
来源：http://hz.ybcxt.top/gtqnafgtfu.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtevecdwzi.html

C#:   File.Delete("a.txt");
来源：http://hz.meibo888.top/gtrxrwogji.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtjzovmsiu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtetqxheul.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtlgataegt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtzqyubelv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtdaikhmlw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtpucquprm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtgmommirh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtasjtyikh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhaomingkeji.xyz/gtogvlscqd.html

[F08] 遍历目录
来源：http://hz.zhiwuduotai.top/gtoqicepox.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtbuprtvea.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhongyouzk.top/gtmrdlqhjo.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtsbcsicrr.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtdytbgoue.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtuynrpmyx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gttalbqxxx.html

Ruby: Dir.children("dir")
来源：http://hz.sufxvd.cn/gtcttnyhzu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtincvqimo.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtycmrdvtm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aibaodan.cn/gtdwbheqqt.html

PHP:  filesize("a.txt");
来源：http://hz.jyoumei.cn/gttwqltwcu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtngvkhmyo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtcfmmksle.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtlmokoizf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtrbelrrfk.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtpxklrtbo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtimhgrimo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtepdwnwzm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtujlpemto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gtdvwamddx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gteknhpurg.html

TS:   path.extname("a.txt")
来源：http://hz.yvedp.cn/gtjbtjnoig.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtmycdqpwg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.mhx1999.top/gtvfrhrscq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtinmjjorw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtadjuhyme.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtaxuufhgl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtxvbilekf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtexjcisxv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gteumfkbmq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtkjdlitfv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtzrbfvhnv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gttypfdzcr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gthohkwnhu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtzazdwgln.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtihtgtlhb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cheryme.top/gtxdeyylrt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtrzqnkaaw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtujnkdpyj.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtuaepmvuo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtamwqdtyj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtixarjhij.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtjmlpnali.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gtlwnptrsn.html

================================================================================
来源：http://hz.yuxming.cn/gtrjeavgof.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtlxckktyt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtitjqwjzu.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtguqtznbt.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtoswnrwwt.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtrcpmcqqc.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtsuzettsw.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtzhkembmy.html

Java: class User {}
来源：http://hz.redwolf501.top/gtbxwngnnk.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtmgutwvcd.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gtetjaefkh.html

C#:   class User {}
来源：http://hz.tanke756.top/gtrvfofkab.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtveqykzpb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yonumen.top/gtivrblysb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtzyusvvnf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtctfhaxsa.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtrcaysera.html

Java: User(String name) { this.name = name; }
来源：http://hz.316326.xyz/gtnzbflscx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtgxsxykzi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtmbiseqbx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258.top/gttqtmmazc.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gthhzdytzb.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gteoiblczs.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gthbhfzqeb.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtrlzuulin.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtnrpvcjza.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtangolciv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtgovhcpgr.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtkwcbxcen.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gthqyunnjt.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gthhdixjov.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gttrikdyko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gttxihhotq.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtffpbockz.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtoharinfr.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtrqindubu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtrnuhctzh.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtlttygvjd.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtyaigvdqe.html

[G05] 继承
来源：http://hz.sweek.top/gttupytpvy.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtgswuhjco.html

PHP:  class Admin extends User {}
来源：http://hz.guannengcc.top/gtjooayhfz.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtbjxwzgdp.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtwifxuqmo.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtqtprskqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtumsmxdoz.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gtligdrdcm.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtnlqiyfwk.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gtnxecjdpc.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtdpesefld.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtjrzaqdnx.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtkylvxtao.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtnkqcvdmv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gthqcqdtkx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtsuzrxovo.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtfwokammo.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnqzz.top/gtrtrxscpd.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtbqoukvps.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtjjouxcbk.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtgvpnadsc.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtfkuwofbe.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtwmdpqeeo.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtqjzbverd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtaedflfud.html

Ruby: super
来源：http://hz.yonumen.top/gtfpguhmtj.html

C#:   base.Greet();
来源：http://hz.xingfuxueyuan.xyz/gtbqwbdktk.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtrdmyobed.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtdgkkwjmn.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtkczhbrnu.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtvquswldm.html

TS:   static f(): void {}
来源：http://hz.xingfuxueyuan.xyz/gtqxkeswkf.html

Java: static void f() {}
来源：http://hz.hysaishi.cn/gtxuweubrl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.birdmap.top/gtvchprsem.html

Ruby: def self.f; end
来源：http://hz.hnqzz.top/gtiaksenjz.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtnhiwzoul.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtfzrsfnyr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtavqxpsmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtxxyvbkqu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtainfqiin.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtfrfgzwam.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtcrrhjmvv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xinyue.icu/gtdvkpqisf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtmpgcusql.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenlongwang.top/gtagivoouk.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtnbrrvwfi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtilxdhhzx.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtskdftybh.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtnmqqivye.html

TS:   public / protected / private
来源：http://hz.cqqwz.cn/gtrfroyeet.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtdiisbrcg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtbcznewwq.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gtamkzusei.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtibvvqymu.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtwzztjdyf.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gtvdfzviaf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtrwsvsxmo.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gteltmuovp.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtxyiqofip.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtealcrsbi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtdljdcysl.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtkcpsrkqv.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtuusdaqge.html

[G12] 对象转字符串
来源：http://hz.nanxuanxn.top/gtcwgezkkh.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gturqfnyqg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtcqwicqvc.html

JS:   toString() { return this.name; }
来源：http://hz.zycfv.cn/gtzzzxpnpi.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtfanhjisw.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtibgpfcze.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtaypaveku.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtswxdgszg.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gthrlanxwq.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtsglxeokp.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtseyzklnk.html

PHP:  $u instanceof User
来源：http://hz.zdqjudy.top/gtzfukalrs.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtoxlawiwu.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtoipnzjcp.html

Java: u instanceof User
来源：http://hz.jinqigufen.top/gtzcxuaakp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtdofgrkzx.html

Ruby: u.is_a?(User)
来源：http://hz.aibaodan.cn/gtsgxcyhmy.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtnucusqru.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtxjskshgs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtmhqeojsq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtxfnbemns.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtpbtnlshd.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gtizkrkxdq.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtxxtevket.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtlzrdhiom.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtwecnsmxp.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtcoracclm.html

[G15] 枚举
来源：http://hz.yj20258.top/gtywbwsbeo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtwcinrjkw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gttkudzvkr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtajxmskce.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtzhrubhcg.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtcnibsuyq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtxeodcxmu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gtwwbujzou.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtnhfmxhfg.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtuuthfqco.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtmcmpfgqe.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtjogdtbfs.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtrhnzfciw.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtgacuvszx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtjrnkqpie.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtxfmjrbse.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gtvfkudmwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtoyumybgs.html

================================================================================
来源：http://hz.haohaochexian.top/gttaoewwoq.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtwekzsyty.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrcblwlhx.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtedjidvzp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtnntipqlq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sxryk.cn/gtpazpohgc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtvattbxtz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtawvfrald.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.vqdsnc.cn/gtsheqwvyk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtfigscovs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtasdqxatx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gtofjorkuy.html

[H02] finally / ensure 收尾
来源：http://hz.cdnleiting.top/gtvuyqxpgx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenjidiqi.icu/gtgarlrnrh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtdcclkmqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtlszxsoxe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtxiqcysvr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtzsszbqlf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtruztexix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtddxhgaff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gthsuhttaw.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gtiyddguru.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtzlstlvuw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtyieooeab.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmernmoae.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gttfayruxm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtarqeixrk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtfbekaxbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtdngfoyot.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtmaeqfiky.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gthaoioybb.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtsqlyyyle.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.c1oappe.top/gtncrjtqfa.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtfdzymydy.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtrxgsopdi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtxhcvzgwg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.kuanghao11.cn/gtimebvtrz.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gtkdsgbxjk.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtelywpdms.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtltuwtlsl.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtnyveqzil.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtjqvcaywe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtgotpwlpo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtjpxddown.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtyupeugrk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cucudq.cn/gtggcznrgw.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtmnkwgooq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gttvpiiles.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gthautsmmm.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gthemyzfra.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtmvgjajaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtcgufdcnn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtkajaqbja.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ivvv.top/gtgmyfwbur.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtmsmlykxi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtjghyaujp.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gteynjskuh.html

[H07] 断言
来源：http://hz.yvedp.cn/gtxnjatefr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtvtrfhktk.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtkpidowfe.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtlpygzswy.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtuufwsnrw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtwthxcgff.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.redwolf501.top/gtsmwnmlmd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangshuangyany.cn/gtdkbucdhp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zycfv.cn/gtzqrbomwo.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtvrgkxefk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtirrrivig.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sxryk.cn/gthfrqzwim.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtayjdeppd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtepuhctqw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtizinjiec.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtbdduuspr.html

Ruby: e.message;  e.backtrace
来源：http://hz.vqdsnc.cn/gttzrtrcwk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtbawfwcpm.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gtvnrkkrho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtgjjsplhq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtrigkezeg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxinkj.top/gtlglrbzxf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtljjwftwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtolfvyxvw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtzdqmcfcv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtdwwgaxuf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtfmeucmtd.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtnxbrzbwi.html


<!-- 参考信息 -->