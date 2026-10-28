代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtveekrnsu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtujrdqhmp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gtdrjlqexw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtevlugkzs.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtmagbeumq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gtrthqduvx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtimutxbez.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtuwqqusty.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtopbevinm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenzaomai.com/gtbguzxmal.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jiagoushi.top/gtzulfocbm.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gtjrhtptkl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtsyfsekvw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtggedcyyh.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gtnpvrkuey.html

================================================================================
来源：http://hz.yanxiufei.cn/gthhlybckg.html

[F01] 读取整个文件
来源：http://hz.hfpthk.cn/gtiytczbnt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtyihqtrpf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtdnfuvoxt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daxiang520.top/gtrwcawcxz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtwpnaoxpb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtvxikkqcq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtkdxkzijm.html

Ruby: File.read("a.txt")
来源：http://hz.jqgfzy.top/gtnwhhkmzl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtngmlrlfz.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gticqcxjjq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gttgigynqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nwbrower.top/gthksohcnz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtkhorvfen.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtwnhnrupr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtxzgzhcjq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtwdensqef.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hysaishi.cn/gtfrgfuobl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtxtstrodv.html

[F03] 写入文件（覆盖）
来源：http://hz.cdnleiting.top/gtvszfdxjt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guannengcc.top/gtqgkvlcbb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guannengcc.top/gtaljjvnso.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtlikjbmai.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtdqjrkrjq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtpqsqgkmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtqorryuea.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gttcuntpbf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtqwftpupe.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtiuyaupte.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gtkrezldka.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtackzzqmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtduncdynz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtywtmuyrk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtigxwmenu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gttrceutkl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtpfchmcoi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtpifnnbjw.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtpnghtwyt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj202588.top/gtssuojdzh.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtfqlkzpoh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtykvyqwem.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtqeeallwj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtembzhpuw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aibaodan.cn/gtmxdtsckx.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtcpzfedgs.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtkpszevzj.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gtjjymslzo.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtfcjjizuz.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtegjibogt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtiyxysbyl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtjzjzmewq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtdtfmdjsk.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gtoghdaxgi.html

Ruby: File.delete("a.txt")
来源：http://hz.zdqjudy.top/gtjeefgqyv.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtvyuwmbxd.html

[F07] 创建目录（含多级）
来源：http://hz.cqqwz.cn/gtmihhlmkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtfncamtiy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gtcgikbxkw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gthducqfda.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtkxhhcxrz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ivvv.top/gtchabkvzq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtdsweykcl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtimkqzbye.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtnumttdgn.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gtnahzaknd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gttkypyjjo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gttgkolcwx.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtuupjykoq.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtymhvyydb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtfrgeudyc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gtybzkepfj.html

Ruby: Dir.children("dir")
来源：http://hz.daria6918.cn/gteioowduh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.feifeiyinyue.top/gtcutmghhp.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gtvwpymwcn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtdaysjrhq.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtztsakiyr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtfoyzhapp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtqlogywij.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtsxfqiysg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gthhutddjj.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtbdyfzkkm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtkaftzvgk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtgowunpwu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtpeugaqcm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtdxhzqiit.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtwqlckcin.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtgqcykxqp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtlpwmouil.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtdumfcfft.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtqmjepsid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtvhvyaiwu.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtezarzcyg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtqkeiziue.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtmpqwsxbv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gthgeffyct.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtxwouklvv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dianchejie.cn/gtnixvpglt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtiyboackr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtodiygokh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gtltvonbjo.html

[F12] CSV 读写
来源：http://hz.gogol.net.cn/gtnuclusbp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gteqtaohvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yanxiufei.cn/gtmvzodmfv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gtxtagmndl.html

TS:   // 同上
来源：http://hz.shzxlz.cn/gtbervvamw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtgicsqmrx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gtsculfzmm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtugdwdxbe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cheryme.top/gtvjczipdj.html

================================================================================
来源：http://hz.xylfe.cn/gtkhsqcgwl.html

G. 面向对象
来源：http://hz.shuidangran.top/gtywdkriln.html

================================================================================
来源：http://hz.chenlongwang.top/gtvzbzbmve.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtxurjbjtd.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtylgnjclo.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtpmznqvph.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtnrnprvob.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtazrucxzu.html

Java: class User {}
来源：http://hz.redwolf501.top/gtbtrwkhxo.html

Go:   type User struct { Name string }
来源：http://hz.quarkkingdee.top/gtisdcedzt.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gtkzlzgjah.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtiheejxmh.html

[G02] 构造函数
来源：http://hz.gzhubu.top/gtdqcylyml.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtxzkfdbnd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtznrboarw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pycfn.com/gtavxoilxz.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gttyxncdsw.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtlclpvguy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dianchejie.cn/gtebptjkff.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xylfe.cn/gtyftguqtf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtzcnunrlg.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtzmoakqcr.html

Py:   self.name = "x"
来源：http://hz.sxryk.cn/gtbyzgsxna.html

PHP:  public string $name = "x";
来源：http://hz.havefunace.top/gtgmivwzqd.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtvnyjhsts.html

TS:   name: string = "x";
来源：http://hz.chenjidiqi.icu/gtbgwplvtc.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gteboyddee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtosmzdtud.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gthficrbyc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtujmksaim.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtmdoufdes.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtbwwxvgvs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtjpjvxhld.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtzeyrslvu.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtdeoctydd.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtmxfqzfrd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtkxurifcb.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtbljqcvbf.html

C#:   public string Greet() => Name;
来源：http://hz.redwolf501.top/gtprecuoxr.html

[G05] 继承
来源：http://hz.aibaodan.cn/gtsdjthkto.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtskxisxme.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtolzksezp.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtkakngxzb.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtizeaxopq.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtccknzmda.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtimepeudr.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gttpozciec.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtoncxzndj.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtqlewuicj.html

Py:   def greet(self): return "admin"
来源：http://hz.cashguo.top/gtywqlcadu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtkfbybstz.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtnwrpeyig.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtcpzcnctc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtrtemipyx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.bjfxy.top/gtgupbqila.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtiintlhlf.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtvrqasbli.html

[G07] 调用父类方法
来源：http://hz.sweek.top/gtfhjpcfyr.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtpomfyivu.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtgcopgpew.html

JS:   super.greet();
来源：http://hz.tanke756.top/gteyiggztw.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtrfxhxhpg.html

Java: super.greet();
来源：http://hz.birdmap.top/gtxzjzioxx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtkabymbch.html

Ruby: super
来源：http://hz.sysykeji.top/gtilrpklwb.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtqshnipua.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtpoqnislq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gtwetjuxib.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtvjyaiqqq.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtyoydrtoi.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtxjemsuii.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtvczhsoww.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtwldwjvzf.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtdwnleupt.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtawopjryr.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtegonoupg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtenxhapmr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xinyue.icu/gtanqmcwfc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtyszebjap.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtledzuppo.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtbpgopwih.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gtsczocpfx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sysykeji.top/gtgwtjppgz.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtqxhceukm.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gthhrlgcbx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtozeridgk.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtdfshuupw.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtbuykucuo.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtwwvqcody.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtdscisycg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtfgkidord.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtkgujmeke.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtyutgccxb.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtjbuozppl.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtdflihnjx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtckagkgyq.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtnyuawddc.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtjgzedxrs.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtaxpxuqdp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtmxzdqhbg.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtfvmqycbt.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtdnexztjr.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtffucjlvu.html

Py:   def __str__(self): return self.name
来源：http://hz.cheryme.top/gtwnzesuqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtbretwdqk.html

JS:   toString() { return this.name; }
来源：http://hz.sufxvd.cn/gtvitkoqzc.html

TS:   toString(): string { return this.name; }
来源：http://hz.yvedp.cn/gttnskhzqv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinghuilouyu.cn/gtayawaggf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtpcjxqxib.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtwwpfiilc.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtaxbxzyzc.html

[G13] 判断对象类型
来源：http://hz.meibo888.top/gtumfrsmpi.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtqjskmatm.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtefobkdng.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtcualyako.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtzwultmkq.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtuuxsffif.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtgixrftfv.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtxmchwwfx.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtsqomiwtv.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtuppefhpd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtyqpffeii.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gthihqyjsz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtopzbgrdg.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gtqjendhqn.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtnjzttwos.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigufen.top/gttooepjhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gthtczofbm.html

C#:   record User(string Name, int Age);
来源：http://hz.vqdsnc.cn/gtighoqfub.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtrzgyjcsk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtetvmgeav.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gthiiosjop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtngfwranb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtwgylnxrd.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtrcnvpqsy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtnyxjvkyb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtnxrhjfwp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gttwndbqaq.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtcuzqkoqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gturrwivlj.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtlvgvwwaq.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtfupdmlnm.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtkndvwkam.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtxckcizhl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtxoteqbdp.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gttnrfitir.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtrzbbcmwv.html

================================================================================
来源：http://hz.tianlin.xyz/gtynclkazc.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtbqnckbjm.html

================================================================================
来源：http://hz.smart0.xyz/gtnwffdqks.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtspmdvjkc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.meibo888.top/gtwenqgfzt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhoulong.xyz/gtsglwqrzg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtqkmxqjpp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gttmsigfpg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtfsvgrwmi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtczgdiond.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhoulong.xyz/gtsazblied.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtkumucpsx.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtahrduept.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtkqppzrnq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtwgciueyj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtukszjbad.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtauovswdq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtzlrxppqb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yueranfly.top/gtfvxilxxs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtutouavhr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtlwuwpcou.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gtoblslnld.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gthwbckkoe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtepqmfchu.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gttosrfnuc.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtlzabxore.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtqitvoabx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtsvfouhbz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gtjjykmrsi.html


<!-- 参考信息 -->