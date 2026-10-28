代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtvrcqrbdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.52xcode.cn/gtohvmdxat.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtbotbevty.html

Java: if (s.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtchhtkmwl.html

Go:   if s == "" {}
来源：http://hz.andypj.xyz/gtigscmruh.html

Ruby: if s.empty?
来源：http://hz.smart0.xyz/gtyngxdfpc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtnfslwpef.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gtbgdmjoxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zycfv.cn/gtedzinwpv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenlongwang.top/gttcuxuokp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtciagaeff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtqvrlzntp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtyhwpikij.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gtejmvimfn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtjkenobew.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtwpmyvjyg.html

[E22] 字节长度与字符长度
来源：http://hz.dashuyun.cn/gtirhjywii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtggrfcjoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtyfjowqrm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gotoacloud.top/gtnatojccg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtzomzwlto.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtzvsrrmux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtungbwhde.html

Ruby: s.bytesize;  s.length
来源：http://hz.hongshengwenyu.top/gtgstfjbib.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.vqdsnc.cn/gtbeyahwwi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqemnjcdd.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtmtclvznc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtllohskab.html

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtrackqmsp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhoulong.xyz/gtfzjewvng.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtviikguzo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gthfhneywp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtplankkwy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtdepqfxjl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtyqxhpray.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtssdfsxjp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtuppymwff.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtgshnnwpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtjmgkxxae.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtmdjidarm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtxpvucbai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtxkknpiop.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtzwbrbmjv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtchntxurq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zycfv.cn/gtsiweyyns.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gtoongqnyn.html

[F03] 写入文件（覆盖）
来源：http://hz.tian-w.cn/gtqzdfqbph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj202588.top/gtfoormtfu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gtonlavwyv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtjfrrfhvw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtoqofwouq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtivduqkcc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yueranfly.top/gtaixgtyor.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tianlin.xyz/gtcafwybux.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yonumen.top/gtjjwxigtk.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtevlrxnyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hfpthk.cn/gtwaevylaj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtojakmicc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtrokuriaa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtklyrxmrs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gttpiagftd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtodswugww.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtqromwhrt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtuvmrkxnf.html

[F05] 判断文件或目录是否存在
来源：http://hz.jyoumei.cn/gtbgewdcnd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gtgejslcbp.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtddmnuqwg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtmluxhfyi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtzkjvwdss.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtfkuourdl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtzewiwoeo.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtzkojvirn.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258.top/gtjxqsbbxc.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gtysnezwry.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtmbluxuom.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtxmvrafuk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtojggpntv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtkfekgzep.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtamaflqlz.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtugzondpt.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtpozprlif.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtunhpnnbl.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtkpvmmqry.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtqwcqevba.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtyrcblupv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtslmyipnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtvsraicfs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtdsvpshtb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtxdfzlrgb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtauvsyjpj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gthojwtrjn.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gthklruabh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gthusjtarv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aibaodan.cn/gttsosmvhd.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtojdkxzar.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtrrffcjji.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtowfytliw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtruodcgmc.html

Ruby: Dir.children("dir")
来源：http://hz.0kj1m.cn/gtjvzxfswz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cashguo.top/gtxbscfsxj.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtazoqjctl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.smart0.xyz/gtgaguudya.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtehravwwv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtzqtpelum.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtrlnfryjk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtynycpmdf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gttalsrhsh.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtsjeamqgv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtlbzeexhp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtvvlbzhpv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtsvrhigrs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtgyoujgeo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtsiyyjxxe.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtzsdviogz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtjvpemzve.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gtbhjwqppl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtqwhoyfom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tanke756.top/gtiboysjnz.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtsignlvpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtsibpjlmb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtzthjtcig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtfrvbkycj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtwbmquliv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtfxhatzpm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtrphiryle.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtkcrejxyc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gtknfiwxgo.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtncanqjms.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.52xcode.cn/gtvvzgetxi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtiymmqvyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gttqlzogte.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtedrfwhyp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtcnzxudzs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtklhdxsmq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xinyue.icu/gtocbduxjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gttdodcgka.html

================================================================================
来源：http://hz.ehwqpu.com/gtxbhkqfau.html

G. 面向对象
来源：http://hz.sweek.top/gtuwtuhaot.html

================================================================================
来源：http://hz.nwbrower.top/gtogcolqwr.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gttmzkuqzo.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtqgzojswe.html

PHP:  class User {}
来源：http://hz.xylfe.cn/gtglfzedib.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtrtycohfa.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtdnwefvyc.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtzwbvbuhx.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtaakwoqev.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gttojvkfle.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtwxrloajb.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtndsyskll.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtmisgnjrv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtykzbfrol.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtsdwahzei.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtuzzeqzbm.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtbeghlhlx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtswwzcirh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtqqgqzsfc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gteiqvnqsc.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtbgfswymt.html

Py:   self.name = "x"
来源：http://hz.meibo888.top/gtfjaanorl.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtmsppjtiv.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gtmksfctfz.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtfgtdmmxh.html

Java: private String name;
来源：http://hz.havefunace.top/gttybornjj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gthjpgjbqh.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtehfpjyuq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtxxatxrnz.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtvwggxwub.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtzfyxtfat.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gthpnlzobn.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtbophaghh.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtcewhtdiy.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtuswgfmxs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gthsdkprpr.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtbperfhxq.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtrtveuwbo.html

[G05] 继承
来源：http://hz.zhongyouzk.top/gtrcmnftlh.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtbytjggmq.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtnripmrts.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtrltwngbd.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtvhzohnik.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gttvytcvmc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xinyue.icu/gtyzejpzpx.html

Ruby: class Admin < User; end
来源：http://hz.quarkkingdee.top/gtnomokcob.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtguvydkkc.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtosfxwoya.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtkwhoezra.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtnmrfjfxz.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gtnjyevqyy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtbecwyacn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gticozrjux.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gtexqvwwep.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gttowhbygf.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtpxchmxmm.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gtyzxalpmq.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtfbhjvlsj.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gttgxioywi.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtiplydmiy.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtdryxdegk.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtntrrxzos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtyuwkzpbb.html

Ruby: super
来源：http://hz.hywenlv.cn/gthqnzvkac.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtreceorhw.html

[G08] 静态方法与属性
来源：http://hz.snrcjt.cn/gtsfgppypn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtyolhwbun.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gteqgntkfx.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gttgsngpfy.html

TS:   static f(): void {}
来源：http://hz.zhengqikj.top/gtehekqyta.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtuxtifshv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gotoacloud.top/gtaaazpevq.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtujaertzt.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtecjcypgi.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtlyobnqbn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtvtouvyqy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtxncaplzz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuetiantiany.cn/gtmektjuia.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtlkfpiyea.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtthxqoogs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtybtlutrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtjcixehwc.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtkthhwvdx.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gtehqyskbo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtlwlnmtgc.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtgzxstemu.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtfcbkhelo.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtksmxeemw.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gttxsrcnef.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtrzsargha.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gtbqpxklug.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtprxmavgb.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtdswmbvjs.html

Py:   @property 与 @x.setter
来源：http://hz.nanxinkj.top/gtfowksizx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtbpyedwog.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtdrfbmqjq.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtjsaaqadt.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtwuzdxknh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xziqi.cn/gtkjjukokc.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtqeigruvb.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtbllmzckn.html

[G12] 对象转字符串
来源：http://hz.ydjk.org.cn/gtagdctdgk.html

Py:   def __str__(self): return self.name
来源：http://hz.yuxming.cn/gtbysbmnbd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtetedempb.html

JS:   toString() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtwcfbopip.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gteuqrtqrc.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtwiwuajol.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtovndtogj.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtyprsddjj.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gturlhovdt.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtsjizymga.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtryqeqatb.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtqpyzdthg.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtnmioslvj.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtvtarqmkd.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtocnbepnv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gticbuztvn.html

Ruby: u.is_a?(User)
来源：http://hz.xziqi.cn/gtgnlxacfq.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtkrlcnkcp.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtrvxmlrmh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtpngjiavx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtttsxsbyc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gtmhgrlsto.html

TS:   type User = { name: string; age: number };
来源：http://hz.yonumen.top/gtekwpkwrp.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtektfamkn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtucfcpxen.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtyiqehepv.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtzbdsbzso.html

[G15] 枚举
来源：http://hz.yueranfly.top/gttzsbabfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtqehdlqsx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gtsnrxqxqt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtyfmofkug.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtagxhrhja.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gthrelwlwn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtnyvbzkod.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtjmbhgwwg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtpbbfelkh.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtiqkerigb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtklaxamef.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtambbxitv.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtkasrzkwc.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtdxoozpqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtxbsfgysc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.smart0.xyz/gtotlogfvl.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gttnnxfrmb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zycfv.cn/gtrclgznfi.html

================================================================================
来源：http://hz.quarkkingdee.top/gtdrsqcbsx.html

H. 异常与错误处理
来源：http://hz.ybcxt.top/gtlnixpcad.html

================================================================================
来源：http://hz.yangfankeji.com/gtrvvcdqfc.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtkufnhynx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtkavmcjjc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtyxluxzty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtzvxtgnqz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtclgzffmj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtshsszvjt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtxwdgwksp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtshogmzin.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtzcagshua.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtsvabuhbn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.snrcjt.cn/gtzxtwpzvk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gthfgpcpxq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtjxhmpabh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtunoaajxj.html


<!-- 参考信息 -->