代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtabzfnvca.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtgqeypqhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gaohongyu789.top/gtmastkgeu.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtupimrilf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gogol.net.cn/gtksfflwlh.html

================================================================================
来源：http://hz.xinyue.icu/gtlsmdekia.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtfodmqgyw.html

================================================================================
来源：http://hz.yvedp.cn/gtluyytsbi.html

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtfildhdjl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtuzzcpfyv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtvptlawrg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gttzeuhlwo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtxfhqlygn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtuhwzvmul.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtscknntvv.html

Ruby: File.read("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpezbtutz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtsbbochrw.html

[F02] 逐行读取文件
来源：http://hz.pengpengdd.cyou/gtmyhphohs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cqqwz.cn/gtorzpefsx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtdkmgjdwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pycfn.com/gttzyoqbns.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtgdwyrciv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shuidangran.top/gtyzajbpoh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtjihjoshf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtwqgdwyzp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtczilerds.html

[F03] 写入文件（覆盖）
来源：http://hz.hfpthk.cn/gtbhretefo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daria6918.cn/gtantsanrq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtuasiukeu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gttfmlhnho.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtcfjhuxic.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtdnasfqbq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.andypj.xyz/gtihvfvmll.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fzhhl.top/gtvrtcoaer.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtqattknle.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtqbfeugep.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtxxnrapcy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shzxlz.cn/gtbtlehqgf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtvzogagjk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtexihfnkr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtewsphldk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtpmlejomq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gteciemxsu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtwyplhomf.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gtpxpjhadx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gtlrskjpby.html

PHP:  file_exists("a.txt");
来源：http://hz.yj202588.top/gtjotinfrl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtfdjxucwh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtowliotyx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtitnakkkf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.feifeiyinyue.top/gtpproiunz.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtnhrvexwk.html

C#:   File.Exists("a.txt")
来源：http://hz.hywenlv.cn/gtraxxxzil.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtcllfeubt.html

Py:   os.remove("a.txt")
来源：http://hz.nwbrower.top/gtigvvxzet.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtqjvkbnzt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtnyehsduo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtvnqkpilu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtolnqcjnh.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtspmoaokg.html

Ruby: File.delete("a.txt")
来源：http://hz.xylfe.cn/gtseqiyhbn.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtwcubmcnm.html

[F07] 创建目录（含多级）
来源：http://hz.sysykeji.top/gtjavnrood.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtkkiirdzm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangdashe.top/gtzonhbutu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtmvjgjhus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtgtcjmxoh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhaomingkeji.xyz/gtivbgcfei.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtxckejhbe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.52xcode.cn/gteeprrbfl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtshpzylgd.html

[F08] 遍历目录
来源：http://hz.cheryme.top/gtakurhzwf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gtlcysgxvs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtggtmntht.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtwyqsskjm.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtssuwnzuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtrxrwtdfn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtjenoeqel.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gteymeogzq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtscjnrikt.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtjvbbywzm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtzllgjytv.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtwvzetiwj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtcsmryooa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtgzlqdnli.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gturfouktq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuanzhike.top/gtogziqavt.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gthvabpwbp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.vqdsnc.cn/gtvjovygev.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtkzmroamh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtxjncgzfu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtaqvakucw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtzspraulr.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtvlptozlm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtwehyikgn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtqxwyqmhh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtlujqepjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gzhubu.top/gttzzgagar.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gtrkfodren.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtpjhblklv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtuwkhuwci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtgeznxkyg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtrkhjsbit.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gturvmoqug.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhijiandao.cn/gtqlriileu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtzazxotjh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtsxdrklpz.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtaemynwbf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtnemqehfx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gthfntgkll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxuanxn.top/gtlpfeiaaa.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtbcvaatas.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtuxrfwhje.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtlovvkcnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtmxiizvuc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtvftqzgwx.html

================================================================================
来源：http://hz.hywenlv.cn/gtibgmmqtp.html

G. 面向对象
来源：http://hz.hfpthk.cn/gtjkhgallf.html

================================================================================
来源：http://hz.nwbrower.top/gtpcheckyw.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtaurfabva.html

Py:   class User: pass
来源：http://hz.nanxuanxn.top/gtfjmjqvpz.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtmetlnnxd.html

JS:   class User {}
来源：http://hz.nwbrower.top/gthpfonjoe.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtcpcyypij.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtlrfpilnd.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtvzxqkxii.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtpnpksncn.html

C#:   class User {}
来源：http://hz.ydzc1.top/gtlipyakuk.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtqbmittci.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtgbyicukr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxinkj.top/gtwcxnmsrk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtbrggciil.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gttelaprke.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtenwiuszz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtrvfyhjnx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtcjspplzy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gtainqscds.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtyxhlxqpr.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtcrbvxkpd.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtguygtfnw.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtmqlqqzcj.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtiaflnrow.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtbebjxiyo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtklshoeiv.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtwhxffuay.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gthghqytlm.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtezoiicpt.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtvaajyzdj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtxcdrfuyv.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtgestuhon.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtgfnldrko.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtdoktmpen.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtrozhktwg.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gthdslzbop.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtmajwojmt.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtufggszhx.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gtgqglrzen.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gtuexjfbdv.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtpchacxjk.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtysupqfml.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gthponhcwa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtnhviuabn.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtrscxokxp.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtcwmqbter.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtfskahhnq.html

Py:   def greet(self): return "admin"
来源：http://hz.hysaishi.cn/gtosldihqh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtobneyvbz.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtendlqxvy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtsyrnuynl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtkdyzugwt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtxmtgsdyd.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtxvjnquuz.html

C#:   public override string Greet() => "admin";
来源：http://hz.birdmap.top/gtywyunncb.html

[G07] 调用父类方法
来源：http://hz.yongpay.top/gtuwygfctg.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtvvmqmjah.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gtpscczffv.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtuovahzcj.html

TS:   super.greet();
来源：http://hz.gogol.net.cn/gtgysvwrne.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtiqwvxhhn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtxlhrjvdo.html

Ruby: super
来源：http://hz.tian-w.cn/gtqtagebad.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtfbjjdbkk.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtqgbrqqjl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtixpobjwy.html

PHP:  public static function f() {}
来源：http://hz.wangdashe.top/gtcfxkwohb.html

JS:   static f() {}
来源：http://hz.shuidangran.top/gtockakspb.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtuevpfeif.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtdqrlyfik.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtaybbncom.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtnvfqfbcz.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtljqoygmm.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtbwnzwguj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtgvuhlajl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtuvloyabs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yvedp.cn/gtwvbbhvnr.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtoaeyrbxt.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gttacpvbfj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtmlhezxkp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtgyagopfe.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtzytaydbb.html

[G10] 访问控制
来源：http://hz.zhoulong.xyz/gtdjxvzfhp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtgnapffne.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtexsepfhz.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtufhaksay.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtftqxjoln.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtsatcsnrh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtkxvrkagz.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtakzcvskn.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtdengqupz.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtupdoegvz.html

Py:   @property 与 @x.setter
来源：http://hz.birdmap.top/gtiiezzufk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.birdmap.top/gtvcoajnpa.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtolmvortw.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtuykbnuzo.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtjozhjzdc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtztquzwjh.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtmifulqwl.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtjvxotzuz.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtzhwbufhy.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtifdusevk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtfgfdzria.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtwkoufrbr.html

TS:   toString(): string { return this.name; }
来源：http://hz.yonumen.top/gtmfqplwfb.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtowmidgvj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtiojlnpos.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtnnesmtnr.html

C#:   public override string ToString() => Name;
来源：http://hz.zhijiandao.cn/gtkzsrsmtj.html

[G13] 判断对象类型
来源：http://hz.sufxvd.cn/gtjeqjjelw.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gthopvzwqp.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtsrfznmby.html

JS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gteyrurlyl.html

TS:   u instanceof User
来源：http://hz.sxryk.cn/gtblxnsclr.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtfrmkblis.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gtfvoegqav.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtznbkslrf.html

C#:   u is User
来源：http://hz.shuidangran.top/gtakangrix.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtyvtocrhb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gtzikslrca.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtprtzrnsp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtoxusumac.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gthaxkpseo.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtnvynkzqu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtdlhqanzf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gtwjkfdhnp.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gtmkocwtzr.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtztizhnzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtpouiiskw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtoilkwrxd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ivvv.top/gtzxtzusij.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtpkyujfba.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtgeehqbdx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhongyouzk.top/gthyborhvw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fengsongda.top/gtgrkdtdev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtnqfrbmej.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtpsxtgrcl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtyxdbvkbi.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtkykhzhlg.html

JS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtkilyygxm.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtnpmlidlh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtiarkfpxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtepglhexy.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtcbrvodpy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangshuangyany.cn/gtyfipalvy.html

================================================================================
来源：http://hz.xinyue.icu/gtbknbowhv.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtwclkhysd.html

================================================================================
来源：http://hz.316326.xyz/gtykzeweji.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtztcsqspr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nwbrower.top/gttbmhzonn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gthbbntqcn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtfwfqnxwy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtgkbhwkfa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gtrdsoyogk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gttmidftej.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.snrcjt.cn/gtcjkthmri.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gtybtznycb.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtegrjsouj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtubaultls.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtxpljtoeb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtfysjcvdy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtgdbodrzw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtqmpszfpp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtcioiyyyz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtglavlahh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gticogdikt.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtrscqgmtd.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtijpykxsr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtqwnixazj.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtesxkbrnn.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtwtzgiqlr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtoggwhjmi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gttjdljxxc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtfinfuybn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtmhqgbuch.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtorwyljsu.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtskygjkix.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gttgqazkam.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtupnedkfu.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtwvypqzmr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtxftrcfqj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gtshsvoopl.html


<!-- 参考信息 -->