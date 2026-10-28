代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtxqigrnuu.html

================================================================================
来源：http://hz.pycfn.com/gtjkyxmhaq.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtmewpczwz.html

================================================================================
来源：http://hz.jqgfzy.top/gtgxrncefi.html

[F01] 读取整个文件
来源：http://hz.mhx1999.top/gtzwppqiif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtyvslqgjn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtkndipvoo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtarivwgus.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtvyfgzsca.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtaxyjgckg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtrgibbtab.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtddeirtxt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtchfyruku.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtnjtqissp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtmcthhtnf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtpgiacwkm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtbibehutt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtpwntwjzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gthadiolqr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gtoytzslyt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gtthpykmdx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtigbtbxrw.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtouidrdpy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtuldkydhe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtmcuyivde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtzyvhcort.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.0kj1m.cn/gtybaqvpkr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtsnhxzgbt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtosnwknpa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtkcmdczak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gthfdfwwsg.html

[F04] 追加写入文件
来源：http://hz.tian-w.cn/gtxllwwopo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtqhzdykqn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtkvhlgnps.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gttjwvcvga.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtcryhddqb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258.top/gtodjprbrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtwpaookts.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtjqrwltwc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ybcxt.top/gtuhfrsowi.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtawywerqs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gtpwmngqyr.html

PHP:  file_exists("a.txt");
来源：http://hz.cucudq.cn/gthxgfykfk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtqesldkql.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtqyahpcnt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtmpykdizl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtmdukxbew.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtvvvblvko.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtkjqjjtui.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtlhsubpvi.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtkjufikuc.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtscuwshiq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gteqojbwrz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtqratqgdt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtdtksfrkb.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gtxvtujiep.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtgsdnjcpo.html

C#:   File.Delete("a.txt");
来源：http://hz.wangdashe.top/gtusgwbwbg.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtugdaddeq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtofelioss.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sweek.top/gthwhgzhmp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtxaldvrne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtgipcytzr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtlyfrduby.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gtsjwgdfhz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtzuegludc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gtncgsjnun.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtmioyberx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtwhfgbszs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtwpspkuiz.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtmezkepyu.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtsreopjuv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtacrpivkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtldyudogz.html

Ruby: Dir.children("dir")
来源：http://hz.ydjk.org.cn/gtkknrsegy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gthpullabv.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gthsaqjgam.html

Py:   os.path.getsize("a.txt")
来源：http://hz.mhx1999.top/gtfbcaafwh.html

PHP:  filesize("a.txt");
来源：http://hz.ydzc1.top/gtxzxhstnb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtfhjatcoy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtllwrtwoh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtldnvudni.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtvohmmlwu.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gtsnpbbhbb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtlbptqext.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtmcrtvocx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtleiexrbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtmzryxksw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gthwlfhmrk.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtfdpilycs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtkavuyikh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gtnxxjrrhv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtrinvtpou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtrotmvyjf.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gttbnoexzh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtwxfjjlri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gtkxglcpbk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gttdxanklt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtyvmkpgrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gtkdtxamkb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtljknhgij.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtcpfhjzge.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtsqdcuawn.html

[F12] CSV 读写
来源：http://hz.jqgfzy.top/gtrggrjesp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gterezlbmg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtjhmwvixg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.bjfxy.top/gtetdhqsld.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtmogxcfhm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtsotatgle.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yvedp.cn/gtejgmezye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtnnrmvngr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtphtgkajn.html

================================================================================
来源：http://hz.cashguo.top/gtffjuqitv.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtuvamwgdx.html

================================================================================
来源：http://hz.nwbrower.top/gttuzaywev.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtpaillohy.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtnfaiillx.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtqhpbaztb.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtlmlilcnh.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtaxqdbpin.html

Java: class User {}
来源：http://hz.nwbrower.top/gtriybjmcz.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtfcrskcqa.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtmomenxud.html

C#:   class User {}
来源：http://hz.yongpay.top/gtwofdgeyb.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtvisnppfk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.bjfxy.top/gtkgknzjdr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gtizonrntf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtlpqwwyrl.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtdhmfxbml.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtpjhmhswu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.9152youxi.cn/gtrqowoeqi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtoskjngks.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gterhzeqzy.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtdrgcmqpc.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtuagjjfru.html

PHP:  public string $name = "x";
来源：http://hz.nanxinkj.top/gtyvvlrgnt.html

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtqgxmsvzr.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtwrihznwb.html

Java: private String name;
来源：http://hz.tian-w.cn/gtrzcceoxb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtkqoorswo.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtxseljawq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.bjfxy.top/gtwbcyaxrf.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtxffnuiyx.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtpzotqrcu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtogrkrctc.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtfugbiltf.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtrcndeyjj.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtjsfrzyyd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtajbilmei.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtnlhrpixq.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtmowvausg.html

[G05] 继承
来源：http://hz.birdmap.top/gtlosgrvpd.html

Py:   class Admin(User): pass
来源：http://hz.yj20258.top/gtkrxtwonl.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtlnsjejef.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtsryelgbt.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtqvdnjbjn.html

Java: class Admin extends User {}
来源：http://hz.zhixingplan.top/gtxkhlehkx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtgzyngqjh.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtgwufsstz.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtvpdhglul.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtnzaarcrn.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtcotkyqoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gthmcelmcz.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtkmzxyezz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtlmmgiwuc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtrkllsuur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtjtyrmqdd.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gteoycbwuf.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gttqqazqfw.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtcmjzhwdh.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtbqbvschj.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtgsymtuuz.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtyrgnqfxo.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtikgpoagj.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtevycwbcx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtgocoqypk.html

Ruby: super
来源：http://hz.quarkkingdee.top/gtndfnngvt.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gtljjkwaep.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtdxopsxpw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yonumen.top/gtygzqyvmk.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtsfpqgbnh.html

JS:   static f() {}
来源：http://hz.ydjk.org.cn/gtibwwpplk.html

TS:   static f(): void {}
来源：http://hz.zhijiandao.cn/gtpheepzpa.html

Java: static void f() {}
来源：http://hz.jyoumei.cn/gtwppmtruk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtinjznkzd.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtvhnmjpwh.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtylaxkijd.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtllgqpfyf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtpegbcwqq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtlqctskdo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtpgzlidid.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtkdxyijev.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtndfgnbjg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtacuybnep.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtwfjmtgaf.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtajknjxqv.html

[G10] 访问控制
来源：http://hz.xylfe.cn/gtccjsknpi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gthvpegfjc.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtgycmxlaz.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtibvodtsd.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtrdatxejg.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gttxllbnnm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gttxjhbmro.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtuhvdbysp.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gtkudjhboe.html

[G11] getter / setter
来源：http://hz.sweek.top/gtuaxojjhv.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtggnqdedt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtoydkmiou.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtnnuxzdhf.html

TS:   get name(): string { return this._name; }
来源：http://hz.hysaishi.cn/gtvhnzdlwn.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtgzocfgoo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtbcqussoz.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gtmguyfiab.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtgcjqeirw.html

[G12] 对象转字符串
来源：http://hz.jlsjyb.cn/gtggbuhtvf.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtphgdloyj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cheryme.top/gtalhnxlwv.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtnzammtkk.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtmnnhscra.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtretmlmwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.redwolf501.top/gtsqtpwhis.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtuczkkwbs.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtqiydrhre.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtqmfpxhzo.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtlpqqcevj.html

PHP:  $u instanceof User
来源：http://hz.cqqwz.cn/gteyreunxk.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtbsiibuga.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gtbqbuzpbd.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtigciqmwf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guannengcc.top/gtnfnratry.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtlcktwqyq.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtecljvyyf.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtaygbeapm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtiycpfosw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtmngqbcuo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtzbzigiib.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtvriirjzc.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtxilnaveo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtkjcewvqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yueranfly.top/gtsswfhgle.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtopecmeen.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtqccsjbde.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.birdmap.top/gtoihpkenc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gtqttegbay.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtqxcqreuo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtzmvspcut.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtlnkorybx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtiuvqkxtn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gzhubu.top/gtymagkjjl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtjuvmzslu.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtkmwidkja.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtozewugqf.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gtygaffdob.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtmtacnwxh.html

TS:   Object.entries(obj)
来源：http://hz.pengpengdd.cyou/gtnrzaxicg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xylfe.cn/gticeocgag.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtoatwpyds.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gtcjeviaia.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtsjqoyvqe.html

================================================================================
来源：http://hz.cqqwz.cn/gtvevwdlnx.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtqmejzumi.html

================================================================================
来源：http://hz.ivvv.top/gtuazviuhy.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtoeysbgpm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtathrkjkn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aibaodan.cn/gtyqvtzmpj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtkfauvahc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtsqqeqltu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtmzvtjsaa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ywan-chungtsiang.top/gtlyuseuxn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtizptwvwh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtvyhzvydt.html

[H02] finally / ensure 收尾
来源：http://hz.52xcode.cn/gtwxxgpuqj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtzjprnyob.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtmmsinoek.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtdzhctvwq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtgezfmjko.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtonykglea.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hywenlv.cn/gtjpacfqni.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtrxtokfom.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtipjdlbjo.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtkkxasbee.html

Py:   raise ValueError("错误信息")
来源：http://hz.hysaishi.cn/gtykcjbqxr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtmldhnamw.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtorcaenco.html

TS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtyktnseqx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtohjtotuy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtldwuzqio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtiyxzgjng.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtpneaqbql.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtwjwuquay.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtudlmcumj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtwnycswwz.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtnzbzyxkj.html

TS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtoebihnst.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtnxdggmqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gthxgzzhnn.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gthrvtltoe.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gtjmlbfhmh.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtvpycjkfb.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtvbnjtljh.html


<!-- 参考信息 -->