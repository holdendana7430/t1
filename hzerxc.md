代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.bjfxy.top/gtbmypwydv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtivqjgyip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtgnqquqtr.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtuqbodcao.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtuhghbyhp.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtaprwsbuk.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigufen.top/gtvgwygaza.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtirjvvzwt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtiqwomgbv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtmclddpko.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtzmruzqis.html

Go:   os.Remove("a.txt")
来源：http://hz.0kj1m.cn/gtinmevkbk.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gturmstqcb.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtmcdelvdg.html

[F07] 创建目录（含多级）
来源：http://hz.zhoulong.xyz/gtfvlqfxuj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtlpyxkkbs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jlsjyb.cn/gtulfdevrw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtepmjkyxe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtmwwpjuzk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtlhyaguqk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtbluixuix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258.top/gtgcjuguin.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangtech.top/gtcaotlucc.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtsowqsqff.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtdhzektzz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shzxlz.cn/gtymgazien.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtgnlpnudb.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtiqmmnzrh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtbtydtpmd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtrxzbsptv.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtzswebkss.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xinyue.icu/gtiysduisw.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtigfdqxtf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtnskblyrh.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtrnlpvpbf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtgphgxthi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtjuhjsnrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtpimuldrv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gtkfxqfbuv.html

Ruby: File.size("a.txt")
来源：http://hz.bjfxy.top/gtsjgqnbur.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtoppibqfg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtxdaekqdt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gteuphuzca.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtcfycucvi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtbgzaujjn.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtquxazpkm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gtxtnwdvmh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtcpzrgone.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtlfzqvafx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gttrxfaoae.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtsepkbvfy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtteqmrsiu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gogol.net.cn/gtzamrtoln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtjtqlspei.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtimfctpel.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtlxslzgsc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gogol.net.cn/gthaqundxr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtmwftksdi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtwxrwommb.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtvmiebmrj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.svipenyu.cn/gtkvpynyrw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sweek.top/gteyqgsgmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gtkjhwbbrv.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtegcacfdw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gthqcgggya.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtuliorigg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtceqlqxsz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtgautnjoe.html

================================================================================
来源：http://hz.meibo888.top/gtmaeopran.html

G. 面向对象
来源：http://hz.jqgufenzy.top/gtagdzprzu.html

================================================================================
来源：http://hz.tianlin.xyz/gtsdagzgnu.html

[G01] 定义类
来源：http://hz.cashguo.top/gtqjyhhywg.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtwpiwfyqz.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtfexkjwap.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gtyipklyjd.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtbxudqxol.html

Java: class User {}
来源：http://hz.jianghu66.top/gthmaufyqo.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gtutkhspdf.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtqkxiizvd.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtclfwgxrg.html

[G02] 构造函数
来源：http://hz.iojbl.cn/gtovizieoe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtkvzyldyf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtavdwkdph.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtsadychmx.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gtbdoiwylj.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtoxrhrhpt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtwhvlseoq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtacxfbwhu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gtsbzsikux.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtjtestnip.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtwddtivsf.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtpdygidbe.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtlfjcowev.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gttezxleje.html

Java: private String name;
来源：http://hz.guannengcc.top/gtrobeuwkn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtznzqdhim.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtktoikaao.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtuyqgvipm.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtltpdqeos.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtfiiqqadq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtmspnrqkq.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtjiqqukev.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtnukacdxd.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtiviuhrkq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtaaugltys.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtzribqwhx.html

C#:   public string Greet() => Name;
来源：http://hz.fzhhl.top/gtcgbwaclu.html

[G05] 继承
来源：http://hz.shuidangran.top/gtcrosinky.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtldaarcut.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtjsuxrqao.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtfahupkrk.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtsxnilmgk.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtqivebhok.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhiwuduotai.top/gtkpcqybtg.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtmgahrtsf.html

C#:   class Admin : User {}
来源：http://hz.redwolf501.top/gtfpcomzws.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtdvbqnuna.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtxqauykco.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtxxrsypsg.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gttiyripbc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtgftpiwhx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtuufuvear.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtydjddyzm.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtibzfzqos.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtisnrsrfr.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtuiekwyyu.html

Py:   super().greet()
来源：http://hz.fengsongda.top/gtdpoveadk.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtinwbwugy.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gteqfbmmha.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtnjjzadyx.html

Java: super.greet();
来源：http://hz.jianghu66.top/gtvcrlqkof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtvmombgbt.html

Ruby: super
来源：http://hz.birdmap.top/gtevgstvvo.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtgwrzvtsu.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtmrzbcinb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtfdnlfkgf.html

PHP:  public static function f() {}
来源：http://hz.hammf.cn/gtlpbopsbt.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtpqmsbwax.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtdvevovyg.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtosgkjokq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtzkuqbjci.html

Ruby: def self.f; end
来源：http://hz.yuxming.cn/gtdmzmkuto.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtomiehpaj.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtetrdxzmn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cucudq.cn/gthtysgfuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuxming.cn/gtupztbkzd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtvqudvxvy.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtgfhqihsk.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtrepoimpu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gttyxwnres.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtjccllykr.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtgjhnmrim.html

[G10] 访问控制
来源：http://hz.havefunace.top/gtzerfcluf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtjohxaxcg.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gtrpjuphsj.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtrvuqjlxr.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtpsbosgdg.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtglowzgsa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinghuilouyu.cn/gtfjvmwdvr.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtlbfkrlvd.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtovpewwyv.html

[G11] getter / setter
来源：http://hz.shuidangran.top/gtjsepgcch.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtsmozkgwm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gtlwxchlvi.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gteizldbhf.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtpjnxycrk.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gttployydd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtgpemoixb.html

Ruby: attr_accessor :name
来源：http://hz.vqdsnc.cn/gtncqrbsua.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtdsjgphof.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtxoaqeygj.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtmjshuria.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtbojzzkbv.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtopapjnjt.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtjsruuqiw.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gttbtawdoz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gttwvxjmdz.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gtxoswiiwh.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtzlnqgsph.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtskqxaina.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gtzpzizxpc.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtzhghccgb.html

JS:   u instanceof User
来源：http://hz.guowangkeji.top/gtuqofqpsf.html

TS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtoxziktyh.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtypiipfjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghu66.top/gtpbdnzcfl.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtubwmiqld.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtcpepkyom.html

[G14] 数据类 / record
来源：http://hz.quarkkingdee.top/gtqnbwiqtd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtimvmohvt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtbeeuesal.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtsurmpqfz.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtkqblewko.html

Java: record User(String name, int age) {}
来源：http://hz.yj202588.top/gtqmcmranq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtifkaaxqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fengsongda.top/gtlnbnqkjf.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gtsrhzbpfp.html

[G15] 枚举
来源：http://hz.dashuyun.cn/gtxkclhojd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtmxoyhevr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtukttgjqj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtcquyhpjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtddoizubi.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtcqjyncnb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daria6918.cn/gtkacgjqow.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gthphljzgb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtrcvdrxkg.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gtowjkinmr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.feifeiyinyue.top/gtwxfccilv.html

PHP:  get_object_vars($obj);
来源：http://hz.yuxming.cn/gtskyisrsc.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gthkfxfeff.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtcjnzpmho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtneuznvgq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtyoddgcwv.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtcnvzfewd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtkcxqusgl.html

================================================================================
来源：http://hz.meibo888.top/gtxsmcprwu.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtpysuarsg.html

================================================================================
来源：http://hz.gzhubu.top/gtzppkhylk.html

[H01] try / catch 基础
来源：http://hz.zhijiandao.cn/gtzecdpdxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtypgovzck.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtmzefwwcp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gteuecworq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtvedzeucq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtjvaqkxcp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydjk.org.cn/gtqhjrbudj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gttcndjqer.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gtzbdafndc.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtpcojmmub.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtxidsmxhz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtmkwwelzi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtakudzfyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtbhkmbvsk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtgeixmwae.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtcwiegkfb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzhubu.top/gthiqwoyio.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtbrusdfpm.html

[H03] 主动抛出异常
来源：http://hz.andypj.xyz/gtbsefdwrv.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtipvgjlog.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.havefunace.top/gttezkvvvn.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gttdfgqcxs.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gteroheama.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtjgtfmzkg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtyigmlkmo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtnmsfxuhz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtiggtaxlw.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtrujewicc.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtwbajjgvi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258888.top/gtclkahxqs.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtxbtpbmcp.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtlcvqgxkc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtmpthbrvh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtsoefzirs.html

Ruby: class MyError < StandardError; end
来源：http://hz.shzxlz.cn/gtvevxbnuz.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtmeesumer.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtctfzyvzw.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtfnqgkkcm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtpqlqgkly.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtzchodrco.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtuygatdng.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtnumxmfrj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtevjsgpdh.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gttyxlagiz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aibaodan.cn/gteoomtrpn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtqcmtccbk.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtfvcaxpfo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtbbmuqnxg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtzsckxtzx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtbqhjrdrn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gtemdqbeje.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtdalqlrqq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gtfdnybcup.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtufbcmrdn.html

[H07] 断言
来源：http://hz.tian-w.cn/gtmgsnbiec.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtilcqmqvg.html

PHP:  assert($x > 0);
来源：http://hz.sysykeji.top/gtosnrtojb.html

JS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gttyyrmswv.html

TS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtwreurtdu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtadtrrxko.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtpvnjilov.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gthpcelopr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gttoegrayh.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtmicnxlxb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtekwttdzu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gthdjypfsb.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtwekbkmty.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtnhatnugo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtsdcvzimp.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtazofzacd.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gtzzbmkwgz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtxxuczrov.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtshafipdt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gtuvrzzikc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtqfqvhtex.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtxjccqiur.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtxyzfcpqi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtervntkcp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtenwuenai.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtgbsoipyn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gtltieadpt.html

[H10] 资源自动释放
来源：http://hz.yj20258888.top/gtyenipoab.html


<!-- 参考信息 -->