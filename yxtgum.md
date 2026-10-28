代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtriilfzei.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtoimordpe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shzxlz.cn/gtkghivslq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gtxczakrzk.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtmhhxuedq.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtpnkgtxdh.html

Py:   os.remove("a.txt")
来源：http://hz.snrcjt.cn/gtwjegvvnp.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gteqzruzig.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtjtowgazl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtsaszpgly.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtxtqqqrll.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtlsbdwomy.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtkwqftrya.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtmzqkybtk.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gtkujyaudx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtkizecsmu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tian-w.cn/gtihbgrsuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtiaiheglq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gthjnqfffa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtuxvekcro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtimmzmnxp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtkgrxsekl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtqqfvvccp.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtbbiultze.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shangyingyoupin.top/gtauwnefcn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtkbunekco.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtgnvkpiuj.html

TS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gthiuuyfcf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gthdejeohk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtonfstuxh.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtqjpzpwxx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtxoscanto.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtqdyorfac.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuanzx.com/gtatclwcbb.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gttqeaajnv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtcbicgmwv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtwfcmoqnw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtynkmcian.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtdinfnhnk.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtgkpbqaxe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cdnleiting.top/gtolnqclon.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtrexkdddt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtmuzdoepw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gthigsoenu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtyofarlap.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtyqdzzbwp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtxlvpizxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtjtzjitpu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtuqqkvvkf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtngioghgz.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtpogdyylh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtyggcnihx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daxiang520.top/gtwepcehfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtfipeofjp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtqildlloh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtpwfabsev.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gtuyzewtoc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtkcctftpz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtvynsmqyf.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gthrzleqpa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.mhx1999.top/gtofbwtova.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtfckqrhzu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtiszplhmq.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtmxtozxgd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtbvconbmx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtlaolxeaz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj202588.top/gtubgxndld.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtxhjvzybb.html

================================================================================
来源：http://hz.yueranfly.top/gtfxisvgbv.html

G. 面向对象
来源：http://hz.wangdashe.top/gtttedwmmc.html

================================================================================
来源：http://hz.iojbl.cn/gtpvfvshgd.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtumjrzzwd.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtpzhnxpcg.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtqprvskuh.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtodargvfc.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtdjziiezj.html

Java: class User {}
来源：http://hz.wangdashe.top/gteibqxjvw.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gthwvkoqnc.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtjpvwszne.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtpeskmffk.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtggrhxqjo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cashguo.top/gtwwtfpkks.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtmrahhewh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtvhezmbpw.html

TS:   constructor(public name: string) {}
来源：http://hz.cqqwz.cn/gtvzcvzcic.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtsjcpdkvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ywan-chungtsiang.top/gttiujxoho.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtericfwje.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtknyojazu.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtncnupfap.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gttxdsthdy.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtqrkykvfj.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtmfrkebfi.html

TS:   name: string = "x";
来源：http://hz.sufxvd.cn/gtczmlsffy.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtpevqfliu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtxlveinow.html

Ruby: @name = "x"
来源：http://hz.cashguo.top/gtmtxoecdq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gogol.net.cn/gtchirobke.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtleiyguur.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtnbhllztt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtrlqwhxax.html

JS:   greet() { return this.name; }
来源：http://hz.nanxuanxn.top/gtybalusoh.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtvknnpxww.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtmjammbsj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.havefunace.top/gtwwjkidvt.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gteucnyrsf.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtsxmfhsao.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtaiiermws.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtxopzslox.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtcsnazxsi.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtqphxyyyq.html

TS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gthtlnekaf.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtxwiqbglf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtnhwegyvo.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtarckodge.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gtcuswtlhc.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gtbobjcxmt.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtwuqqxrew.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtbywmwtyj.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtnwdlwoto.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtpxbgajem.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtkorxirwm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.snrcjt.cn/gtbvivndsl.html

Ruby: def greet; "admin"; end
来源：http://hz.0kj1m.cn/gteepjseaf.html

C#:   public override string Greet() => "admin";
来源：http://hz.52xcode.cn/gttvnczubh.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gtamghosyr.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtnsrvpbcl.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtuidhbuwr.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtuaqgjhxh.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtjklqtdsy.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtkockpbpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtsjqlefuv.html

Ruby: super
来源：http://hz.yangfankeji.com/gtfyzeqpur.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gtauwskyhq.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gteeetpjqz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtmxiinaxg.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtdiwubedz.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtkjwhrbkt.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtjyhymowx.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtgmjeasve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinyuanbaomall.cn/gtangnvhjw.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gtkmslkvga.html

C#:   public static void F() {}
来源：http://hz.jianghu66.top/gtqrjelvez.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtibrvkqgu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtgjinokot.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jianghu66.top/gtfizxjygo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtbdyofbfo.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtssmuoitn.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtjwqeavma.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gtsjtezspk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtgxrzwwzx.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinyuanbaomall.cn/gtiwrnzocj.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gtjfgsotaj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuanzhike.top/gtmwxfdlwq.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gtuftlturf.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtsvsyxywx.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtshyergst.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gtplmlitgu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtkkjkbemf.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtyayyydlz.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtyyjvvkoz.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gthopmblch.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtcicneqfm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtrddwxshh.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtruniquug.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gteiqdpwgm.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtlnwlsqdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtemuevvsl.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtouxazzir.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtdypmbdpk.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gtacrxkjzc.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtyotfycdr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtwqejlwdc.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtelukctog.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtoprrroxp.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtrryejjjh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtycaasbvm.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtzshuwuhc.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtohcalzkn.html

[G13] 判断对象类型
来源：http://hz.dashuyun.cn/gtyudypdgs.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtbnxjcbff.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtdpebggja.html

JS:   u instanceof User
来源：http://hz.havefunace.top/gtlkhznljf.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtfhdxwbat.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtevfgawyl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuanzhike.top/gtbsfbgrmv.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtfoggllxx.html

C#:   u is User
来源：http://hz.yj20258.top/gtqdnsycdp.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtneglcehy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtnaiezmsz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtkghlgpti.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigufen.top/gtbnummved.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtjgmulczu.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gtgwnsxdxa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtxpebiszc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtompojpkj.html

C#:   record User(string Name, int Age);
来源：http://hz.ehwqpu.com/gtuagdlemy.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtaxfauenz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gthtyuabsb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtxoiklhrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtnxjivxfd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtrtipravr.html

Java: enum Color { RED, GREEN }
来源：http://hz.gzhubu.top/gtcseizzdm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gttgxfgzly.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtivmktbsf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtqpiyeayc.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtavdknggn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtereuzcep.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtlwlvjuex.html

JS:   Object.entries(obj)
来源：http://hz.sweek.top/gthqewyydp.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gthmkrggzl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtzajyalvr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnxiangtu.top/gtsmthtomk.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtnkxyfiir.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gticzpgckf.html

================================================================================
来源：http://hz.guowangkeji.top/gtsmzktukm.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtbqopcodp.html

================================================================================
来源：http://hz.haohaochexian.top/gtbknltoii.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtpvrmenaq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtvijmnqof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtjkoaeuoj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gthjtombpg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhongyouzk.top/gthyhpnihz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtexxbujue.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtfpdizvjy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtnbdmfdyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.0kj1m.cn/gtrkxesrsm.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtirrqpify.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtlmbiffne.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtpmxsubci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtktwdeqcd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtepzlifob.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtfxatspna.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtpxmkdeap.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pycfn.com/gtydchgukh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtebrbhywi.html

[H03] 主动抛出异常
来源：http://hz.cheryme.top/gtfuxmsklr.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtvqdokiro.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtctdrtbgw.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtoxcjvske.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtfjcekktg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtrheneyxr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtiayzsltm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtyuhvqekk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtolmcrfjv.html

[H04] 自定义异常类型
来源：http://hz.jianghu66.top/gtnwahqgpt.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtvndpmyti.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtvklyekzw.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtpffaxanl.html

TS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtrfvaenti.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtruxvogbi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gtdbhdobvt.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gtrokdfzpk.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gtlwlscqvm.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtdnnbjuej.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtyeyojzzh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtfvazlsen.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtmapujkah.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtfqrleoob.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuxming.cn/gtvhkayzjn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jyoumei.cn/gtfsjbbqzj.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtbiszmyms.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtobpnfwxr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yonumen.top/gtzljedepi.html

Py:   value = d.get("k") or default
来源：http://hz.ydzc1.top/gtoeyhqgba.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtneekages.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtfswnyons.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtwhopetlk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gtijptrjpa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gteqmpqgzw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtvasfgyhx.html

C#:   obj?.A?.B ?? default
来源：http://hz.fengsongda.top/gtfcmsddap.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtqjxkvrmk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtkniehket.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtmvcouinf.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtmjvfctmk.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtnrgzsing.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtvdphrory.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtgmqgfxuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtshayfmqy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtqydwpabd.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuetiantiany.cn/gtefshjwqr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtyhtaytbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hongshengwenyu.top/gtgvymqgpc.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtapijvgbp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtarhwcgil.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtarbuvxcy.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtcriccjwu.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtdffknqok.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gthxtkirla.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtwwcsshpw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtpxxhuzlr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtzvuznuyn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gthyrguqvv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.bjfxy.top/gteijpfupa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhixingplan.top/gtiklgqntc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gthgcyptxv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.meibo888.top/gtexgdgyou.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtpnnjncad.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtxchmiubv.html


<!-- 参考信息 -->