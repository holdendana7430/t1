代发 wailian999

Go:   if s == "" {}
来源：http://hz.yonumen.top/gtftbfnwyz.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtayzgfttt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtpruiplhy.html

[E21] 超长截断加省略号
来源：http://hz.9152youxi.cn/gthxgbhgey.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtuggeotwl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hysaishi.cn/gtgovsrzct.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtvlfbmuhp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtxdjsmhis.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtrlvzdvxw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtbwimufwi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtxvkjamrb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtyesddedz.html

[E22] 字节长度与字符长度
来源：http://hz.birdmap.top/gtcdkqhtzm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhoulong.xyz/gtqcmizrub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtbicpqlkh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtufeqitik.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtkjlkqari.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtnkmttlxc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pengpengdd.cyou/gtliwjuflx.html

Ruby: s.bytesize;  s.length
来源：http://hz.hfpthk.cn/gtxbedgyvg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtyljhkeca.html

================================================================================
来源：http://hz.iojbl.cn/gtaegkvogs.html

F. 文件与目录
来源：http://hz.zhixingplan.top/gtdpimiloq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtybtrwuhp.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtlbpxuglt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gtkjfksgzw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ivvv.top/gtlkxewnsa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.316326.xyz/gtzwubiowc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtjiwakerg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtjymsgege.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.52xcode.cn/gthkstcsre.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtpaqgscki.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.quarkkingdee.top/gtattmyvik.html

[F02] 逐行读取文件
来源：http://hz.hammf.cn/gtvqectwsm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hongshengwenyu.top/gtnicspyrx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.mhx1999.top/gthgihxdxd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtuueltbpt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtpgqznidx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtfhbngjnn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtlwsgkjis.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtygelrgax.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtfqzclxsn.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtagdnhncn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtrtvxvinm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtrcidkxfi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtchpisdfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtinmnzfee.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtcjpajuzq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtzmiphstz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtcgpvhpiw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtfmgjdzaj.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtqsjaqrrz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenlongwang.top/gtzbbvllin.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtabsinlny.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtfvqewbmt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtkxcppfzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtbbkpfhns.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtyhnkbajb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guannengcc.top/gtlrbqibam.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtswuacmiy.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydzc1.top/gtwseylvsa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dashuyun.cn/gtggcauhfc.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtpndehdyr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtbspkayny.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtosrdosar.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtiiwnrzxh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtxmssdtep.html

Ruby: File.exist?("a.txt")
来源：http://hz.gzhubu.top/gthetdyalk.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtpmwhllka.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtnstgnkjw.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtynatclab.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtddkukmmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gttbtdqgzo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtuwdjpwrg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtqtksbulo.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtrxjislqt.html

Ruby: File.delete("a.txt")
来源：http://hz.dashuyun.cn/gtwmgqkzjd.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtkzqavnnf.html

[F07] 创建目录（含多级）
来源：http://hz.sysykeji.top/gtnizvtmny.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtmjpzedzd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtbhjkesln.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtjiavfrou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gturwlpdej.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtbhaqldmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtylansnau.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtthmwupvr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gtkmlihswv.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtvctcvaal.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtmoxujwyd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtzbbelpri.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtctzovehg.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtcujeiykq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtmsxevpcf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shuidangran.top/gtmtczuoxx.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtropllgjp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtutdxwynj.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtvqocynhi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtugvtattk.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gtuackawxn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtpqpgexyz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtrloknrcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtfynerruo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cqqwz.cn/gtrudiktrm.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gteycitkfk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtwfhpmqwj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydzc1.top/gtakfmaxjf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtvvtpoojw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtqwaxgrnw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtzjksegzb.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtvwzqxpta.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtxbxqwfac.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shuidangran.top/gtnexqzdla.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtkmyzfbiw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtbxugijpd.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtnogvoqci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtssfuohdc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gthxdqurme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtgwpfcyzu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtucgybtgi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtfqppwbsv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gtlxwgwsml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtwvnuezge.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtcsxtyfto.html

[F12] CSV 读写
来源：http://hz.nwbrower.top/gtmojvnzox.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtntcmvmsu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gthqibuqaq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtsuwubkjt.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtnzwoowyy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtnjiygubu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ppjwa.cn/gtqkdlheqo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sysykeji.top/gtvhwlkefr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtzqyppeki.html

================================================================================
来源：http://hz.cashguo.top/gtavcltywp.html

G. 面向对象
来源：http://hz.zhongyouzk.top/gtuytobejj.html

================================================================================
来源：http://hz.xziqi.cn/gtstddmzbc.html

[G01] 定义类
来源：http://hz.nwbrower.top/gthqoxbhts.html

Py:   class User: pass
来源：http://hz.daria6918.cn/gtynykwbwz.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtkexetlcs.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtypcufatd.html

TS:   class User { name: string = ""; }
来源：http://hz.fzhhl.top/gtmjfzmdow.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtoyqedjwl.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtueedhezc.html

Ruby: class User; end
来源：http://hz.wangdashe.top/gtxgfyvbzm.html

C#:   class User {}
来源：http://hz.wangshuangyany.cn/gtyyaxvkie.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtulagstwa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtrdvbnrfu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtsfuhcyit.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hammf.cn/gtshhuwgqw.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gtvivaswmf.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtvnaoiaro.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtqhocsiez.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuanzx.com/gtmpprzgcn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtxyudkqqf.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtqhfitfht.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtrqulegth.html

PHP:  public string $name = "x";
来源：http://hz.gzhubu.top/gtykmbygmx.html

JS:   this.name = "x";
来源：http://hz.jianghu66.top/gtflholmce.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gtdxrrxqcv.html

Java: private String name;
来源：http://hz.sysykeji.top/gthgohtqhd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gtmbzkgkub.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtoaqoitur.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gogol.net.cn/gtsnkpnzal.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtfwztsbau.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtqttyndez.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtmxapvmyg.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtxplgaepa.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtzxaglbph.html

Java: String greet() { return name; }
来源：http://hz.meibo888.top/gtnptytjjv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gttzvzwlpo.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtoukwonei.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtijkhzati.html

[G05] 继承
来源：http://hz.cdnleiting.top/gtpzgqtcvx.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtrhnxiwkv.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtzsvktczy.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtprfjrmcb.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtcnbgtthd.html

Java: class Admin extends User {}
来源：http://hz.ydjk.org.cn/gttatmtpga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtvuxzeiha.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gtmaigruqr.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtpyklmytk.html

[G06] 重写方法
来源：http://hz.yj20258888.top/gtnqdfxogd.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtiirizjeb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtaumewjny.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtptudmzpc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtcxetmmpt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtvhsmjclk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtyolfdhsr.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtolymhyby.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtwyfphdlq.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtownbhcof.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtvnokwmqv.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtmxrrvyij.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gttmqdzmrd.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtrbpdrokx.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtzorjvitt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtvwszgqkp.html

Ruby: super
来源：http://hz.nanxinkj.top/gtabqgkvdi.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtqktbpohr.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtsmbylpum.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtokdkbxga.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtvbwdiudq.html

JS:   static f() {}
来源：http://hz.tanke756.top/gttdfmenuq.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtmbcqwdqr.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtgppwkzum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gtykyednwg.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtruxdvsiq.html

C#:   public static void F() {}
来源：http://hz.c1oappe.top/gtcpesmqcr.html

[G09] 接口 / 抽象类
来源：http://hz.cqqwz.cn/gtjxhgtmvu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtbsnhxwaz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtyvubhbqx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhengqikj.top/gtpmaqyfdl.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtgavviuwh.html

Java: interface Shape { double area(); }
来源：http://hz.xziqi.cn/gtcnyqfhdp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtcdzadwlm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtegzbuvav.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtbepglcsf.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtfvkpwepg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gthieowded.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtlscqyywr.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtmgfbujoq.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtopgssxxz.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtoyzersji.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.havefunace.top/gtjpitdokp.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtiibpfdrk.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gttxszqkjw.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtgfpfogdl.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtwtzkqswa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtlaorkgmd.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtdydjaxkj.html

TS:   get name(): string { return this._name; }
来源：http://hz.cdnleiting.top/gtygomtumc.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtwvzfsxlu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.smart0.xyz/gtvecaguxr.html

Ruby: attr_accessor :name
来源：http://hz.feifeiyinyue.top/gtevizsfkz.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gttkohwwbp.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtadtngzlp.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtwflmstlk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtxzmvhxgw.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtcoltncbb.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtztbhuxbk.html

Java: @Override public String toString() { return name; }
来源：http://hz.yonumen.top/gtxaujlnzs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtfvmwqzwl.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtbjqtiktg.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtetnmdebl.html

[G13] 判断对象类型
来源：http://hz.cashguo.top/gtdpixvjpa.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtjwsgsotn.html

PHP:  $u instanceof User
来源：http://hz.hywenlv.cn/gtwibfmqwn.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtohckawpk.html

TS:   u instanceof User
来源：http://hz.ybcxt.top/gtrmbrqlax.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gtwbzbzpvg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtvytmtwcd.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtjvsluygl.html

C#:   u is User
来源：http://hz.smart0.xyz/gtujelldvn.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gteblebfcq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ehwqpu.com/gtcekhtxlu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtfsqlyzqw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtqfstosjw.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtbdcervud.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtauglwiac.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gthohdgksp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtsdovapnu.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtgfozphum.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtmempagkz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gthvwxdtzm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtmyuragrk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtfnaoacgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtkfofdqvk.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtsncxlcps.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangkeji.top/gtacfbngei.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtrydaexiy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtddntmwsf.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtwdlubkrz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtqlmessap.html

PHP:  get_object_vars($obj);
来源：http://hz.hongshengwenyu.top/gtpndzoppa.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtqsrteqdu.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtexxfnhec.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtvdkzixpl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtroiwbevx.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gthchxqdua.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtjyhfwzxg.html

================================================================================
来源：http://hz.wangdashe.top/gttussrtnk.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtmeqisibq.html

================================================================================
来源：http://hz.haohaochexian.top/gtjjreityh.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtybwsoihf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.andypj.xyz/gtknjafymj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtzarftvsz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guannengcc.top/gtbgiihcvh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtughepjab.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gttrqydrfy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sweek.top/gtazeegszs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtqjuiklxz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtlvyncqpd.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtjfhoaqlk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtepuunhnm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtuywxrylz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtfpnrvppz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtxrcowdaz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtxdevzyil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shangyingyoupin.top/gtexsdakqs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtnhmeuazw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gtthuzowau.html


<!-- 参考信息 -->