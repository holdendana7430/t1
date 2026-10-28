代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxinkj.top/gttiniljno.html

[F02] 逐行读取文件
来源：http://hz.pycfn.com/gtbpqilldo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtnclbwgrg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtvtpostgw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtysvbxclj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtyyvfjsxa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gttzdytepv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtvhqzntfb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtuinodxfg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zdqjudy.top/gtwgdtvrxa.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtfjzjgdnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuanzx.com/gtqwbsshsg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtmqnsoilu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtbtjgtirr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtkiafyxcc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtjdqpzdmf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtijgiwtga.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.haohaochexian.top/gtlgccipsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtmslliesc.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtapaimhyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hywenlv.cn/gtxnvjgcrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtjpixycnm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtdwbogszn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gthxggrxkt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtzuxnemaw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtuxoprnne.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtnapvdbmh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhaomingkeji.xyz/gtohxswuqn.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gthpnosfmd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtcsxodgba.html

PHP:  file_exists("a.txt");
来源：http://hz.nwbrower.top/gtumvnxtrn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtydlvlksm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtzypyyndq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtuxojuxtj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtvozdadlz.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gthqqbxwxd.html

C#:   File.Exists("a.txt")
来源：http://hz.zdqjudy.top/gtolscjdzv.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtptjvbyge.html

Py:   os.remove("a.txt")
来源：http://hz.svipenyu.cn/gtiudqsldh.html

PHP:  unlink("a.txt");
来源：http://hz.wangshuangyany.cn/gthevpnzll.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtjqyrygre.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtynefukrp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtcvjkoirl.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtyzdwsoas.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtblfdiwto.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtnzshwvtf.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gteehnrrwr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtploxgvli.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxuanxn.top/gteyrcvxal.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtsskgdbew.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtjajptdoo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gtgtrlyfeu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtgfdoszof.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtmxqcosqo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtzoujtyls.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtnwxuyqjv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtuerqeqan.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gtvkapvpzj.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtphlqrtbl.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtphjfhuoj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtbdbqwprp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtzhnzelmr.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gtauedwvhy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtldsjvbdx.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtbhjwlkzz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aibaodan.cn/gtrvoqnjst.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gthgizdwwz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtpwhjiwxs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtizenktgp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtemsmztak.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtfbfotieh.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtbpkkrkna.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtmctdpnar.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhengqikj.top/gtahlgzsmi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtvfrxkcna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtcqppwlfv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtkchwwoef.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtuemslggl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.andypj.xyz/gtbihlbwfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtonuugjcf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtjsmyyocd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jianghu66.top/gtrmeiusue.html

[F11] 复制与移动文件
来源：http://hz.gogol.net.cn/gtbtibbtxu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtjazgtkdl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtzjuinikq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtycxrlxcg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtcdcfxtwh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gttjiwtkpu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shuidangran.top/gtieihpvlh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtxxcsyeui.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daxiang520.top/gtggntwcsv.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gthdlmsbpq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtaqtdjydd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yanxiufei.cn/gtllhsoyls.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtnfvucpau.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtremwuoky.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gthmykmnit.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtklwaibek.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtizygsyab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtdtgpyyqs.html

================================================================================
来源：http://hz.jinqigufen.top/gtszdvvytc.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtxxmloxih.html

================================================================================
来源：http://hz.yanxiufei.cn/gtaptrjuqa.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtycnaxlzl.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gtmblujies.html

PHP:  class User {}
来源：http://hz.shangyingyoupin.top/gtterenqnh.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtgeekikgu.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtjbiukati.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtfelwkgvf.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtbqhsvxew.html

Ruby: class User; end
来源：http://hz.cashguo.top/gtqahnwzqf.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtuxtsqjdv.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtjgyogvpc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gtscswmksh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangtech.top/gtdffmghhs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtqudtzwns.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gtpfqqpnef.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtozvqokkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtceezbfbk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtofrergdc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtznzjfkob.html

[G03] 实例属性
来源：http://hz.yonumen.top/gttkyupooz.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gtbwreuqjw.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtgvlvidip.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtgldahgmu.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gtfrerpuft.html

Java: private String name;
来源：http://hz.yuxming.cn/gtfqazbhob.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtthbxovdz.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtucstwetk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtbeutnkeb.html

[G04] 定义方法
来源：http://hz.zhijiandao.cn/gtskengoau.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtwkurotrw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtmugjcbid.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtwgsthnom.html

TS:   greet(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtxvbycvpa.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtqobysmfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtdykmcddh.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtthputlxv.html

C#:   public string Greet() => Name;
来源：http://hz.ydjk.org.cn/gtbrcffcvp.html

[G05] 继承
来源：http://hz.aibaodan.cn/gtkkfkqiug.html

Py:   class Admin(User): pass
来源：http://hz.cucudq.cn/gtadqprkwj.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtgwalwobw.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gttnfsgffe.html

TS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtvnzpocfc.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtcaveumqn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtaljazfxq.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtxurligrj.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtobraobuh.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gtswmqknna.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gteeolaijz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtivxklvbp.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtocmalijz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtkxeziynf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtsibockya.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtwsnmlbmc.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtplcupzmi.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtwarlhddy.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtrbmrdkec.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtnpbfbtoq.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtdpzrsplr.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtgygspoly.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtwzfuwfuf.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtgixscxjc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gtomzymmwt.html

Ruby: super
来源：http://hz.chenlongwang.top/gtufrceheb.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtyqivlchx.html

[G08] 静态方法与属性
来源：http://hz.jiagoushi.top/gtdczqgifu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtwqjedljn.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtsitlsldp.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtjrvuuztb.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gthrytksgi.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtakhbslso.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtqtbezkhr.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtzihktyrv.html

C#:   public static void F() {}
来源：http://hz.vqdsnc.cn/gtrvozojig.html

[G09] 接口 / 抽象类
来源：http://hz.xylfe.cn/gtqkpknrzp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtkfdbjvun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtctkxuiug.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtjpfgkwpp.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtodomfhux.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtlprocali.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtxabucpbr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtnkfogmpk.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtjzsixoav.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtrknolblw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtpxysngco.html

PHP:  public / protected / private
来源：http://hz.vqdsnc.cn/gtquzlrhfm.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtbhvzqtxi.html

TS:   public / protected / private
来源：http://hz.jlsjyb.cn/gtsiqvqjes.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtuyjoabkd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shzxlz.cn/gtyhxxcrhb.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtxhbxzpcl.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtnpnnqtap.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtkglsikpc.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtvhjavonw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.52xcode.cn/gttkaqmhun.html

JS:   get name() { return this._name; }
来源：http://hz.nwbrower.top/gtifpwtejl.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtnzajywpc.html

Java: public String getName() { return name; }
来源：http://hz.snrcjt.cn/gtkoyvbwlv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtpvpnotzn.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gtyksejrvk.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtugvglikd.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtgkzlrosc.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gthczjxkjm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtytzkuarz.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtkrgpuryd.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtiqwqyzzk.html

Java: @Override public String toString() { return name; }
来源：http://hz.jianghu66.top/gtncynwarx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.9152youxi.cn/gtzzjkigbq.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtogqydnyt.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtgjuruvst.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtungbvegh.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gthmmclbmg.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtfxjxoxgc.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtupeirbat.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtbermekul.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtspgzzhlx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtwtndiiez.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtkozbfoyf.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtplspqtse.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtleiwwlkb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtgrqbffjb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtoeyesbit.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ppjwa.cn/gtzcjlufyx.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtewhdcwrh.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtgyzhxgli.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtvjktvklz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtyzkquwgt.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtshhjvqbc.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtxrpfeeqg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtvjpslvga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenzaomai.com/gtiqbufbtv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtmqnpdixa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtxldmktss.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtrqfsuvwj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtfrlqjvpu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtaayylqpg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtpdxrymmp.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtenmlgvnu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtmjgtbqsh.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtjlyvysgp.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtkpdezrli.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtifonwqod.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gthxrnmayn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtrxncigqq.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtxnqxvweh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gthetbzlwv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxfkrgxkd.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtwkejsafn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtubenkufm.html

[H01] try / catch 基础
来源：http://hz.havefunace.top/gtfsxshgkq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtcnguigrh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtrqkfoznd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtrzrcspyk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtpffotwpv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtacnccwge.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.c1oappe.top/gtkezxswin.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtjvkdlmtz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtcvabbfbc.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtlbenzxkr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tianlin.xyz/gtqhkdzpkt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtpgvteess.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtlfpqlhhw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtguyzydji.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtuvladryv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtffpvmgju.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtkjrpxaby.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtotsdbjby.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtgwbietnt.html

Py:   raise ValueError("错误信息")
来源：http://hz.yangfankeji.com/gtugfactnh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gttycnssyv.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gthddqgczv.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtriaycppu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtbrjfjqrh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtupheuaig.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtrbgzkbae.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtsukoulkb.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtjkphwzus.html

Py:   class MyError(Exception): pass
来源：http://hz.yj202588.top/gtfwgxgbyg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtqobgrhmt.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtaajpdxwv.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtbkosrifp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nwbrower.top/gtbbhspsgo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtjwhynegk.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtuplkrlyn.html

C#:   class MyException : Exception {}
来源：http://hz.jyoumei.cn/gtdakdnsah.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtgvinycxz.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtuplerumm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtcelxdduc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtsqzinkuc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtbegerpqn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gttyxwmbju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtpqsjfltp.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gthoqhntgc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sweek.top/gtfzrvponb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtwqvnlxsq.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtcgrbiiev.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtqfzavxzl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhixingplan.top/gtloxlgrwz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtmfpdznoi.html


<!-- 参考信息 -->