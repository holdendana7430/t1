代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtajvynrkt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnqzz.top/gtdufnudeq.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtbrcvklgr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gttropyjwu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtnbusjwpw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtpnqaxtfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtbskacyeu.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtuugenzln.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gthxjfqfnx.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtfshvsdxf.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtciozswdk.html

PHP:  unlink("a.txt");
来源：http://hz.gogol.net.cn/gtjfidklhc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtogmcqauo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtfeeeyubp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtladrrbnk.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gttecgeiic.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtbddsfdoj.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gtjsbxnngb.html

[F07] 创建目录（含多级）
来源：http://hz.haohaochexian.top/gtowlactbh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtmzicrzpz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtiigniwwi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtomrlakik.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtexionxol.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gtcoojqlyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtjyfexdtm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtadvbjubr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cdnleiting.top/gtsflgcbjk.html

[F08] 遍历目录
来源：http://hz.havefunace.top/gtcuopeisk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtytzoxtqr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtrgplvnjd.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtpgywzqlb.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtslsrtipw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtmhyalkvw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtxisrijya.html

Ruby: Dir.children("dir")
来源：http://hz.fengsongda.top/gtqkgqglmj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gthihabjfa.html

[F09] 获取文件大小
来源：http://hz.zhijiandao.cn/gtefryzdvi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtexevuleb.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtzruufuyh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtvvtuleyb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtrkcqreaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtctcrcpzv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtvnlufxwt.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtedcyrhay.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtjvkvlzzd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xingfuxueyuan.xyz/gtmacxdqpe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtqwygzlov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtolisrjxu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtdtedkfgy.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gtvtujgzeg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtqbbpqxlb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtfqcxdrch.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtslmmvskd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtvnhwerwf.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gtmopfaqpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gthhbbjszy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtdibrfwoz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtibpcclib.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtqxywgvnx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtkmhcbxic.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gtszonlmmu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtrozvfryk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtqtqpsref.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gtvmukjlfn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtpuuylnaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.316326.xyz/gtdimqfswp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cqqwz.cn/gtdopumryp.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtyhpsobfw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtyymdvjsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtvmlxakzp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tianlin.xyz/gtzgimemoy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtosvajsbw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtoidticql.html

G. 面向对象
来源：http://hz.nwbrower.top/gtqqplnulp.html

================================================================================
来源：http://hz.chenzaomai.com/gtgjrvfstb.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtkbctnhbh.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gtodyqexyf.html

PHP:  class User {}
来源：http://hz.shangyingyoupin.top/gtnbvbxkyv.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtxmymnves.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtiuymvede.html

Java: class User {}
来源：http://hz.yueranfly.top/gtdqsajnpw.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gthteazggo.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtvywnfjzb.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtybzfkvxh.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gttgorqolk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtxvzpmsfz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtnmcfodoj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtexjpghzm.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtwhefgjxl.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gtiiliyegi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtifrmrmrt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtgzoefyas.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtqzsrdarr.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtuopwaigo.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtuysiqvmc.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtmrigzowy.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtpjwvkmek.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtrzafnhdc.html

Java: private String name;
来源：http://hz.meibo888.top/gtftkmsnum.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtsqiphfam.html

Ruby: @name = "x"
来源：http://hz.yuxming.cn/gtcqswsdro.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtcqilgxxn.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtlqalogbr.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gthqnikbpx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtdrovbwmm.html

JS:   greet() { return this.name; }
来源：http://hz.dianchejie.cn/gtgipddtwd.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtnpcosxds.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtlnydwtjp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtqvmguuju.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtsycmpteo.html

C#:   public string Greet() => Name;
来源：http://hz.vqdsnc.cn/gtnutrjevk.html

[G05] 继承
来源：http://hz.yueranfly.top/gtntzlvrfi.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtkvhdyiar.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtqzledarm.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtrckdxlow.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtgvmeddka.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtvbfzlmos.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtvlbzxvcb.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtslsqdjzb.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtbcudnfan.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtafkiuinc.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtmfthuhoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtqglacbvi.html

JS:   greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtvlyxtbfi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtykujkurl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtcuoambep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtgpkmhlsr.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtayzjthyp.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtbtqcznjz.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtpsluwxik.html

Py:   super().greet()
来源：http://hz.yj202588.top/gtrblmziqb.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtxbjlyrgz.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtmylqband.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gterlomjkq.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtztfebfvx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtjhshatbl.html

Ruby: super
来源：http://hz.yanxiufei.cn/gtbcrimcyh.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtaaurfryk.html

[G08] 静态方法与属性
来源：http://hz.daxiang520.top/gthkzttdmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.feifeiyinyue.top/gtuggaaoje.html

PHP:  public static function f() {}
来源：http://hz.yj20258888.top/gtxidkhtqu.html

JS:   static f() {}
来源：http://hz.vqdsnc.cn/gtudjwomtb.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtjigdwbqe.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtusbzlsrr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtbjtdcojd.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtfogsygdq.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtqpvijlzi.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigfzy.top/gtumrfajym.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yvedp.cn/gtqxxhqafs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtoppiggiy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtrbwyxhgn.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtcokmyfft.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtsiyenbwm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtfakjiltj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gturmplspo.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtrkworzlq.html

[G10] 访问控制
来源：http://hz.yonumen.top/gtofsvysqx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtyofkxrec.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtbnuubngi.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtijizecoc.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtwuhstnat.html

Java: public / protected / private / 默认包级
来源：http://hz.jlsjyb.cn/gtnemrdmms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtdaiwqvyf.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtwbtggron.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtczxdeeea.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtjomeckoo.html

Py:   @property 与 @x.setter
来源：http://hz.wangshuangyany.cn/gtholnddgn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gtyvpkrnkz.html

JS:   get name() { return this._name; }
来源：http://hz.ivvv.top/gthibbefnj.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtdnlgdkwr.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtsmsccmzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtdcdvhivo.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gthmpiggfz.html

C#:   public string Name { get; set; }
来源：http://hz.guannengcc.top/gtxxnepjrp.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtprlrwywi.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gtuowonppp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtnmshdzti.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtjcegwyla.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtpbouwyti.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtwpwihwsk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtnbfeaxne.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtcdznlnvp.html

C#:   public override string ToString() => Name;
来源：http://hz.chenzaomai.com/gtvxlggagh.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtupxdnuux.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtdrjgnjpt.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtbeaffprq.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtrfktoagt.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtrkknqove.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtmreliala.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.snrcjt.cn/gtwclblkxu.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gtgwbvuauc.html

C#:   u is User
来源：http://hz.gzhubu.top/gtkbiijfen.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtipcdizbz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtmrvsbydo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cqqwz.cn/gtnbwsjxar.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtvmfvlfqn.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtqlrtgtdh.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtxlvyhmvg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gteasogkjm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtxejbugwq.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtshjifxsx.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtvmlslpzw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtosnzbueu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtyfhgyuuw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtatohhyzz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtwhvzfmph.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtxzgfasvl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gttdjcqfop.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtvpsfygvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtgckwpmew.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtivboqnfg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtmqfepjjq.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtvuxzmlzp.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtgaoccuya.html

TS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gttfhdvsah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtabixvieo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gttmbtsmgw.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gtopvhzwdc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtozwcsoar.html

================================================================================
来源：http://hz.yueranfly.top/gtzptywkbk.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtmdvzsyhf.html

================================================================================
来源：http://hz.mhx1999.top/gttojxvpho.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtopqazptb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258888.top/gtmqonnddx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtzpkthqrd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtpoothzqf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtqeaxybsw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gteilouycj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtdhszsxrz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtpnjbusrj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtgfwrmjvc.html

[H02] finally / ensure 收尾
来源：http://hz.pengpengdd.cyou/gtxthjoibq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yanxiufei.cn/gtlffuofjs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtiflqkqfu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtwkxtolnk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtbepgrawt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gteadwthrh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gttziiendp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gtwntqevfc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gtqfysfrcb.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtltdwvccx.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtwqvsulzq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtbzbhvrir.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtjfyijvdl.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gttesbqcfb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtftirshdk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gttvkybnpy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gtwjnuqiwu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtfmutdvhd.html

[H04] 自定义异常类型
来源：http://hz.guowangkeji.top/gtwfyhjsds.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtbfdifjpl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtqbgkzmpg.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtkxivjtrd.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtanrqberq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtujhtooet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtswfyagyo.html

Ruby: class MyError < StandardError; end
来源：http://hz.mhx1999.top/gtqmzbhyfd.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtxwnklwmq.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtvnnttkhf.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtzfsjpwka.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtynggzxyg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtxdqqfois.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtggrigzqe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtcmplpetb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtsbcgsrkr.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtkaywbdap.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtffbsxhej.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258.top/gtnxumxkhb.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtewiafhqe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gticdlmdph.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtuogrimas.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtullwzdar.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtyvkjrkgx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtcgwtxxxs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtvkpivbyx.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtjwsccfft.html

[H07] 断言
来源：http://hz.tian-w.cn/gtsgauouhr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtwuoktjvs.html

PHP:  assert($x > 0);
来源：http://hz.vqdsnc.cn/gtcxrcvcnk.html

JS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtyyzddfls.html

TS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtzxzdxchj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtzxkxgehz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtxtytzcnz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtmbatglzf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtoxcxhysj.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtdwomxuae.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtehpmfsqn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtnyukpvrc.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtovexoqcz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtezhvftjw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtvzkwhsfv.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtlqsqvgiq.html

Ruby: e.message;  e.backtrace
来源：http://hz.haohaochexian.top/gttqacsrgt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtbrqzefnp.html

[H09] 带错误码的异常
来源：http://hz.jqgfzy.top/gtwpkeebpt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtcirrbfbb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtkstnomcp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258.top/gtsfdyflpb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtmcoegtdq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtsllwhgts.html


<!-- 参考信息 -->