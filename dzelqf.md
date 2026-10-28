代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtaxrppkzq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtpuamxfax.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtsscgpjbs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtyjhujezr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtvdpemcwy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dianchejie.cn/gthwqrwcbk.html

[F03] 写入文件（覆盖）
来源：http://hz.wangshuangyany.cn/gtmhatnzcv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tian-w.cn/gtgsdfjvxf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtqjtwzdab.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtophcaalp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtjojmfdni.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtcspbpdsj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtbjzrqgzp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtijuffqad.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtfgikyodd.html

[F04] 追加写入文件
来源：http://hz.daxiang520.top/gtksyaywva.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtxaudbmyx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtdkorbcen.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtkbloqnpa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtmaazdglu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.birdmap.top/gteuzhkfnn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.quarkkingdee.top/gtsiwfulke.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtpighagfy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtlabgrniw.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtkhpqhspo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtndmyavrs.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtfpziocuq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtktujrmzl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtzgfmrgft.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtrfhshyqn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtbcetcnuu.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtouoeinhg.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtydtqymrz.html

[F06] 删除文件
来源：http://hz.fengsongda.top/gtqjtcajnb.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtphujnflk.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtnjwudnec.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtgnpayelk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtykyemgij.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtnklntvsz.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtribrgalw.html

Ruby: File.delete("a.txt")
来源：http://hz.dashuyun.cn/gtecoigaaa.html

C#:   File.Delete("a.txt");
来源：http://hz.tanke756.top/gtgcjybrhz.html

[F07] 创建目录（含多级）
来源：http://hz.zhoulong.xyz/gtapagrnuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gthmbbhisw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtbcttkbcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtvswqzdrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtihckqlap.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtvaeewnhg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtlgwdlfwa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtolscoeol.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gogol.net.cn/gtrujmtgiu.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtixnxygiw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangshuangyany.cn/gtmzrpkcme.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.havefunace.top/gthwolexjk.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtkycvlbnd.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtzerrwbww.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gthtuxywdn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtwykcvovl.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtvdznabqa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtgpgefmrj.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtvisljmro.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtckzjzbfy.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtmibjclrg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtnzvxtcul.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtmpkglsix.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtyinwkgyn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gttotvanob.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtbcyciulu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xziqi.cn/gtsldyxyvl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtpgmwqenm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtepryejco.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yueranfly.top/gtfugiiazw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtfkneamai.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtisbbqigw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtrrouooiu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtckbjcitl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gthaqicqdo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gtbckjmbyv.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gttjdshqpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtgyrnpqzk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtmbmcduln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtflnqmhbd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtmeiasner.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtfxfirvfc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dianchejie.cn/gthxhgwqke.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtkyecwuvd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gttwqlnfms.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtfotuqnbb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtwrhdzrtv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gtzfmxtwjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gthdbjaaso.html

TS:   // 同上
来源：http://hz.yonumen.top/gtdbffondt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtjlgqthcd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtcqsouxsj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gttnehnzzt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gthcmfdmrp.html

================================================================================
来源：http://hz.gzhubu.top/gtksrajaar.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtivnpjsyp.html

================================================================================
来源：http://hz.bjfxy.top/gtmdlcqpfx.html

[G01] 定义类
来源：http://hz.52xcode.cn/gtvbsdfbzk.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtdyjtbbax.html

PHP:  class User {}
来源：http://hz.gogol.net.cn/gtulhxltkt.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtyscwtvqy.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtbtzuaqik.html

Java: class User {}
来源：http://hz.daxiang520.top/gtiuthkcgc.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtwpuzvvbp.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gtxhbxxwyg.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtaorbmurk.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtxfprmxxg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtoffqafrl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gtbcpduqzc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtbinqikwo.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtgfcdmsyy.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gteizdidgx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gtnjlgpubk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgufenzy.top/gttciclwbk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gaohongyu789.top/gttpznkmii.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtyujfrela.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtpgmfnqpb.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gtsyfmrmfd.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gthiqnkvob.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gtyaxxtbew.html

Java: private String name;
来源：http://hz.shuidangran.top/gtjjxxhtvf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtcsyitgrh.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gttermfjxp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtlxilkzet.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtnzfjtnpa.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtpgfydjxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtvspcrwxs.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtyrtflflz.html

TS:   greet(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtujyhqouk.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtgdrpsjke.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtstykkped.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtfpjgmuav.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtiaclaqnx.html

[G05] 继承
来源：http://hz.sxryk.cn/gtlqzocxgo.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtvkgjtutl.html

PHP:  class Admin extends User {}
来源：http://hz.yvedp.cn/gtrupsldeg.html

JS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtuanwiiyw.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gturcxxfei.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtphpfhapj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigufen.top/gtuzpsqnqp.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtnmawystc.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtrpazvxfq.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtsvfxnvbh.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtjguzvfka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtwpobksyt.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtfnrtyepw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtjrzfcamk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtlsubcffg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtrmtloovj.html

Ruby: def greet; "admin"; end
来源：http://hz.ywan-chungtsiang.top/gtctythpxo.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtvmnysstd.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtklzbrevo.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtvxylzjvf.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtyspjskui.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtfryamtoj.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtkgjvahsv.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gtthnnixdp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtzxuhpzaf.html

Ruby: super
来源：http://hz.ivvv.top/gttghvnmza.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtxiljffoj.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gtdmqyfqjv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtupwdcmyn.html

PHP:  public static function f() {}
来源：http://hz.yanxiufei.cn/gtrqjgcmun.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gtjipricrj.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtfyhoxkti.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtmnrpflnf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gtumhkagct.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtnxjcrdig.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtbftasinj.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtxpfsxibw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtipxzxrzz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtrmquryvb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtetzasasc.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtjoqoymfk.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtdtqacfbr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtsympkcnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtxefhuxcv.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gttlilhhsl.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gthavcfnrn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ehwqpu.com/gtuogbbnuq.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtnyxoewyk.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gtoqixvhol.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtlqmkgamz.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtivdrkpih.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gthqhdeizw.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtxznxabyv.html

C#:   public / protected / private / internal
来源：http://hz.jinyuanbaomall.cn/gtuoveihul.html

[G11] getter / setter
来源：http://hz.xziqi.cn/gtaomrcpqs.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtkpffwygu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtvafdxryu.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gthohvpwop.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtcasryozi.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtpvcuymml.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtzxmaxocd.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtokqsuygm.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtjctqiomu.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtaqgocysi.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtbnovvskg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtytpndxov.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtyawgqzoe.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtdvpnufls.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gtfxhtofxg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtkrkwptpa.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtxgqasvqn.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtwqihuytt.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtviansqtm.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gthqzqrxgm.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gturcqgaau.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtihnxrtzs.html

TS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtqzqcuebv.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtmjjqkvlp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtlitoleli.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gteukehncc.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtxpzkiukx.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtbrzrqjtf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhongyouzk.top/gtrdyigbdx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtzehqnnik.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtpespxxub.html

TS:   type User = { name: string; age: number };
来源：http://hz.pengpengdd.cyou/gtmpmjkhqf.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtrxhnskue.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtkawrpsuo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtalntjcfs.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtplkclggn.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtsrgecadd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtissslbvr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtwuxpbdap.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtpqgdilwz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtvdhzcazk.html

Java: enum Color { RED, GREEN }
来源：http://hz.tian-w.cn/gtwtsxoctk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtqzsqkkys.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtdwasskiq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtnjbvvyyb.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtwakvffvm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtpzzpqoau.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtzgpforxd.html

JS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtgftvbqdl.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtridwzmix.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtfzbgpgsj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gtgmtwchdf.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtqjoidhhn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtklcfvzmg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkbzrjfss.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtiyddkhtw.html

================================================================================
来源：http://hz.xinyue.icu/gtkkcbbutk.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtutkousjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cdnleiting.top/gtupunqvfz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gthcospepx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtgvmdkppz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtzajbefei.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtziubgmpq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtdhuynzip.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gteedcwswu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sxryk.cn/gtcwrkvqgt.html

[H02] finally / ensure 收尾
来源：http://hz.tian-w.cn/gtaruzvjgw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtjtzwptsx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtjumwwvmz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtfkwgsgrz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtqziparew.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtxqyoarjy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gtcxphobth.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.9152youxi.cn/gtqmkbvzqd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtyihiycqc.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtwgnwrjjv.html

Py:   raise ValueError("错误信息")
来源：http://hz.ivvv.top/gtidanyrwj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtvxolbhud.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtzqwqrptx.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtdfuqupds.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtdksulqhj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.quarkkingdee.top/gtpbakmxcw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258.top/gtnqjqisvn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gthavhpmax.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtouimcpae.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtbysyjbrc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtsbqosjmv.html

JS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtmhxcvzfa.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtgbpglrrb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtgcvtxuep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtugbcwioq.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtrfefqycr.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtinffrtrx.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtzaacckyq.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtnsuuvkjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtawazmiuk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtycnppkhj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtutmsbrln.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gttdumhglx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtpyhktciw.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gthcdyiwxx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gtthqqayee.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nwbrower.top/gtonopaihb.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtnuqzfxbh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtabsupoes.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtjfbgpiik.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtmrnmbtud.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtieseldbv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtkflmqvwe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtiodothlc.html

C#:   obj?.A?.B ?? default
来源：http://hz.hongshengwenyu.top/gtfinzxnxw.html


<!-- 参考信息 -->