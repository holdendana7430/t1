代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtdjflfrve.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gtpnvzvfza.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.mhx1999.top/gtlxuxtvrv.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtfscowylj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtesoykvdm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtatnfebez.html

F. 文件与目录
来源：http://hz.birdmap.top/gtgztmwxcf.html

================================================================================
来源：http://hz.hfpthk.cn/gtotguaors.html

[F01] 读取整个文件
来源：http://hz.pycfn.com/gtreitonhb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zycfv.cn/gtobthrczu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtqelvzcfl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtnlseoqiz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtvevpnxvx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtatrevgya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xylfe.cn/gtsyrdgoni.html

Ruby: File.read("a.txt")
来源：http://hz.xylfe.cn/gtgnegvawe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtmmfcszpw.html

[F02] 逐行读取文件
来源：http://hz.svipenyu.cn/gthoivmlkp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtmvrttekz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dashuyun.cn/gtaalgxoce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtgywhzugm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtimafkwnx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtaqekspmh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aibaodan.cn/gtovfpkxdt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtizegsuxg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtteasqusc.html

[F03] 写入文件（覆盖）
来源：http://hz.zhongyouzk.top/gtztpoarwv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtdckzezei.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gtgqbvwvow.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtiuuggltx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtnyojbgkc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtadunzgqd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtndmoofyw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gtmveswhfd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtewczsvus.html

[F04] 追加写入文件
来源：http://hz.yangfankeji.com/gtuasukwip.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtncmiklen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtugbcwgpq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtaradmjyo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtmhrtjrfd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gttgicitzb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gtuleemfqw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gttcvprnhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.svipenyu.cn/gtkyvscvsc.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangshuangyany.cn/gtiwaptjmx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinyuanbaomall.cn/gtksxxtczk.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtwdhnrcpr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtofnxqanc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtmtnxooab.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtifvoyura.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gteopqboya.html

Ruby: File.exist?("a.txt")
来源：http://hz.0kj1m.cn/gtgbdsxoau.html

C#:   File.Exists("a.txt")
来源：http://hz.daxiang520.top/gtmynplarb.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gthopwqdpq.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtgasmbyyv.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtimezhqol.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gthrcdfpxt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtzgbpavkp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtforsajyr.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtfozpkjyj.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtevrjnpqd.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtiyrrabfh.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtaxhyeyva.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtwszynaue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtcphhfcyh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtdstsenoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtmvliskdo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yonumen.top/gtjlhaqovw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtildraokr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtpnxfdbft.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gtugkcsqoz.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtxrrtjtoj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ivvv.top/gtxvucraee.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtocmfvdpw.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtetuljnca.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtcoiadwch.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtatetbeuk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtfqzlwwak.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtxbnjfvzb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuanzx.com/gtffmstxat.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtsxiddtuk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jyoumei.cn/gtiogggigl.html

PHP:  filesize("a.txt");
来源：http://hz.zdqjudy.top/gttsfxzhfe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtgtigqukt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtwebiyksz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtbhxekukq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtxweecuwf.html

Ruby: File.size("a.txt")
来源：http://hz.yuxming.cn/gtvymigadv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fzhhl.top/gthdoysjov.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtvqzqoavi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtfffsonru.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guannengcc.top/gtayyjoait.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gteybbwhvs.html

TS:   path.extname("a.txt")
来源：http://hz.yonumen.top/gthccbgpwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pengpengdd.cyou/gtuomizbcn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtcjernwda.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtrrdsodpc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xinyue.icu/gtbtkesnma.html

[F11] 复制与移动文件
来源：http://hz.zycfv.cn/gtxxkqpxur.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtwgdbatzf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtzegwrtfq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtrtwoitkv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtrnsqhkwr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtyapcvljs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ywan-chungtsiang.top/gtvosxuoho.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtfsbmoeza.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtvwahvbeo.html

[F12] CSV 读写
来源：http://hz.sysykeji.top/gtfxdyebac.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cheryme.top/gtnsujvqhb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtfrpmbdxh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtfdbneyfy.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtmvuxoihh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gtbpjlferj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gttilstdyf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtohxxdxfi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtgnyvumsr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnchtwgud.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtqppsoaio.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnirlmvgf.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtrzqigxgk.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtmuxqslgg.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtxucvnktj.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gtmcmdpdrm.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtxeutuumd.html

Java: class User {}
来源：http://hz.aizwys.cn/gtnzsenzqh.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtxpkslpyi.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gthatajynl.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtcprcwxyj.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gtlctshroo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gteewfksos.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtfnckexis.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gttmhdxkvx.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtojiovqnb.html

Java: User(String name) { this.name = name; }
来源：http://hz.gzhubu.top/gtlpxupybh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gtbtkyblxn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtiqqzmndl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtsthmsgxv.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtyvxtnllo.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtersvdynk.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtnfxpdfrf.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtidjfqygt.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtrgtkyxnf.html

Java: private String name;
来源：http://hz.gaohongyu789.top/gtcobrpaow.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtcaadqepu.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gteeeygddl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtmxhemvao.html

[G04] 定义方法
来源：http://hz.jiagoushi.top/gtwytzhffw.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtwowbljfk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtrnccddct.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtzlufezso.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtonzqkaqu.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtuyokejlg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtuiucvnlm.html

Ruby: def greet; @name; end
来源：http://hz.nanxinkj.top/gtcxjqpjso.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gthbmardhi.html

[G05] 继承
来源：http://hz.yvedp.cn/gtdwcpftrf.html

Py:   class Admin(User): pass
来源：http://hz.fzhhl.top/gtyknnqcdi.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtxwszhasm.html

JS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtmssnltpj.html

TS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtfrxvbfto.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtimfkhepq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtjeecbmpv.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtbvgtdyvq.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtbkcgvsuy.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtttbrlbpg.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtqbvpgjfy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtxqsvjfat.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtefillhjg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtqyucydim.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtcsxzmmak.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinghuilouyu.cn/gtfpknhyuo.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtudaurzdt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtarcikxcv.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtihrgwgoy.html

Py:   super().greet()
来源：http://hz.yj202588.top/gtrtaibzhy.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtkmbctmys.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtkgthbplq.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gthrhufyln.html

Java: super.greet();
来源：http://hz.yvedp.cn/gttxiawaft.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.svipenyu.cn/gtjgmzsfqr.html

Ruby: super
来源：http://hz.zycfv.cn/gttymbbqvv.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtwcxtnxsz.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtesuemail.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtqzwaxwbn.html

PHP:  public static function f() {}
来源：http://hz.jlsjyb.cn/gtqxrairpd.html

JS:   static f() {}
来源：http://hz.svipenyu.cn/gtyibqavio.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtaoewdcub.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtryiaafvg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtsxwduegr.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtsvuqvmtl.html

C#:   public static void F() {}
来源：http://hz.316326.xyz/gtzthxnkyc.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtlgrsdxqt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtfmzkqotz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtcyqpklgb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gtnpfkrbmq.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gtbycnybua.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtkzgooajy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtwdhmrtya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtxnuvzbah.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtfdhrpyrj.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtlhfayiud.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtiktsqokg.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtbkxipbgt.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtwkdwkbnr.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtrmpocbyu.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtcrjdzscs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtovsknujo.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtejicyfei.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gtperufsuz.html

[G11] getter / setter
来源：http://hz.birdmap.top/gtpprvqqwu.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtozscokvb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtrxxowalq.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtvuhtqbyz.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtjlzpidpm.html

Java: public String getName() { return name; }
来源：http://hz.ydzc1.top/gtsfykydly.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtqeqeheoh.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtdtkvfxqm.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gttkhaegpj.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtetpoamay.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gteqxdyiup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtgunairpb.html

JS:   toString() { return this.name; }
来源：http://hz.vqdsnc.cn/gtstszlofo.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtvmwffirv.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtjwvmdbqd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cheryme.top/gtanrqumgh.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtzobyeszi.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtpycjxqxo.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gttmblmskx.html

Py:   isinstance(u, User)
来源：http://hz.guowangkeji.top/gtdmiblptx.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gteqgtcbip.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gthlojhaqv.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gthwnknlda.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gtctyidgpt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtzeuprhyp.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtdlgoirvq.html

C#:   u is User
来源：http://hz.jinqigufen.top/gtibtfflwi.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtoebkfjpt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtnulqcrgz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtxwnnskwy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtazlmmeol.html

TS:   type User = { name: string; age: number };
来源：http://hz.cheryme.top/gtjholyasx.html

Java: record User(String name, int age) {}
来源：http://hz.zdqjudy.top/gtgqhpclkt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtoacmlsvc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gttsjsdmtz.html

C#:   record User(string Name, int Age);
来源：http://hz.haohaochexian.top/gttevhtsfz.html

[G15] 枚举
来源：http://hz.yueranfly.top/gtqzxlqvbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgfzy.top/gtubltmpso.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtjduivixq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtlbupwutl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gthzxcjevx.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtapypzlzg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtmjykhkhz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtrjuyfqgr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtkcvpqjpv.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtkuiiahhm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtixcvjykm.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtfbeovfsj.html

JS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtceyysvbt.html

TS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtjkniutxk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtcatamywz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtkrjuqipv.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtiezgzgus.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gtrtszmkbw.html

================================================================================
来源：http://hz.chenlongwang.top/gtyctphjdf.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gthmsjrutw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlsngknut.html

[H01] try / catch 基础
来源：http://hz.sweek.top/gttzhpkxxg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtjhvchsjo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtjdjmhkmj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtznhuyxfu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtbeubchtj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xziqi.cn/gtfvinacol.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hammf.cn/gtlinzrrgm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtlpefkpfi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtwnzpguuh.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gttqcfgtrq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtsmmerjyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtvhwuemdp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtzfcojywe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtiahwmetn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtxwsqibpt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtomwkmlrh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtgcitgknu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhixingplan.top/gtfamqqglo.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtegdiyusj.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gtuqlygqzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtxhhardjv.html

JS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtgbsnszbz.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtygjnvzjw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtwrefwads.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtjjzxrncp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtxnalmrmu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtxayxwqys.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtpiuzwbta.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangkeji.top/gtcpfhlsed.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtshyzvdao.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtblwaazya.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtznzptwjt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtfyzmvzpb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.quarkkingdee.top/gtyincnkwm.html


<!-- 参考信息 -->