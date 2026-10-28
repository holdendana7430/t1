代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtegptxacy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gttztsyzzk.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtxgxiqtha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ehwqpu.com/gtepzefpwh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtfkhlhpas.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtwdoghzgv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtfhvvwlzx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtqgodvxtd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtgofvaeve.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yonumen.top/gtuxjkrbiz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tian-w.cn/gtwbanpswn.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtwgzxrmhj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtjohhwbfz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtniydaijv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtiifcnfct.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gthmonoxrs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtirflypug.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.iojbl.cn/gtlnbfmldn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtafgyjblk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtareybwba.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtcskisxks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtbucocoyq.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtmocwfvgi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtajweutxw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtjuxnydmo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtkwdbgkjm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtimdxfvce.html

Ruby: File.exist?("a.txt")
来源：http://hz.birdmap.top/gtqfpewzmb.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gtvzrjoaue.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtdupwxmdz.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gtoplycluj.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtshgsryte.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtmkihrjey.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtmfxtmxpr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtxagqhqtk.html

Go:   os.Remove("a.txt")
来源：http://hz.9152youxi.cn/gthehmawgd.html

Ruby: File.delete("a.txt")
来源：http://hz.wangshuangyany.cn/gtrocsfipa.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gthtdenxhx.html

[F07] 创建目录（含多级）
来源：http://hz.aizwys.cn/gtyqvxsuij.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtlfbdgzhe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhoulong.xyz/gtqxbhheju.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtjsaevdeq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtgcwphbdv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtoqdfjdmu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtwdttwauf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtfpnxowog.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtwxllbxtz.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtppcusaeg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.dianchejie.cn/gtzcbmtruu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtovhaqmxq.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtmenkvsqg.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtngdkzrso.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtdkxjibui.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtfzkzzoek.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtxbmscqeo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtogcklrdw.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtqiflnqbw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtwsdapxqr.html

PHP:  filesize("a.txt");
来源：http://hz.xziqi.cn/gtfxpinomm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtiiprhebc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtjqdbkemr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtmavkiurf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.c1oappe.top/gtgbipmaas.html

Ruby: File.size("a.txt")
来源：http://hz.yvedp.cn/gthyqosbgz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gthllxhzua.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtwsuxihtj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtdrcvexyj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtxeytdkhd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtvznvfqsi.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtcnrouyzq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtdpydlaka.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sysykeji.top/gtfxgeyrht.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtykqhcypt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtuspapeva.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtbibswrxd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtlocpemwz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtxynetdru.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gttwzadwvk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtsjwrdwpm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtbmyjspsw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtnlkdizlt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtmjgnbghs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sxryk.cn/gthtsknnbg.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtqqzsxonf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guowangkeji.top/gtfzretpls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtazdqkcvi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtlvfjqvtg.html

TS:   // 同上
来源：http://hz.yj20258.top/gtqhxgqvgx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtekjkmbvk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtgmfvxwjv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtrkwibabs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gttgwlwray.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtcbrnqlmy.html

G. 面向对象
来源：http://hz.havefunace.top/gtwwvjkwik.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnthenlgf.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtedxqovfk.html

Py:   class User: pass
来源：http://hz.birdmap.top/gtflysphtc.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtfgfcttkv.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtznqcjtee.html

TS:   class User { name: string = ""; }
来源：http://hz.andypj.xyz/gtznbzhxzl.html

Java: class User {}
来源：http://hz.52xcode.cn/gteqqqsphy.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtutlszsed.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtjsmipnex.html

C#:   class User {}
来源：http://hz.yongpay.top/gtgkaljfyt.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gteolkvnft.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gtdgntivsg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtuibyufge.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pycfn.com/gtvyagizoo.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtglztcuxu.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtjatcjlft.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtwyacqlbx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhongyouzk.top/gtcmvikfuo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtswwgfjmd.html

[G03] 实例属性
来源：http://hz.hongshengwenyu.top/gtywkndzuh.html

Py:   self.name = "x"
来源：http://hz.zhongyouzk.top/gtufvyqybc.html

PHP:  public string $name = "x";
来源：http://hz.jinyuanbaomall.cn/gthrooigwn.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtrnuzhhlz.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtebvxtpkh.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtxvlapfgb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gttcddjimq.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gteybuuyre.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gtxspjsxqd.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtdyxsmdqs.html

Py:   def greet(self): return self.name
来源：http://hz.hywenlv.cn/gtcmwspnlu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtmizwpyfq.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtlyzedfbc.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtvytcirnk.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtwppkllbi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtkfrgcmdc.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtawrasaod.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtvzisoqae.html

[G05] 继承
来源：http://hz.birdmap.top/gtqissddzc.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtwgwbwjlm.html

PHP:  class Admin extends User {}
来源：http://hz.zdqjudy.top/gtznjsvhzx.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtkxszfjwj.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtgxunfzfb.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtcsyoyats.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtcdioxwqw.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtmoiqdwbi.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtvceubukw.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gteafkvlob.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtwwnlfwxc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtcratogdy.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtdxaxpbzg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtpadniyps.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtggmgsrme.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtqmyaqfer.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtlvjaoert.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtizwqkuht.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gtoibntpfx.html

Py:   super().greet()
来源：http://hz.ppjwa.cn/gtlecdjflk.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtltqewzdv.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gthhyfrfep.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtzpqwqbhr.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtltcnrsms.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtbupolsrg.html

Ruby: super
来源：http://hz.yvedp.cn/gtmglfiuqs.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtgstguqks.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gtadnsnkyg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtztsrelfz.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gteztmxioj.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtoemlikuu.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtwkhshrel.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtklopnsbw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gtutywvrnb.html

Ruby: def self.f; end
来源：http://hz.wangshuangyany.cn/gtuatcuonh.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtkoitnref.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtnsadntfg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtcbnxdvix.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtelhmspqj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtotkthxda.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtohwzjhuz.html

Java: interface Shape { double area(); }
来源：http://hz.xziqi.cn/gtouotjcua.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtfhsjialn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtkjciltii.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtxnjpotxv.html

[G10] 访问控制
来源：http://hz.sweek.top/gtpzfimbhm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtksmvfhxy.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gttimoofjr.html

JS:   #private 字段；其余公开
来源：http://hz.xingfuxueyuan.xyz/gtvwzzzxzt.html

TS:   public / protected / private
来源：http://hz.birdmap.top/gtpiajbqwj.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtcwfbolhh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtpebygpvu.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtotomqwry.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gteulygnmq.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtpynpcupy.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtjlktdhdl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtxnicvsam.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtsnqdpvqd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gthobxbwlt.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtiompsbgy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtkhfmrwvt.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtglyibysc.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtaeaaoboe.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gtxpkvzuyx.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtwcuawnbe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtytalnwao.html

JS:   toString() { return this.name; }
来源：http://hz.52xcode.cn/gtozbuqrgy.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtszedtzns.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gthvfvzxwf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtkjecewob.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtfwedpqmi.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtlxgcqano.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtkjdknoud.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtrnigbzaf.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtycmmcgza.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtufenlhom.html

TS:   u instanceof User
来源：http://hz.gzhubu.top/gtfewvkeew.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtmhuvomow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtaamewbdf.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gtliltlniv.html

C#:   u is User
来源：http://hz.guowangkeji.top/gtlrnkjxdm.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gtokcnlkts.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtfhxckkdx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtzutfdakc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuanzhike.top/gtxehqxqmx.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtjiydorul.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtypwfpugm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtkaatrmrq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenlongwang.top/gtadyfcenw.html

C#:   record User(string Name, int Age);
来源：http://hz.9152youxi.cn/gtrxhckovz.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtbgwwzbgb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtofwakoqb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gtpbtdljyb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtymmbmgkk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtipresitj.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenjidiqi.icu/gtqlelgqrf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtdncgiwut.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtllotalnb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtjubexbvz.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtqugunhpz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gtbcolhufk.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtptpmnwiy.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtqvqhwfzj.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtgwescqpl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtozqubjnk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtueevpqfs.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtuathohzj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.haohaochexian.top/gtweoizexq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtradzdhcf.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gtomhmqvih.html

================================================================================
来源：http://hz.nanxuanxn.top/gtictaoxmg.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gtopaddivf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gtttlbykgc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sysykeji.top/gtfaijpjuf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtmpmxczdm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtwgevenbd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtaixygzbh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gttwyggosy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtadgpkcro.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gtgbdbwsvi.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gtnmgchpmi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtyilsrpbv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtqnmivjta.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtcwawuwoj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gttghbnkmm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtyfhzemdh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtjaphwbpf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtqaayseua.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtfrransyy.html

[H03] 主动抛出异常
来源：http://hz.snrcjt.cn/gtasbzotqs.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtzxxzjjza.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtucurxusk.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtknwncksq.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtjhrjzzwy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtweprxcuv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtewmdnhuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtmuhsbafp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtmkngvfhd.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtliscsdxw.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtovvxkorw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtquoffbhr.html

JS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtfbudrtng.html

TS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gttdcrvmtv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtwhbxmigj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtrhgcxgbn.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtjnbjlwst.html

C#:   class MyException : Exception {}
来源：http://hz.jlsjyb.cn/gtllgigzle.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtrhbsktid.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtoxpxxpva.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtweywyevc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtukvvkjna.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtfyojttvg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cheryme.top/gthiqsptbc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtropfqeqt.html

Ruby: rescue ArgumentError => e
来源：http://hz.shangyingyoupin.top/gtaontdpip.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtnvwqpruo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtudykeull.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtboivazln.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtsgzdvsyz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtxpgvqcwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtgdsukjwe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xingfuxueyuan.xyz/gtxgdzahan.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtcfhytvho.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtbflcnthd.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtonfwnyyg.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtzigfeqzk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtitoqwvha.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtckawrfyn.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtwaudinkl.html


<!-- 参考信息 -->