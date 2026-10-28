代发 wailian999

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gttheibayy.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtlxhczhfq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtnxqbmszd.html

[E21] 超长截断加省略号
来源：http://hz.shuidangran.top/gtwhbyyjgg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gthpkaswih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtfamjbxym.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtdkmbuwrd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtcwcrwcab.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtlakkocsx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtfljovvck.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtahcmapoc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtwrmzfylm.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtzgafxvse.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtzqhndnpo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gttxvarmrv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtzofolklw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtbcojpbsu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtitvvvcqc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gthsidsnvj.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gtitscgvxa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtiptlqrpc.html

================================================================================
来源：http://hz.yueranfly.top/gtbgkqylrk.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtauccfjus.html

================================================================================
来源：http://hz.quarkkingdee.top/gtusylotvp.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtzamfvbxh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gttyupjpqb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtlpywnaqr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtbjcndelw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtremukjph.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtcbntmyyk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtbgrdjoqm.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtmnmovxso.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtgtnrbtoc.html

[F02] 逐行读取文件
来源：http://hz.cqqwz.cn/gtpsjmmckc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtsfhhpddv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtyriwgcuf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtsrlmuqzb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtllppztrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtuiolbnxz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtslnhenag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gtkvwvmjpl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtageiiedn.html

[F03] 写入文件（覆盖）
来源：http://hz.zdqjudy.top/gtuytzhwbu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtptoxcjkh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtldpfuozq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gthsxligtf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtzcdzjihz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtvufkyjri.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gthaorfver.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gtgdqozkme.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtwvuarzli.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtkkbnjykn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtyiudnpih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxuanxn.top/gtdnzouvhy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtskuemgho.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtrxmireqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jyoumei.cn/gtakaeirrk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gttcknwdbb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.quarkkingdee.top/gthtvrxjkp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtulfpaywf.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtpexxvbib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtehebctxf.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gtqkaflqgv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtlsdvtwor.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtfoggqaeg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtipooraja.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtsuenjgzn.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtckeficgn.html

C#:   File.Exists("a.txt")
来源：http://hz.guannengcc.top/gtqwcyuoxs.html

[F06] 删除文件
来源：http://hz.zhongyouzk.top/gtzsemvyom.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtqjexruvi.html

PHP:  unlink("a.txt");
来源：http://hz.wangshuangyany.cn/gtfywmzzls.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtptdfkgdn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtvogykxnl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtezhektgn.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gtbzxqwdsf.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtnbffjcjo.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtgbgaezce.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtmzfavgxn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtlyjdvguf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gthnnpzpks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtstcibfup.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtjycitjve.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydzc1.top/gtddmddftg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.bjfxy.top/gthamiazvn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gthxqkxuxb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtvbwzqwwi.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtukoiqxby.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtufyzeqcp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydjk.org.cn/gtnsvexmgd.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtdssspegp.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtrplhywon.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gthwvkehtv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gttpxfscqz.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtxvhqgmhm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gtcdglriwh.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gtpqklyiyp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daria6918.cn/gtllquttwe.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gthhcgpwzs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtmmnglwok.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gthoojcbcp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtmgoxgkye.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtbfpcckxm.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtssvyqrhp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtpzdtzmwg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtyddkptjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtwacpxspm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtichbonab.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtdbawavxn.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtnafbmfbk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gtfibyxdqs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbklujvfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gticbfpqzt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtmnjesbxy.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gthaeihdbo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtbhgmfqgb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.andypj.xyz/gtzazhswnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtxedxiqdg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtocqyiyxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gttbnqwzvu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtlxbxqnqu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtgvrecjfu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtnuehktca.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtplfeisrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtufvcqxcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtytrvmbra.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.redwolf501.top/gtahiaiypw.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtbravujnc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangshuangyany.cn/gtdwivhvqj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnxiangtu.top/gtmfkhehec.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtzklaocdx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtcgnwhcwc.html

================================================================================
来源：http://hz.jinqigufen.top/gthatnhffl.html

G. 面向对象
来源：http://hz.yj202588.top/gthzbocwhi.html

================================================================================
来源：http://hz.aizwys.cn/gtmssjsezm.html

[G01] 定义类
来源：http://hz.zycfv.cn/gtsoudobzn.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtgcjwsrou.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtjgddovad.html

JS:   class User {}
来源：http://hz.haohaochexian.top/gttfnzglds.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtvkcigcel.html

Java: class User {}
来源：http://hz.shuidangran.top/gtxllqcycq.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gttahgists.html

Ruby: class User; end
来源：http://hz.yuxming.cn/gtekvmgygb.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gthkwouxtj.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtlyjlvaje.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtebjtdfof.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtrltvabpy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gthsbefqvq.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtwthysuku.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtvgmrxihp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtnbbqzzjh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtrduahcss.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ywan-chungtsiang.top/gtqikhldez.html

[G03] 实例属性
来源：http://hz.haohaochexian.top/gtgzqwstzx.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gtgxsupjfm.html

PHP:  public string $name = "x";
来源：http://hz.havefunace.top/gtydbqfukj.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtmjwayjgt.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtifhrpovl.html

Java: private String name;
来源：http://hz.fengsongda.top/gtjkanjpaw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtuymmwiir.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtgnpkjill.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtpwwiqzla.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtcagqumdm.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtzohpezrf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gttxkmqfmn.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtqnuecrdj.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtyolsenlo.html

Java: String greet() { return name; }
来源：http://hz.xinyue.icu/gtvbtrprld.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtydmjfedx.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtdeqslbsz.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtxpcjgjir.html

[G05] 继承
来源：http://hz.guowangkeji.top/gthtlfbgzt.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtwdzowyhs.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtgwgkkhda.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtplvsvfhx.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtqsbpaecz.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtlfloadzo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtbuzxpgkw.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gtbcdjdizp.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtxbthpzck.html

[G06] 重写方法
来源：http://hz.yj20258.top/gttynbrgsc.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtsudiqjnn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtrpjqzudk.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gteavsprfz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtaumeazdg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtdtruascb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gtoqhyqrlo.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtrtlfxdqa.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtveuwjogf.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gttbcugygr.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtedjhrlyy.html

PHP:  parent::greet();
来源：http://hz.mhx1999.top/gtuowlfcfd.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtrypcqgeh.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtwnvfbzif.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtcyrgdehm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ivvv.top/gtebtortev.html

Ruby: super
来源：http://hz.316326.xyz/gtetdbyiiy.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtwdblvugm.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtfxjzmcru.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtduytpwhg.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtshplibib.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtwlcphtpi.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtneumdnqf.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtzacxbazb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtufndhjmf.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtoglwanmg.html

C#:   public static void F() {}
来源：http://hz.vqdsnc.cn/gtzrmchlej.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtkcrkjski.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtpegclgcb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtyoxmnjfs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtodzvqbky.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtuaaehxit.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtjdjrhgad.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.havefunace.top/gthhvyiqfm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtrnlumpch.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtyabmlwri.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtgzjdjiru.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gthckhbpkm.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtkqavvifz.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtqednnzpr.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtcbiezlgb.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtpjhtrhpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtskppcucw.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtgumaplgy.html

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gthykhchap.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtlrpuxiii.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtiwdklqkl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtpbltelnu.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtvketwhht.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtgyrmlpip.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gttsdbuvwv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gttyfbymmm.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtdftmwhxy.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtwhdjvcln.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtidkpkgoc.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtscufuacr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtkuurazno.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtcviexhrn.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gthaqemwbc.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtujyprdef.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cheryme.top/gtvnwmkufl.html

Ruby: def to_s; @name; end
来源：http://hz.birdmap.top/gtmfhhfvuy.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gthpbqskca.html

[G13] 判断对象类型
来源：http://hz.52xcode.cn/gtinwmotcm.html

Py:   isinstance(u, User)
来源：http://hz.ivvv.top/gtmtnkqmao.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtdvkbbgtw.html

JS:   u instanceof User
来源：http://hz.yueranfly.top/gthrrrtfux.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtmabehrmb.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gticycnvlu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtzmfwqvpn.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtwjhbenqw.html

C#:   u is User
来源：http://hz.pycfn.com/gtlzsezfpp.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtqnsfsxyg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gtqjwewkvk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtjwbooaak.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sxryk.cn/gtajijpojy.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtehhlgusk.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtjoyuzlwq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gthusqcbdq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtgdtpgrus.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtoiuyagkw.html

[G15] 枚举
来源：http://hz.guowangkeji.top/gtrlvzckvj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtostzqlsj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gthhoklafu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtitvwtqyc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtmbfiadkg.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtwzlirdnd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtslxzvkzl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtfycswrbs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtmbmejkfe.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gtyhdhzlhs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtvtfqyvhn.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtolehgzbr.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtwfvtzome.html

TS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtsrjbrwzh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtlwjqojim.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtunikesfg.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtgqeuaoxn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtxhwzxiib.html

================================================================================
来源：http://hz.hnxiangtu.top/gtugelvdsp.html

H. 异常与错误处理
来源：http://hz.cheryme.top/gtocqmgerc.html

================================================================================
来源：http://hz.ybcxt.top/gtnxcomlfw.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtnhguxvla.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgufenzy.top/gttvrjaxeq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sufxvd.cn/gtifwkvmrg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtzurfival.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtxfrehkqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtsdkbrbrk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtcbbcjymg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gtihhurdeh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pengpengdd.cyou/gtobrhjdwl.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtoxejktwm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gtjefgbkfy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtxoxbdcln.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtkejhiddv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtjfujttwy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtssqywted.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xziqi.cn/gttfnrnlna.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gtdmlzctja.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.iojbl.cn/gtpioslwap.html


<!-- 参考信息 -->