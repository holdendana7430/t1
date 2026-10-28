代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtmvsvggez.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gtcrcgcwum.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigfzy.top/gtjarrngak.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jianghu66.top/gtvywzkhqu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtzscfdelx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtcgfzvjng.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtlegkqhva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtddfrlbqg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtfmpgacrd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fzhhl.top/gtvpgulauq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtcncljiiw.html

[F04] 追加写入文件
来源：http://hz.gaohongyu789.top/gtibitloxd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtjfikmwyu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtpyyjtbji.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtbdwevhrt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gthcmkfeqq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gthimffupc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gttijphfmj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hongshengwenyu.top/gtkahehack.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtzzbigyet.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtwbuhbtwd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtgmkulkpe.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtncfmlxcl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtqjewsftu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtuabitlal.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtvukkhntv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gttprllvgl.html

Ruby: File.exist?("a.txt")
来源：http://hz.gzhubu.top/gthvnbnzhc.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtyuoufysl.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtqezhzuhl.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdcwqqbih.html

PHP:  unlink("a.txt");
来源：http://hz.chenjidiqi.icu/gtxgcmsdmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtmzoqpgzt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtjvogsera.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtmghnddvt.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtlguijjci.html

Ruby: File.delete("a.txt")
来源：http://hz.hnxiangtu.top/gtdjvlbkah.html

C#:   File.Delete("a.txt");
来源：http://hz.jinghuilouyu.cn/gtaaxqsakn.html

[F07] 创建目录（含多级）
来源：http://hz.zhixingplan.top/gtjkogjjxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtcujhqunu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtmyuqilij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtbmeycfmk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtjbkuzymi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtwrfxilrv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gtbmarcnyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtwruxinyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gtpgwhgpoo.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtqcliudim.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtgkoenrad.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtelzsdurp.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtsmebsime.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtcubxbltq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtjclhqgof.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gthzvglvmy.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtdhtopbtc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtptqybbit.html

[F09] 获取文件大小
来源：http://hz.pengpengdd.cyou/gthentzutb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtfzxcsfhk.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtyqffluig.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtjxubohdg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtanezhqvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtsyqnejcm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtnzbvjgyc.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtzqdqxzhw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtoizbwmva.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtuibudjxw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtteftkddj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gtulipvtim.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtxdzwkxxj.html

TS:   path.extname("a.txt")
来源：http://hz.vqdsnc.cn/gtnaxxeiom.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtfmwsemgr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sufxvd.cn/gttwtfzhuz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwqvptixa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtxxnhdnjv.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtfepepjdn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtevoxloqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtjcdiqtkz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtqzhmtzgw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtepbtmcxl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtdrkdiwsl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtpdexttxs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gteiamzhjo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtvgpcnfwg.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtrowrwnsj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtyxpcyoyv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtjcaimedz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtporxwtcq.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtrgojhbsh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnqzz.top/gtvjkhizwi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtjhwhlgvv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtoyjdfbsz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtjgiggfpe.html

================================================================================
来源：http://hz.yongpay.top/gtnzitvwov.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtrndvyavf.html

================================================================================
来源：http://hz.hysaishi.cn/gtajgnurkq.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtoatdnbqz.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtxoucqkpo.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtdfvrgljq.html

JS:   class User {}
来源：http://hz.yj202588.top/gtyvczwnvq.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtvgmekkli.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtxktrdbvv.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtyrhtxgfj.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gtzbtsooiu.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtotpswiok.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtsxphwrxt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtxukorjoc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtuaacywjk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtddsccjlm.html

TS:   constructor(public name: string) {}
来源：http://hz.haohaochexian.top/gtwkvwjrpi.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtyzkywjfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gtrgvhxspw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtpjguikcx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtssfllarp.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtamqoysmv.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gtaywtyokz.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtrmxcslwb.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtsbbhhvxs.html

TS:   name: string = "x";
来源：http://hz.svipenyu.cn/gtpwbyrzah.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtralpmxzu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtxuwhfdiy.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtrrekwivb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtrfshpzyb.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtgrukjzmp.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gthtcmrbqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtuvgwnobv.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gtiumkcsel.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gtavzvbbcm.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtechsluxl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtevncdwua.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtucdntupx.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtrjoizrna.html

[G05] 继承
来源：http://hz.yvedp.cn/gttrwelzkh.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtzbkrohvi.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtjyexihso.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gthhhpiibv.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gttgkfdpyq.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtnofhqawr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtivhgywsq.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtjmgiketz.html

C#:   class Admin : User {}
来源：http://hz.chenlongwang.top/gtyqijpbbb.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtjrxajicb.html

Py:   def greet(self): return "admin"
来源：http://hz.feifeiyinyue.top/gtyozbvzow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtqcmlrfzv.html

JS:   greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtmvtbpznn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtyhkrwdis.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtqljwhizn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtiuvbwynn.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtlnqfimse.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtytyieghd.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtkxjizfwb.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtjiwxfdtw.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtgbaskabu.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtyiqilxnt.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtkisirfmz.html

Java: super.greet();
来源：http://hz.fzhhl.top/gturfzbndv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtajphrdja.html

Ruby: super
来源：http://hz.sweek.top/gtjliexouq.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtefqxttmg.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtlzmuwxeb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtfoxfwtso.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtgoqojjnz.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gtypjvohjo.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtqtjnzozy.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtasxyckhu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtltzvspwc.html

Ruby: def self.f; end
来源：http://hz.guowangkeji.top/gtobettyzr.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtslsqmqoi.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtamwjrlcq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtiqpxfdwu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gtjtuyites.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtavhlbtct.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangdashe.top/gtatqcsoio.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gthsvxrxhh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtbxfyiopj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtecpllidg.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtxqubibru.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtxvhflecw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zycfv.cn/gtagurdbxq.html

PHP:  public / protected / private
来源：http://hz.daria6918.cn/gtnjjcnjdw.html

JS:   #private 字段；其余公开
来源：http://hz.gogol.net.cn/gtcvhooxxc.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtweytkigm.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtnhbacwxo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgufenzy.top/gtmolnmtui.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtbykdqsug.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtfqelqqcv.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtxrqxbsrt.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtnjrvnbgg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gthrodnywi.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtvraybekf.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtofnplqvb.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtkbpritom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hysaishi.cn/gtebmukjmj.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtdnchyswi.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gteyvgndck.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtcixrnuoh.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtduzeasor.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtsvkrejqp.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gticfrjmvr.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtpaedudyq.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtmgpbhxsq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtcedtiaff.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtjbkbnplr.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gthuujlphv.html

[G13] 判断对象类型
来源：http://hz.0kj1m.cn/gtvbyxqlxz.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtwiemetdh.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtxdzqranh.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtsrppbdrt.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtdbrjwnmk.html

Java: u instanceof User
来源：http://hz.cheryme.top/gttyrefxdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cheryme.top/gtkqqeiarj.html

Ruby: u.is_a?(User)
来源：http://hz.xylfe.cn/gtmjswhncc.html

C#:   u is User
来源：http://hz.daxiang520.top/gtgreaqsuk.html

[G14] 数据类 / record
来源：http://hz.yongpay.top/gtbageorhs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigufen.top/gtbqgvqosv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtyxjimukq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtdwgzovex.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtkmpjzpsp.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gttvmojizy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtsvhcinvj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.haohaochexian.top/gtpuddteba.html

C#:   record User(string Name, int Age);
来源：http://hz.gaohongyu789.top/gttcdepfla.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtjnddmqxb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtsezqxsxg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtuulxmyaz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtgmvswrgc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtvxtcmjkt.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gtvagnnbmu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gzhubu.top/gtqeutdssn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtzvigxkue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtqeyoploo.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtljbxavzg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtdrcetdzs.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtltuyeptt.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtdgordrhj.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtbvpfzjir.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtoagqysde.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtnpblzulj.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtlljunvnw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtfnfzbtee.html

================================================================================
来源：http://hz.xziqi.cn/gtnxqaikvb.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtpwmswfws.html

================================================================================
来源：http://hz.cheryme.top/gtccjfuxij.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gtqpdlekxy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtxsljqfqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtzwejhrtp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtapxrwxct.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtffvfgvwq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gttlqhqpvr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gtgygigodn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtzsjihcsy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxuanxn.top/gtastxhnue.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtsqytvnuq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtioafvavj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtitmxoktq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtsqmuvsba.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtmsypjven.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtqrsfrfuv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cashguo.top/gtwpkgobti.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtkbimfixn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtnmynfilo.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtpuxlsfdn.html

Py:   raise ValueError("错误信息")
来源：http://hz.shzxlz.cn/gtuutlefou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtanyqruzd.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtoponvihh.html

TS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtnatmjxly.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtfkioeffa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhongyouzk.top/gtexyemepe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtvfnvujpz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtkxtjtzdg.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gthxcyxgob.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtuwpojdps.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtemwqafoe.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtjaauhahg.html

TS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtlhyzebsj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtdbiokxiv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yangfankeji.com/gtyfaqtotm.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtqbadxqel.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtakkbzlfz.html

[H05] 捕获特定类型
来源：http://hz.vqdsnc.cn/gtkarkxhsg.html

Py:   except ValueError as e:
来源：http://hz.sysykeji.top/gtdlxkrttv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhaomingkeji.xyz/gtnltmxhds.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtcnodekeq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtcofhvkoh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hammf.cn/gtsdjfadmv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtjzfdivhl.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtdlkbczma.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtcskjreqh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gthnglakqm.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtkdhyzfhi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtqpdsqlil.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtyighhycn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtynbpwryq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtjwmwnzro.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtehvmnqaj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtzhemqhlu.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtwxqkrnom.html

[H07] 断言
来源：http://hz.52xcode.cn/gtmuxuxjiv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtnjcdtzel.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtpzkpwnad.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtafdnszcp.html


<!-- 参考信息 -->