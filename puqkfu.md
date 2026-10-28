代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtdxvdrgzq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtpodcycut.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtkwsyiakd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtskqjzicx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtofmbzkbx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gttcuaebrm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtaacbaqbb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gttvojopho.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtcvxauzct.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtycfamxyg.html

Py:   os.remove("a.txt")
来源：http://hz.nanxuanxn.top/gtaabwsawk.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtiwfyrpzf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtrasfskgj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtaqpweaji.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtynvoprvi.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtgjiodejd.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtsoodtwyb.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtclmxivbd.html

[F07] 创建目录（含多级）
来源：http://hz.jyoumei.cn/gtaobvidcc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtqzwoygzx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtuxyahoib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtcelmuepm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtdwmcchdk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtmioaupdp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtisjsjiro.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtrtqhgxhq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtxvwfkply.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtzpfvvqri.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtbwumizlu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xingfuxueyuan.xyz/gtroayklvb.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtstrhjnee.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtlndrqdnh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtlgguoemv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtikcjwsfg.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtlaiwdgge.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cashguo.top/gtgeulljgw.html

[F09] 获取文件大小
来源：http://hz.tanke756.top/gtdtpvwovc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtfdmbdnau.html

PHP:  filesize("a.txt");
来源：http://hz.52xcode.cn/gtqztoddww.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtyeyfaxts.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtvcscwqfa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gthuiuhssp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtujotknqj.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtzlpbecsl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtwsfqxjiu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtufnqjitn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtjcfnmxab.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtnvvskkif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtlmnicsnm.html

TS:   path.extname("a.txt")
来源：http://hz.kuanghao11.cn/gtvemtqurb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtddjwhtce.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtdbgpcdxd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtyilomekm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gturhojonf.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtrtiabujo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtxuzkrbps.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sxryk.cn/gtxyoawzdr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtqrrblhuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtubgbmlos.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtetqtnyvi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtvwajdqos.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtfajombjo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daria6918.cn/gtaeccrapf.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtvcvpblgi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtnlupgvhj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtmqozzlwu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtrejxeqtr.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtophtvaat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtucaaciou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtwimtgaqb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtmacyhbpw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.smart0.xyz/gtiqrfkbfn.html

================================================================================
来源：http://hz.yj20258888.top/gtukaogfqk.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gtfnndwutu.html

================================================================================
来源：http://hz.ybcxt.top/gtpaqptmfy.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtnyamflvy.html

Py:   class User: pass
来源：http://hz.sweek.top/gtqerfufsp.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtedfierun.html

JS:   class User {}
来源：http://hz.316326.xyz/gtgcskajsi.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtcznddhxm.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtycqclpya.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtobbzrqzb.html

Ruby: class User; end
来源：http://hz.xingfuxueyuan.xyz/gtumcxbeij.html

C#:   class User {}
来源：http://hz.fzhhl.top/gtfvhmtwkn.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtdsnqetoi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gthfahdsdk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtgtrwyjnq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtblzjzdmz.html

TS:   constructor(public name: string) {}
来源：http://hz.tianlin.xyz/gtyazzotmt.html

Java: User(String name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtohhzifbv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtqkgnoxlj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtskyyfamh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtezuzcwwh.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtjacmyuuv.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtbphzjdrz.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtwmybrmib.html

JS:   this.name = "x";
来源：http://hz.hfpthk.cn/gtkcxlkmae.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtltfeapcu.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gtbpdfrzrb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtsyoeohxb.html

Ruby: @name = "x"
来源：http://hz.pengpengdd.cyou/gtkmfdrrib.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtcxrccypp.html

[G04] 定义方法
来源：http://hz.hongshengwenyu.top/gtgssplxgm.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtuqapywcb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtjeigubzy.html

JS:   greet() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtiwdyeqdt.html

TS:   greet(): string { return this.name; }
来源：http://hz.xylfe.cn/gtguackfxt.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtgskumfkp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtwcslcwbe.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtsblumnha.html

C#:   public string Greet() => Name;
来源：http://hz.zhengqikj.top/gtmgzuidfy.html

[G05] 继承
来源：http://hz.birdmap.top/gtnrmykmdb.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtqhsisaic.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtwsishska.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gthmeuzava.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtgacheucw.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtasejdsdq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhixingplan.top/gtoorqtdnv.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gttrxtzcxt.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtctmifzzw.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtdgpnismj.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtzvsifxsf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtagjembft.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtfymqjkpd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtwmvbdmqe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtddjlshsa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtfzkxpoio.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtblhbhvza.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtdkzknljm.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gtxhqfgpkf.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtabmazbbl.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtiavstprv.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtdgztyhos.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtsoysugre.html

Java: super.greet();
来源：http://hz.quarkkingdee.top/gtiiogwkgi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtgeczroxh.html

Ruby: super
来源：http://hz.yongpay.top/gtnnipehcr.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtdbynsatc.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtxxyzajkn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtaxnyinnv.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtnbvyfpsa.html

JS:   static f() {}
来源：http://hz.quarkkingdee.top/gtcreaqbfd.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtuauhyhrh.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtqhqrduio.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gtrdokzdhh.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtxkmxgvgh.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gtlalskyyk.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtxzfcqbgb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtwkeapzif.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtbblklylm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtuhlpvhsa.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gttcgdnztl.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtuypoayqh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtyrmjrrbl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtpxbqqhlc.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtxeosvxri.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gthpzpunfe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtgfoilchf.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtwencerys.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtxlhejuvn.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtgnaaezee.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtvfjorqna.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gtncsctemu.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtkrxgnfbi.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtpilvxsjn.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtyydwvkzb.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gttsxbjhoa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtvcttvesx.html

JS:   get name() { return this._name; }
来源：http://hz.tianlin.xyz/gtubacwusd.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtyokstlrn.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtcoajjqsi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtwfbagubo.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtiuayoxex.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtfotwflzu.html

[G12] 对象转字符串
来源：http://hz.andypj.xyz/gtcvxsrmhm.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258888.top/gtqapqvkvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtjagdlmvl.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtllrgmxpg.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtcddglzcc.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtpndphjzo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtsvlarwny.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtyavrtmwf.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtqxmicoog.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtvrnpsrum.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtaxeipbvt.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtmwnaxuwr.html

JS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtrrpkekoy.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtgteqfqzo.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtannwandb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtwgjyvfxr.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtzbtozsgb.html

C#:   u is User
来源：http://hz.sxryk.cn/gtdfzvrukb.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtacjlllkr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtgckutkrc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gtnvtfjgyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtyvpplluv.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gtbivsjpab.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtnfiprnvj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gtmojpsamg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtyivpwzhf.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtyrhfazdd.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gthunosxrk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gthhkpfhap.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtxdbgyjak.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtjmtnnogm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtkdduxavy.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtzfmymtoo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtsljxipss.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtkzdozlwk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtsxnsgvqz.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtvntgzvpu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtjkgxzewr.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtjkuepdal.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtfkhndlim.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtlbgxghxy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtaqtasieo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtfycbbnua.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtlhxjbyil.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtuabqergm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgdulpzku.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtomdbmxgr.html

================================================================================
来源：http://hz.hnqzz.top/gtbkitgdlo.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtrtckhyih.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtwcrveueo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtmjkldohl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtbhvzwoon.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtmsidqhbs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hfpthk.cn/gteqpdkohj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtwnhrdsmq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yanxiufei.cn/gtxxuwqgzi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gteeitbyzq.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigfzy.top/gtxkvafzwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtdpwtvdbd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtndgcpfee.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtsbfroiaf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtsskbgqlm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gthatfumao.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtldutnxvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtffkfgtio.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtvecqmqug.html

[H03] 主动抛出异常
来源：http://hz.jqgufenzy.top/gtzecwslgp.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gtbzvewtmz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtmsvphadz.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtfhmnznwj.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtjtxcremr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtbazkjcoj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtbmznazji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtgldimzxb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtafqrwlhz.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtgzllhkwm.html

Py:   class MyError(Exception): pass
来源：http://hz.yuxming.cn/gtxckjqpry.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtmoklzrwh.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtzeidpryc.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtkhzusujb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtwddcrmmo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtqcoyqxnt.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtpdgkkykt.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigufen.top/gtyvymjtff.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gttcpmjncx.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtiiraehwq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtzdsjcxfy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gttrpqlumu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtvzrvsagp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gtofbcskbd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtmaezoxfl.html

Ruby: rescue ArgumentError => e
来源：http://hz.mhx1999.top/gtbpneybeq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtdrfvzkzr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtkiqjwozo.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtlvvbddsv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.0kj1m.cn/gtzzoxarth.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtilpaydtr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtssagtdro.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtpadafbsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gtgffokbrn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtvqniyzws.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtixhqvrjm.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtdurtnumy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtsamfnpjd.html

PHP:  assert($x > 0);
来源：http://hz.daxiang520.top/gtpxisfpyl.html

JS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtnewpdifd.html

TS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtfjjasdmn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.c1oappe.top/gtqfjnydah.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtxesjpsic.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtlhbywiei.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtmqgchouk.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtftvdjvat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhaomingkeji.xyz/gtbdloiary.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtguflyvbg.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtcdpqdxyx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtndfntneg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtcecragcc.html

Go:   err.Error()
来源：http://hz.guowangkeji.top/gttubuzfcg.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtbjtgxrgs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xingfuxueyuan.xyz/gtavhlzzax.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtqgcwojqv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtlbxtqchh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guowangkeji.top/gtpnimkhym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtrvtgjfik.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cashguo.top/gtgaefjqli.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtiaymvrhg.html


<!-- 参考信息 -->