代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtibhzlspi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gtejnhasrh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtqrdfitwd.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtenbokajm.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtimeuofwu.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtjczqdfsp.html

[F07] 创建目录（含多级）
来源：http://hz.shangyingyoupin.top/gtwseirjzc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtgtaszwyt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtvntizgbp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtwzafvhrt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gthpgpppqk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daxiang520.top/gtxggjgtwd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtnbukuikk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtjhwsgies.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtpkjjeptb.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtswarjqec.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtzdemjxhv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtkddpjpxe.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtcptgguky.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtjsyuzwtl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtwojjqiuh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinghuilouyu.cn/gttdclamvf.html

Ruby: Dir.children("dir")
来源：http://hz.zhaomingkeji.xyz/gtbgsypulx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtnsxzimfk.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gtbmbthuug.html

Py:   os.path.getsize("a.txt")
来源：http://hz.haohaochexian.top/gtjunxtdor.html

PHP:  filesize("a.txt");
来源：http://hz.gotoacloud.top/gtgtoqxzhu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtduflhabc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtopwbkmba.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtkxsdwwgn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gthecwigdi.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtmnyfmedy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gttkpyiytp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gtxkuxlkic.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtethohtfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.haohaochexian.top/gtzjridagw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtoohnccco.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtruktevle.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ybcxt.top/gtxkmztzqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtvvwhkqha.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtxtegcypy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gtsvzqnjzr.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtntcosskl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtahluwfda.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtxlxicdpg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtydmenntk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtqnhjvrkn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangshuangyany.cn/gteedlexsa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gterkrgsnc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtovqphudh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtdwdvpwlg.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtaumkqoxn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dianchejie.cn/gtmgqcvrag.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtsrxtfzmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gtujabeklk.html

TS:   // 同上
来源：http://hz.yueranfly.top/gtntytibdc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtlnuodkog.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtpdneykes.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gthaoymack.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtynkkejgo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmgsxijwu.html

G. 面向对象
来源：http://hz.ybcxt.top/gtusfbrxzc.html

================================================================================
来源：http://hz.dianchejie.cn/gtahngygcm.html

[G01] 定义类
来源：http://hz.jiagoushi.top/gtozbvnqnx.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gtulpbqoqm.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtnsdhimyb.html

JS:   class User {}
来源：http://hz.shanyushiyangtech.top/gtoocfjfly.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtnivqrjzf.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtrrcmkeez.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gthmycemjk.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtgkcpyxwm.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gtefbsiwxo.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtlutkyaod.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtmhekdbav.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.kuanghao11.cn/gtdgupjdsv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtleeoibde.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtgkktevlh.html

Java: User(String name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtphfdouwa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtxnlmmpja.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtsssvhctg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtdaiykkgb.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtzrzobczf.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtxcketnvc.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtoqqgkauj.html

JS:   this.name = "x";
来源：http://hz.zdqjudy.top/gtqbjqnyle.html

TS:   name: string = "x";
来源：http://hz.zhixingplan.top/gtjirmjlif.html

Java: private String name;
来源：http://hz.fzhhl.top/gtjdfpkbju.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtqgansldz.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtrppabmhl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtvrgbwzos.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtyutkfqag.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtwmhbbrcq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtfooclqtx.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtbzvnpszp.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtzpkwvodi.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtejtljrpz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtuegibvjs.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtkldseswm.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtldkcubpo.html

[G05] 继承
来源：http://hz.zycfv.cn/gtjpkrbyzp.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtsztawmqc.html

PHP:  class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gttftonfoa.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gthunrcikr.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtjubwamxs.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtksjevtpp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.feifeiyinyue.top/gtgmahocof.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtkzvitoxd.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtgopideqk.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gthesiraqs.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtpjjqsebq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtfydyeslv.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtritcdlny.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtxkkyughx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtkbwsmxmt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtfpaugonn.html

Ruby: def greet; "admin"; end
来源：http://hz.cheryme.top/gtmcnwrprk.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtnyreawmv.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gtyrckrzpt.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtoweivfca.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtgtyqaxoo.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtoyfvlwdn.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtyqgtftgc.html

Java: super.greet();
来源：http://hz.snrcjt.cn/gtyeglghdm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtwuyvcmhh.html

Ruby: super
来源：http://hz.ybcxt.top/gtcghnzdkf.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtsrijgslj.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtkgppdgbp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtamlqjnhl.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtkggsyvzd.html

JS:   static f() {}
来源：http://hz.hfpthk.cn/gteojykahw.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtgwjrizro.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtelyrayas.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtiibdwsoz.html

Ruby: def self.f; end
来源：http://hz.hnqzz.top/gtjouzokov.html

C#:   public static void F() {}
来源：http://hz.tianlin.xyz/gtyyeqkuqe.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtxoychlpw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jyoumei.cn/gtdlykzlmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtonthvyjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtkrepqmqy.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtrbjvqzxc.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtwdcialyk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.quarkkingdee.top/gtxutvvpgr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gthxhczwuv.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtowphiwix.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtkcryfkbh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhoulong.xyz/gtpjjunccj.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtswqgodux.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtmbngdkbc.html

TS:   public / protected / private
来源：http://hz.ydjk.org.cn/gtpqhyoatq.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtrbzivhkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtqmpmcakr.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtqrthosbn.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtcshtdezi.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtvlzmnzkf.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtrnapqrmt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gttgkfbluy.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtertzblyn.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtsegxqbmp.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gttmemwgcw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtmhecljqs.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtzzqcpmcv.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtgrmqegno.html

[G12] 对象转字符串
来源：http://hz.jianghu66.top/gtyreuubhr.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtsbufnutc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtrejfwjpo.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gthvkbbmvj.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtdcpkngwa.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtoknvukkk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtahtjgynd.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtlzpysiqg.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtmicprhma.html

[G13] 判断对象类型
来源：http://hz.mhx1999.top/gtumrxlhmv.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtljsqocyv.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gtptrxvboq.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gtrxwcemnn.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtcqcwsglr.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtggwytxfh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gthfqhrarj.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtfnefpsxb.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtnficosfq.html

[G14] 数据类 / record
来源：http://hz.redwolf501.top/gtmtsolxct.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtnsyhjdbz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dianchejie.cn/gtevcczvpd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gthdcqmlii.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtvyxdoeuy.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gtnuvtzlzi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gthunnuznp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenlongwang.top/gtmpyzugix.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtlczzbrsy.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtnhfjdftz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtzyrhppxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtjnaemmir.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtovqoeodu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtqgbqdnru.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtewcgbtpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtkzblcwys.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yangfankeji.com/gtmoqpmelg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtpdmtbwpa.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtjmizgdvz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gthpehymwe.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtnynnksrh.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtftxccpgr.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtzntdxkvj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtpiybxjef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtgdoooorq.html

Ruby: obj.instance_variables
来源：http://hz.zhaomingkeji.xyz/gtatbnrayt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gthdavegle.html

================================================================================
来源：http://hz.guannengcc.top/gtqkyeymsi.html

H. 异常与错误处理
来源：http://hz.52xcode.cn/gtfuvghizu.html

================================================================================
来源：http://hz.chenlongwang.top/gtuqcepzdt.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtzyuhgzjg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtbejjcypp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtnnlhdcjt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtbnrzxfrs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtxaotiuxu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtpdorwbhn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtwnrtuxiv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gzhubu.top/gtvwtzmujh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtjgqplcyb.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtpumlvsjc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtdpbchisa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtllofdcew.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtesmvwuao.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtbixnbzan.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtsbqpklni.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gthagbvhed.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtribbebbk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtbipafnbe.html

[H03] 主动抛出异常
来源：http://hz.birdmap.top/gtgyhnjgmi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinyuanbaomall.cn/gtoltbxhzr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtjvtlwwco.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtjfirdchp.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtexdqgtqu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gthozupzhp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pycfn.com/gtvtikykjf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtanalhjtl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtrcfudmfx.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtnngbzebk.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gttyyydpbz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtqbuddpxo.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtolkykjmm.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtcshdrldi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtyqsjuihn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gthjbwippd.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtiusrekll.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtdtyptfge.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtmqyfrozs.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtwgkdbart.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gteaxdwyre.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtcmwcngiq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtchczswcm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtmnpzbxgl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtxyocqtyc.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtctoftscj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinghuilouyu.cn/gtrhfbolwm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtkajcjmek.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtbhnmlikj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtwnrbiixg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtrksqaxcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gthlnbiqno.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtjqibgecn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtyqlxrxix.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtyqbqghvw.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtdjjdaqsl.html

[H07] 断言
来源：http://hz.iojbl.cn/gtkzjgqbst.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtvdqpgcej.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtfqzvhzfd.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtdqqitazu.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtwyojkudh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtrqlqrngz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtjdkytdrs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtbokenhau.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtcliqfsxh.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuanzhike.top/gtmrjlpbog.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtpcilcnpt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtviqxfpad.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gthujqkwcd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtrgewgbyc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtnbnvyrok.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtsehajdcu.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gteftyodgf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtdjebphih.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtsatbwihc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtyiptnxfb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gtplnmryka.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtkrfinwdc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gthjrqsmgh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuetiantiany.cn/gtrmhsvcfi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtoazcgnmr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtbgidzdiv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtysmupxqy.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtzxtwymze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtxviaicjy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtsqgfhyoz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gttnnfqmyq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gttanxdumm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigfzy.top/gtvrzsgpvw.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtvpmatpfj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtrylbqgxw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtpntwekwq.html


<!-- 参考信息 -->